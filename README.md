# amlmarketplaces/deepgram

Claude Code marketplace federating all `@amlplugins/deepgram-*` plugins.

## Install

Add to your project's `.claude/settings.json`:

```json
{
  "extraKnownMarketplaces": {
    "aml-deepgram": {
      "source": { "source": "github", "repo": "amlmarketplaces/deepgram" }
    }
  },
  "enabledPlugins": {
      "deepgram-agent@aml-deepgram": true,
      "deepgram-listen@aml-deepgram": true,
      "deepgram-listen-live@aml-deepgram": true,
      "deepgram-manage@aml-deepgram": true,
      "deepgram-speak@aml-deepgram": true
    }
}
```

Then launch Claude Code in the project. The marketplace is fetched from `amlmarketplaces/deepgram`, cached under `~/.claude/plugins/cache/aml-deepgram/`, and each enabled plugin is loaded from its `amlplugins` source repo.

## Plugins (5 total)

- `deepgram-agent` — [@amlplugins/deepgram-agent](https://github.com/amlplugins/deepgram-agent)
- `deepgram-listen` — [@amlplugins/deepgram-listen](https://github.com/amlplugins/deepgram-listen)
- `deepgram-listen-live` — [@amlplugins/deepgram-listen-live](https://github.com/amlplugins/deepgram-listen-live)
- `deepgram-manage` — [@amlplugins/deepgram-manage](https://github.com/amlplugins/deepgram-manage)
- `deepgram-speak` — [@amlplugins/deepgram-speak](https://github.com/amlplugins/deepgram-speak)

## Related

- npm packages: `@amlplugins/deepgram-*` published to GitHub Packages (`https://npm.pkg.github.com`).
- Aggregating parent: [`amlmarketplaces/aml`](https://github.com/amlmarketplaces/aml) — federates every `@amlplugins/*` plugin under a single marketplace.
- AML topology: see `.claude/rules/definitions/ageni.md` § "GitHub Topology" — this repository is a Tier-4 HUB-INSTANCE under the `amlmarketplaces/` Tier-3 HUB-ORGANIZATION.

> Built by `.claude/skills/aml/metateam/marketplace/test/cross-org-amlmarketplaces-batch.mjs`.
