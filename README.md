# fukucha

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

A 2D gacha-style game built with Unity and ported to WebGL. Collect characters based on tourist spots in Fukui Prefecture, Japan.

## Demo

Play the live version at **[https://fukucha.github.io](https://fukucha.github.io)**.


![fukucha game interface](https://github.com/fukucha/fukucha/assets/1/2a3b4c5d-6e7f-8g9h-0i1j-2k3l4m5n6o7p)


## Features

-   **Gacha System:** Use a random gacha mechanic to acquire new characters.
-   **Character Collection:** Collect characters inspired by real-world locations.
-   **Simple Gameplay:** A straightforward tap-based action interface.

## How to Play

1.  Visit [https://fukucha.github.io](https://fukucha.github.io) in a desktop web browser.
2.  The game will load and start automatically.

**Requirements:**
-   A modern web browser with WebGL support.
-   This game is designed for desktop. Mobile devices will display a compatibility warning as WebGL support is not guaranteed.

## Technical Overview

The project is a standard Unity WebGL build.

-   **Game Data:** Character and location data is sourced from `tem.csv`.
-   **Entry Point:** `index.html` contains the Unity player configuration and launches the game.
-   **Build Artifacts:** The `Build/` directory contains the compiled game assets:
    -   `hukucha.data.unityweb`: Compressed game data.
    -   `hukucha.wasm.unityweb`: The WebAssembly binary.
    -   `hukucha.framework.js.unityweb`: The JavaScript runtime framework.
-   **Web Template:** The `TemplateData/` directory contains the CSS, images, and favicon for the loading screen and web page.

## License

MIT License - see [LICENSE](LICENSE).