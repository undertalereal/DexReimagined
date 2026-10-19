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
- <img width="294" height="365" alt="image" src="https://github.com/user-attachments/assets/f8851b23-f660-4f21-8f3c-f3c848ee754d" />
<img width="186" height="54" alt="image" src="https://github.com/user-attachments/assets/9f79f95a-8744-4a92-9c6c-61a8d4c99cc1" />
<img width="186" height="26" alt="image" src="https://github.com/user-attachments/assets/ffecf90c-5270-4799-b765-9605084435f7" />




### Previewers
- **Decal Preview**: right-click a `Decal`/`Texture` to see the image, asset name, owner, ID and creation date, each with a copy button.
- **Mesh Preview**: right-click a `MeshPart`/`SpecialMesh` for an orbitable 3D view with asset info.
- **Animation Preview**: right-click an `Animation` to play it on a clone of your character (drag to orbit, scroll to zoom).
- **3D Preview**: view `Model`/`BasePart` instances, with auto-rotate, auto-refresh and camera lock options.
- <img width="1182" height="889" alt="image" src="https://github.com/user-attachments/assets/f500674a-76f3-419b-9939-8882afb01d76" />


### GC Scanner
Search `getgc` results by function name, constant, upvalue, or table key/value. Click a result to copy it, or press **View** to open the owning script.
*Requires executor support for `getgc` (and `getconstants`/`getupvalues` for those modes).*
<img width="647" height="824" alt="image" src="https://github.com/user-attachments/assets/c277a630-9415-4907-b216-960f77406cc3" />


### Settings window
- Class icon set (`Old`, `NewDark`, `Vanilla3`), window title alignment and background transparency.
- Full theme color pickers, plus per-window background color overrides.
- Explorer, Properties, Script Viewer and decompiler options (fallback: Konstant, AdvancedDecompiler, Shiny).
- Press **Restart** to save and apply changes.
- <img width="294" height="473" alt="image" src="https://github.com/user-attachments/assets/acda52cf-f5b6-49eb-b7d9-678a87226480" />


### Explorer additions
- **Copy All Properties**, **Block/Unblock Remote** (needs `hookmetamethod`), **Fire ClickDetector / ProximityPrompt / TouchTransmitter**, **Save Script / Bytecode**, **Dump Functions**.
- Search filters: `/remotes`, `/bindables`, `/isa Class`, `/rad N`, `/players`, `/loadedmodules`.
- <img width="589" height="487" alt="image" src="https://github.com/user-attachments/assets/f0837362-4f1c-40a4-a0d1-aae3adf11667" />
- <img width="192" height="68" alt="image" src="https://github.com/user-attachments/assets/d57f390a-4ae5-4003-81ec-f6f18d9dada3" />



### Script Viewer
- Search bar (`Ctrl+F`) with case-sensitive, whole-word and regex toggles, and match navigation.
- **Save** writes edits back to the script's `Source` (does not affect running code).
- <img width="765" height="599" alt="image" src="https://github.com/user-attachments/assets/74f88b4b-f534-4b0d-827b-7b45d2a2bed6" />


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
