<img width="2550" height="1101" alt="25 08 2026_09 19 50_REC" src="https://github.com/user-attachments/assets/0f7a873d-93e1-4ced-9fda-57db74f46e28" />


# Dex:Reimagined

A fork of [Dex++](https://github.com/AZYsGithub/DexPlusPlus) (which comes from [Dex](https://github.com/LorekeeperZinnia/Dex)) with some extra tools I wanted. Everything Dex++ does is still here, I just added stuff on top.

## How to use it

Paste this into your executor and run it:

```lua
loadstring(game:HttpGet("https://raw.githubusercontent.com/undertalereal/Dex-Reimagined/main/dex-reimagined.lua"))()
```

## Features in 1.2

### Favorites
- Right-click any instance in the Explorer and choose **Add to Favorites** / **Remove from Favorites**.
- The **Favorites** window lists saved instance paths. Click `→` to jump to the instance in the Explorer, or `X` to remove it.
- Favorites are saved to `DexPlusPlusSettings.json` and saves between sessions. Missing instances are shown as `(missing)`.

### Previewers
- **Decal Preview**: right-click a `Decal`/`Texture` to see the image, asset name, owner, ID and creation date, each with a copy button.
- **Mesh Preview**: right-click a `MeshPart`/`SpecialMesh` for an orbitable 3D view with asset info.
- **Animation Preview**: right-click an `Animation` to play it on a clone of your character (drag to orbit, scroll to zoom).
- **3D Preview**: view `Model`/`BasePart` instances, with auto-rotate, auto-refresh and camera lock options.

### GC Scanner
Search `getgc` results by function name, constant, upvalue, or table key/value. Click a result to copy it, or press **View** to open the owning script.
*Requires executor support for `getgc` (and `getconstants`/`getupvalues` for those modes).*

### Settings window
- Class icon set (`Old`, `NewDark`, `Vanilla3`), window title alignment and background transparency.
- Full theme color pickers, plus per-window background color overrides.
- Explorer, Properties, Script Viewer and decompiler options (fallback: Konstant, AdvancedDecompiler, Shiny).
- Press **Restart** to save and apply changes.

### Explorer additions
- **Copy All Properties**, **Block/Unblock Remote** (needs `hookmetamethod`), **Fire ClickDetector / ProximityPrompt / TouchTransmitter**, **Save Script / Bytecode**, **Dump Functions**.
- Search filters: `/remotes`, `/bindables`, `/isa Class`, `/rad N`, `/players`, `/loadedmodules`.

### Script Viewer
- Search bar (`Ctrl+F`) with case-sensitive, whole-word and regex toggles, and match navigation.
- **Save** writes edits back to the script's `Source` (does not affect running code).

### Other
- Console window with syntax-highlighted command line and log output.
- Save Instance window with decompile options.
- Plugin support: place `.lua` files in `dex/plugins`.
- Mobile/touch input support.

## Requirements
Features depend on executor functions such as `getgc`, `decompile`/`getscriptbytecode`, `saveinstance`, `hookmetamethod`, `writefile` and `setclipboard`. Unsupported features are disabled automatically.

## Credits

- [Dex++](https://github.com/AZYsGithub/DexPlusPlus) by AZY
- [Dex](https://github.com/LorekeeperZinnia/Dex) by LorekeeperZinnia
- Made by soulopsundertale

Dex Serializer Plus is a separate project, based on [DexSerializer](https://github.com/LorekeeperZinnia/DexSerializer).
