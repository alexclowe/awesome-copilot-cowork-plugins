# AI Career Lab — Microsoft 365 Copilot Cowork Plugins

This repo will be auto-populated by CI from [ai-career-lab](https://github.com/alexclowe/ai-career-lab/tree/main/plugins) on the next push to `main` of the source repo.

The plugins here are profession-specific Microsoft 365 Copilot Cowork extensibility packages — generated automatically from the same SKILL files that power [awesome-claude-cowork-plugins](https://github.com/alexclowe/awesome-claude-cowork-plugins).

## ⚠️ Microsoft 365 Cowork is Frontier preview

Cowork is gated behind the [Microsoft Copilot Frontier program](https://adoption.microsoft.com/en-us/copilot/frontier-program/). Your tenant needs Frontier enrollment before these plugins will work.

## How to install (once plugins are populated)

Each plugin folder will contain a Microsoft 365 unified app manifest (`manifest.json`), profession-specific skills (`skills/`), and icons. To install one:

1. Zip the contents of the plugin folder
2. Sideload via Microsoft 365 admin center → Manage Apps → Upload custom app
3. Or sideload via Teams (Apps → Manage your apps → Upload a customized app)

Or, drop just the `skills/` folder into your OneDrive at `Documents/Cowork/skills/` for the user-level folder-drop install (no admin needed).

## Convert from Claude format

Use the [Cowork Converter](https://theaicareerlab.com/cowork-converter) to convert any Claude plugin to Cowork format and vice versa.

— [The AI Career Lab](https://theaicareerlab.com)
