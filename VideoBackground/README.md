# Video Background for BetterDiscord
This is a guide to using the plugin. When working, it will insert a `<video>` element under the page which requires some css to make visible. I provided a sample css theme that will do so.

Example: 

![](https://giant.gfycat.com/ClumsyGreenHookersealion.gif)

# Install
Download `videoBackground.plugin.js` and drop it in the BetterDiscord plugin folder. 

This can be found in:
+ `Discord settings > BetterDiscord > Plugins > 'Open Plugin Folder'`
+ `C:\Users\{name}\AppData\Roaming\BetterDiscord\plugins`

Restart discord and it should show up like so:
![](https://i.imgur.com/1wzj3HE.png)

Include the following code to your css (this is included in the sample theme):
```css
.fullscreen-bg video {
  position: fixed;
  top: 50%; left: 50%;
  z-index: -100;
  min-width: 100%;
  min-height: 100%;
  width: auto;
  height: auto;
  transform: translate(-50%, -50%);
}
```

# Setting Video
Clicking on the `Settings` button will open a window like so:

![](https://i.imgur.com/kWQK9za.png)

The link must be a direct link to any `MP4/WebM/OGG` file. This work with websites such as Streamable and Gfycat. The link must also be https:// or the video will not play. Hit save and if the css has been set up, it should appear.