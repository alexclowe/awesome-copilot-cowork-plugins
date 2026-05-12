# AI Career Lab — Microsoft 365 Copilot Cowork Plugins

Profession-specific plugins for Microsoft 365 Copilot Cowork. Each plugin is a Cowork extensibility package containing a manifest plus profession-specific skills.

Built from the same source as [awesome-claude-cowork-plugins](https://github.com/alexclowe/awesome-claude-cowork-plugins) — both repos use the [Agent Skills](https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-plugin-development) open standard, so the same SKILL files work on either platform.

## ⚠️ Microsoft 365 Cowork is Frontier preview

Cowork is a Microsoft 365 Copilot preview feature gated behind the [Microsoft Copilot Frontier program](https://adoption.microsoft.com/en-us/copilot/frontier-program/). Your tenant needs Frontier enrollment before these plugins will work.

## Install (recommended — pre-built zips)

The fastest way to install is to grab a pre-built zip from the [latest release](https://github.com/alexclowe/awesome-copilot-cowork-plugins/releases/latest):

1. Open the [latest release](https://github.com/alexclowe/awesome-copilot-cowork-plugins/releases/latest)
2. Download `<plugin-slug>.zip` (e.g., `pharmacist.zip`)
3. Sideload via **Microsoft 365 admin center → Manage Apps → Upload custom app**, or via **Teams → Apps → Manage your apps → Upload a customized app**

Releases are tagged with a UTC timestamp (`sync-YYYYMMDD-HHMMSS`) so you can pin to a specific snapshot of all plugins if you need reproducibility.

## Install (alternative — build the zip yourself)

If you prefer to inspect or customize the source before installing, each plugin folder in this repo contains the unpacked Cowork extensibility package (`manifest.json` + `skills/` + icons). To install one:

1. Zip the contents of the plugin folder (e.g., `pharmacist/`) — `manifest.json` must be at the root of the zip
2. Sideload through the same path as above

## OneDrive folder-drop alternative (no admin needed)

If you don't have admin access, you can install just the skills (without the plugin wrapper) by copying the `skills/` folder from any plugin into your OneDrive at `Documents/Cowork/skills/`. Cowork auto-discovers up to 50 custom skills per user.

## Convert from Claude format

If you'd rather author plugins in Claude format and target both platforms, use the [Cowork Converter](https://theaicareerlab.com/cowork-converter) — drag a Claude plugin zip in, get a Cowork plugin zip out (and vice versa). Free, no PowerShell required.

## License

See [LICENSE](./LICENSE).

— [The AI Career Lab](https://theaicareerlab.com)
