# Space Station 3D

Welcome to the repository. Here you'll find Space Station 3D: a 3D remake of [Space Station 13](https://spacestation13.com/).

If you haven't been there already, the [Discord Server](https://discord.gg/Z3sPhyS) should probably be your first stop. 
You'll find a lot of helpful people there, capable of answering any questions you may have.

## Code of Conduct

This project and everyone participating in it are governed by the [Code of Conduct](CODE_OF_CONDUCT.md). 
By participating, you are expected to uphold this code.
Please report any unacceptable behavior to an admin.

## Setting up the project

### Quickstart Guide

1. Clone the repository
    * Clone the **master** branch for the latest stable version
    * Clone the **develop** branch for the development version
2. Make sure to git everything
    * Initialize git submodules `git submodule  update --init`
    * Pull git lfs `git lfs pull`
    * Or you git client's equivalent. Some clients do this automatically
3. Open the project in Unity
4. Compile the asset bundles
    * Open the Asset Bundle Browser: *Window > AssetBundle Browser > Build*
    * Make sure that *"Copy to StreamingAssets"* is checked
    * Click *Build*
5. Run the server
    * *Build > (Build and) Run Server > Your Platform*
    * There's no guarantee the game will run without a server
    * You only need to rebuild the server when the code changes
    * All non-code assets are build into asset bundles
6. Run the client
    * For testing run the Client scene
    * To build a standalone client, run *Build > Client > Your Platform*

### Tools and Setup

> **tldr;**
>
> * **Unity 2019.1.x**
> * **Git** with **Git LFS**
> * Whatever tool you need to do your thing

The game is developed in **Unity 2019.1.x**. Regardless of if you make code or art, installing Unity will be helpful for getting your contribution in. Upgrading to the next patch version of Unity is perfectly acceptable, but avoid downgrading. The plan is to eventually upgrade to the **2019.4 LTS** version when it comes out and stay on that version until a new feature warrants an upgrade, or support stops.

For coding, you can use whatever you want, but [Visual Studio](https://visualstudio.microsoft.com/) is probably the most popular choice. It's free and integrates well with Unity. If you're a student, we recommend getting a copy of [ReSharper](https://www.jetbrains.com/resharper), which adds a lot of code hints and shortcuts that will significantly improve your code quality.

The art style guide recommends using **Blender** for 3D models, but as long as the look and performance match the existing assets, any 3D modeling tool is allowed.

To get a hold of the project, you need a **git client**. Git is the software that manages the source. GitHub is the website that we use to host it. Some of the popular options are:

* [GitHub Desktop](https://desktop.github.com/), recommended for beginners
* [Sourcetree](https://www.sourcetreeapp.com/)
* [Smart Git](https://www.syntevo.com/smartgit/)
* [Git Kraken](https://www.gitkraken.com/)
* [Git CLI](https://git-scm.com/), if you know what you're doing

Regardless of what client you use, we recommend installing the latest version of git separately, to make sure you have all the latest features, specifically **Large File Storage** (LFS).

## Troubleshooting

> When opening the project:`error CS0234: The type or namespace name '<class>' does not exist in the namespace 'Brisk'`

The git submodule has not been initialized. Run `git submodule update --init` or your gui's equivalent.

---

> Some models are missing/invisible

This will be resolved soon, but installing Blender and reimporting the models may fix it.

---

> When running the server: `DirectoryNotFoundException: Could not find a part of the path "D:\Projects\SS3D\Build\Server\StandaloneWindows64\SS3D_Server_Data\StreamingAssets\assets".`

The asset bundle has not been build. See the [quickstart guide](#quickstart-guide).

## Contributing

Have a look at [CONTRIBUTING.md](CONTRIBUTING.md) for documentation on how to get your stuff in the game.

### Forking the repository

If you wish to contribute to this project, you should fork this repository on GitHub, using the Fork button on this page. This naturally requires a GitHub account. You will commit your changes to that repository and make a [pull request](#pull-requests) to merge it into our repository. See [the Contribution Guide](CONTRIBUTING.md)

Soon you will probably find your fork to be out of date. GitHub has made a [pretty clear guide](https://help.github.com/articles/syncing-a-fork/) on how to sync your fork so it is up to date with the shared repository.
