<img width="2550" height="1101" alt="25 08 2026_09 19 50_REC" src="https://github.com/user-attachments/assets/0f7a873d-93e1-4ced-9fda-57db74f46e28" />


# Dex:Reimagined

A fork of [Dex++](https://github.com/AZYsGithub/DexPlusPlus) (which comes from [Dex](https://github.com/LorekeeperZinnia/Dex)) with some extra tools I wanted. Everything Dex++ does is still here, I just added stuff on top.

## How to use it

Paste this into your executor and run it:

```lua
loadstring(game:HttpGet("https://raw.githubusercontent.com/undertalereal/Dex-Reimagined/main/dex-reimagined.lua"))()
```

## Current Features

**Viewers**
- **3D Model Viewer** – preview a model in a little 3D window.
- **Decal Preview** – right click a Decal or Texture to see the image, plus its name, owner, asset ID and when it was made. Each one has a copy button. There's also a "Decal Viewer" tile in the menu.
- **Animation Preview** – right click an Animation and it plays on a copy of your character.
- **Mesh Preview** – right click a MeshPart or SpecialMesh to look at it.

**Explorer**
- **Favorites** – right click something to add or remove it from favorites. They get saved, so they're still there next time.
- **Copy All Properties** – right click one object and it copies every property as a Lua table (`local Properties = { ... }`). Properties that can't be written out (like other Instances) are left as `nil` with a comment saying what they were.

**Script Viewer**
- **Find bar** – search while you type, not case sensitive. Has up/down buttons, a match counter, and it highlights and scrolls to the match.
- **Save button** – sits between Execute and Clear, writes your edits back to the script's `Source`.

**Settings**
- **Theme colors** – 15 color pickers (window, panel, outlines, buttons, text and so on) and a Reset Colors button.
- **Per-window colors** – give Explorer, Properties, Console, Save Instance or Favorites their own background color.

## Things to know

- Theme changes need you to hit **Save** and then **restart Dex** to show up.
- Per-window colors only work on windows that have a fixed title (the five above).
- The **Highlight** color is in the list but nothing uses it yet.
- The script Save button doesn't change code that's already running. It only changes the saved `Source`.
- Copy All Properties needs an executor that has `setclipboard`.

## Credits

- [Dex++](https://github.com/AZYsGithub/DexPlusPlus) by AZY
- [Dex](https://github.com/LorekeeperZinnia/Dex) by LorekeeperZinnia
- Made by soulopsundertale

Dex Serializer Plus is a separate project, based on [DexSerializer](https://github.com/LorekeeperZinnia/DexSerializer).
