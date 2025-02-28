# Unity.SceneViewAlign

Allow the scene view camera to use X / Y or X / Z

Basically, for a 2.5D project I needed to use 2D physics but with a camera with perspective (think [Don't Starve](https://store.steampowered.com/app/219740/Dont_Starve/) or [Cult of the Lamb](https://store.steampowered.com/app/1313140/Cult_of_the_Lamb/)). The issue is that Unity's 2D physics cannot be changed from the X / Y axis, so instead of having the plane on the X / Z axis, I needed it to be on the X / Y, which made for some awkard camera movement inside the editor.

This tools fix this issue by allowing you to toggle between the two mode easily.

In the end, whichever axis points up don't matter, the math is the same.

## Usage

![Screenshot](/Documentation~/Screenshot.png?raw=true)

Click on the newly added button in the scene view to switch between Y or Z align.

## Installation

Add the dependency to your `manifest.json`

```json
{
  "dependencies": {
    "jd.boiv.in.scene-view-align": "https://github.com/starburst997/Unity.SceneViewAlign.git"
  }
}
```

## Warning

Due to an annoying bug, if you are simply "looking" by holding the right-click button, the context menu would appears. Instead, this plugin will overwrite the default shortcut so you need to hold ALT while you right-click to show the context menu. Personally, I've never used the context menu in the scene view, so that workaround suits me.

## Authors

I simply made a UPM package for easy integration into any unity project, see those links for the original code.

- Akulist's [Forum Thread](https://forum.unity.com/threads/change-scene-view-camera-behaviour.649624/)
- FreyaHolmer's [Gist](https://gist.github.com/FreyaHolmer/cca9d07a306fb357c7ab9cc82574fabd)