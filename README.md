# Austin Unimpressed AGS

This repository contains an Adventure Game Studio (AGS) game project titled "Austin Unimpressed". The game is built and deployed to GitHub Pages using a CI/CD workflow.

## Project Overview

- **Game Engine**: Adventure Game Studio (AGS) v3.6.2.18
- **Deployment**: Automated build and deploy to GitHub Pages on pushes to the `main` branch or manual dispatch.

## Building Locally

1. Install AGS Editor from [https://www.adventuregamestudio.co.uk/](https://www.adventuregamestudio.co.uk/).
2. Open the `.agf` project file in AGS Editor.
3. Compile the game for Web platform.
4. Serve the `Compiled/Web` folder using a local web server (e.g., Python's `http.server` or VS Code Live Server).

## Deployment

The GitHub Actions workflow (`deploy.yml`) handles building and deploying the game to GitHub Pages. It:
- Downloads AGS Editor.
- Compiles the project.
- Renames the output to `index.html`.
- Deploys to Pages.

To trigger a manual deploy, go to the Actions tab and run the "Build and Deploy AGS Web" workflow.