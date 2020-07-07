# Babylon 4 Hackathon

A Babylon.js sample project using typescript, latest babylon.js es6 core module, webpack 4 with webpack dev server, hot loading, eslint, vscode support and more.

## Setup

You can clone and delete this repository's history and start a new git project by running the below script. You need to create your own github repo first. Replace <your-project-name> with your own github project url.

```git
git clone --depth=1 https://github.com/Yonet/Babylon4Hackathon.git <your-project-name>
```

OR 
```git

// Clone the seed project
git clone --depth=1 https://github.com/Yonet/Babylon4Hackathon.git

-- Remove the history from the repo
rm -rf .git

-- recreate the repos from the current content only
git init
git add .
git commit -m "Initial commit"

-- push to the github remote repos ensuring you overwrite history
git remote add origin git@github.com:<YOUR ACCOUNT>/<YOUR REPOS>.git
git push -u --force origin main

```

## How to update your project to latest seed?

<!-- Whenever there is a new update for  [Mixed Reality Toolkit](https://microsoft.github.io/MixedRealityToolkit-Unity/README.html?WT.mc_id=hololensseedproject-github-ayyonet) or [Azure Spatial Anchors](https://docs.microsoft.com/azure/spatial-anchors/?WT.mc_id=hololensseedproject-github-ayyonet) packages, this repo will be updated with the latest version. You can automaticly get the latest packages by adding the seed repo as your upstream and pulling from it.  -->

```
git remote add upstream https://github.com/RaananW/babylonjs-webpack-es6.git
git pull upstream master
```

You can check to see if your remote origin and upstream by running:

```
git remote -v
```

You can remove the upstream anytime by running:

```
git remote remove upstream https://github.com/RaananW/babylonjs-webpack-es6.git
``` 

## Getting started

To run the basic scene:

1. run `npm install` to install the needed dependencies.
2. run `npm start`
3. A new window should open in your default browser. if it doesn't, open `http://localhost:8080`

Running `npm start` will start the webpack dev server with hot-reloading turned on. Open your favorite editor (mine is VSCode, but you can use nano. we don't discriminate) and start editing.

The entry point for the entire TypeScript application is `./src/index.ts`. Any other file imported in this file will be included in the build.

To debug, open the browser's dev tool. Source maps are ready to be used. In case you are using VSCode, simply run the default debugger task (`Launch Chrome against localhost`) while making sure `npm start` is still running. This will allow you to debug your application straight in your editor.

<!-- ## Loading different examples

The `./src/scenes` directory contains a few examples of scenes that can be loaded. To load a specific scene, add a `?scene=FILENAME` to the URL (i.e. to load the ammo physics demo, use `http://localhost:8080/?scene=physicsWithAmmo`).

More and more scenes will be slowly added.

## What else can I do

To lint your source code run `npm run lint`

To build the bundle in order to host it, run `npm run build`. This will bundle your code in production mode, meaning is will minify the code.

Building will take some time, as it will build each sample (and create a different module for each). If you want to speed up the process, define the scene you want to render in `createScene.ts` (you can see the comment there)

## What is this

That's an abstract question! What is which one of those wonderful things?

Babylon.js is [the world's leading WebGL engine](https://babylonjs.com) that starts with a 'b'. You should give it a try and leave those other numbers and letters behind. To read more about it and see some amazing samples, go to the [Babylon.js website](https://babylonjs.com), [Babylon's Playground](https://playground.babylonjs.com) or [Babylon's documentation](https://doc.babylonjs.com).

The rest? You should know already, this is why you are here.

## What is covered

- Latest typescript version
- Simple texture loading (using url-loader)
- dev-server will start on command (webpack-dev-server)
- A working core-only example of babylon
- Full debugging with any browser AND VS Code
- (production) bundle builder.
- eslint default typescript rules integrated -->
