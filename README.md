# github-action-unity-example

[![Release on Main 😎](https://github.com/NextFaze/github-action-unity-example/actions/workflows/main.yml/badge.svg)](https://github.com/NextFaze/github-action-unity-example/actions/workflows/main.yml)

Using the Kart Template, and GameCI docker images - this will release a WebGL version of the game to Github Pages

Built project should be available via [GH Pages link](https://nextfaze.github.io/github-action-unity-example/), as well as a [Prerelease](https://github.com/NextFaze/github-action-unity-example/releases)

### Notes on creation

- Had to enable Decompression Fallback under Project Settings > Player > Publishing Settings for the WebGL player to load.
- Tested locally by building and running `python -m SimpleHTTPServer` in the build folder
- Initially created using Personal license, but you can also use professional license serial. More details in the [docs](https://unity-ci.com/docs/github/activation)

### Usage

This is following the Personal license steps [here](https://unity-ci.com/docs/github/activation#personal-license)

- Copy the `.github/workflows` folder into your project
- Set the `unityVersion` to your required version in `activation.yml`
- Set the `PROJECT_NAME` enviroment variable in `main.yml` to your preferred Project Name
- Run the `Acquire activation file` action to create your ulf file
    - This will be an Action Asset
- Upload the ulf file to https://license.unity3d.com/manual
- You should now receive your license file (Unity_v20XX.x.ulf) as a download.
- Open Github > <Your repository> > Settings > Secrets.
- Create a secret called UNITY_LICENSE and copy the contents your license file into it.

