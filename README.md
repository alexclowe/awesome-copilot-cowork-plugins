# AI Career Lab — Microsoft 365 Copilot Cowork Plugins

Profession-specific plugins for Microsoft 365 Copilot Cowork. Each plugin is a Cowork extensibility package containing a manifest plus profession-specific skills.

Built from the same source as [awesome-claude-cowork-plugins](https://github.com/alexclowe/awesome-claude-cowork-plugins) — both repos use the [Agent Skills](https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/cowork-plugin-development) open standard, so the same SKILL files work on either platform.

## ⚠️ Microsoft 365 Cowork is Frontier preview

Cowork is a Microsoft 365 Copilot preview feature gated behind the [Microsoft Copilot Frontier program](https://adoption.microsoft.com/en-us/copilot/frontier-program/). Your tenant needs Frontier enrollment before these plugins will work.

## Install

Each plugin folder contains a Microsoft 365 unified app manifest (`manifest.json`) plus skills and icons. To install one:

1. Zip the contents of the plugin folder (e.g., `pharmacist/`) — `manifest.json` should be at the root of the zip
2. Sideload via Microsoft 365 admin center → Manage Apps → Upload custom app
3. Or sideload via Teams (Apps → Manage your apps → Upload a customized app)

## OneDrive folder-drop alternative (no admin needed)

If you don't have admin access, you can install just the skills (without the plugin wrapper) by copying the `skills/` folder from any plugin into your OneDrive at `Documents/Cowork/skills/`. Cowork auto-discovers up to 50 custom skills per user.

## Convert from Claude format

If you'd rather author plugins in Claude format and target both platforms, use the [Cowork Converter](https://theaicareerlab.com/cowork-converter) — drag a Claude plugin zip in, get a Cowork plugin zip out (and vice versa). Free, no PowerShell required.

## License

See [LICENSE](./LICENSE).

— [The AI Career Lab](https://theaicareerlab.com)
