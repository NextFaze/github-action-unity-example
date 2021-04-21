# github-action-unity-example

[![Release on Main 😎](https://github.com/NextFaze/github-action-unity-example/actions/workflows/main.yml/badge.svg)](https://github.com/NextFaze/github-action-unity-example/actions/workflows/main.yml)

Using the Kart Template, and GameCI docker images - this will release a WebGL version of the game to Github Pages

Built project should be available via [GH Pages link](https://nextfaze.github.io/github-action-unity-example/)

### Notes on creation

- Had to enable Decompression Fallback under Project Settings > Player > Publishing Settings for it to load.
- Tested locally by building and running `python -m SimpleHTTPServer` in the build folder
- Initially created using Personal license, but you can also use professional license serial. More details in the [docs](https://unity-ci.com/docs/github/activation)