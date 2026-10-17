# Super Mario Platformer in Unity

A 2D Super Mario style platformer built with Unity and C# for the Master Advanced Practical at Heidelberg University, with three levels, enemies and power-ups.

**[Play it in your browser](https://heidelberg-university.github.io/super-mario-platformer-unity/)**

| | |
|---|---|
| Course | Master Advanced Practical (computer games) |
| University | Heidelberg University, M.Sc. Data and Computer Science |
| Semester | Winter 2023/24 |
| Type | Team project |

## Features

- A start screen, a loading screen and three levels (`1-1`, `1-2` and `1-3`).
- Player movement, jumping and fireballs.
- Enemies that can be defeated by jumping on their heads, including Koopa shells that can be kicked.
- Bricks, coin bricks, power-ups, stairways and a castle that ends each level.
- A game manager that tracks game status and moves between scenes.

## Repository structure

| Path | Contents |
|---|---|
| `Assets/Scenes/` | Start, loading and level scenes |
| `Assets/Scripts/` | Gameplay scripts, grouped into player, enemy and system scripts |
| `Assets/` | Sprites, fonts, audio and other game assets |
| `Packages/`, `ProjectSettings/` | Unity package manifest and project settings |
| `index.html`, `Build/`, `TemplateData/` | WebGL build published with GitHub Pages |
| `WebgL/` | Compressed copy of the WebGL build |
| `html/` | Code documentation generated with Doxygen from the configuration in `Codes` |

## Getting started

**Play online.** The game is published with GitHub Pages at [heidelberg-university.github.io/super-mario-platformer-unity](https://heidelberg-university.github.io/super-mario-platformer-unity/).

**Play locally.** Browsers block WebGL builds opened directly from disk, so serve the repository root and open the address it prints:

```sh
python3 -m http.server 8000
```

The copy in `WebgL/` is gzip-compressed and needs a server that sends `Content-Encoding: gzip`; see Unity's guide to [deploying compressed builds](https://docs.unity3d.com/2022.3/Documentation/Manual/webgl-deploying.html).

**Open the project.** Install Unity 2022.3.17f1 through Unity Hub, add this folder as a project, and open `Assets/Scenes/StartingScene.unity`.

## Tech stack

Unity 2022.3, C#, Doxygen.

## Team

Rishabh Tiwari and RakkiG.
