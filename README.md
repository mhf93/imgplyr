<img src="https://raw.githubusercontent.com/mhf93/imgplyr/refs/heads/main/imgplyr%20logo%20gif.gif">

# IMGPLYR
Image Slideshow Performance Software
 
**Version 1.7**  
© 2026 John Zobele | A zobele.co Project
 
---
 
## What is IMGPLYR?
 
IMGPLYR is an image slideshow player built for live use. Load a folder of images and play them back automatically on a timer, advance them manually at your own pace, switch between different image sets on the fly, and display them in a variety of visual styles — all without stopping the show.
 
---
 
## Supported Image Formats
 
PNG · JPG / JPEG · GIF · BMP · PPM · PGM · WEBP
 
---
 
## Getting Started
 
When you open IMGPLYR you will see a control bar across the top and a black display area below. Nothing plays until you load a folder.
 
**To load images and start playing:**
 
1. Click **Load ▾** in the control bar
2. Select **Load Main**
3. Browse to and select a folder of images
4. Click **Start**
The images will begin cycling automatically. Every image in the folder is shown once in a random order before anything repeats.
 
---
 
## Control Bar
 
All controls live in the bar at the top of the window. From left to right:
 
**Load ▾** · **Start/Pause** · **Background ▾** · **Speed ▾** · **Scale ▾** · **Motion ▾** · **Styles ▾** · **Effects ▾** · **Settings ▾**
 
The **status bar** on the right shows live information — which image you are on, which bank or folder is active, speed confirmations, and other feedback.
 
---
 
## Loading Images
 
### Load Main
Your primary image folder. This is what plays by default.
 
### Load Trigger
A special folder for images you want to display on demand using the number keys. Name the files `1.png`, `2.jpg`, `3.png`, and so on up to `9`. When you press the corresponding number key, that image is displayed immediately and held until you advance the queue.
 
### Load Are.na Channel…
Loads images directly from a public [Are.na](https://www.are.na) channel via the Are.na API. No account is required for public channels.
 
1. Click **Load ▾ → Load Are.na Channel…**
2. Paste any Are.na channel URL (e.g. `https://www.are.na/username/channel-name`)
3. Click **OK**
IMGPLYR fetches all image blocks in the channel and loads them into the main image pool, exactly as if you had loaded a local folder. The status bar shows live progress while fetching. Only **Image** type blocks are loaded — text, links, and embeds are skipped.
 
> **Note:** Are.na's API rate-limits requests. IMGPLYR spaces out page fetches automatically and retries if a rate-limit response is received. Very large channels may take a moment to load fully, the app may be unresponsive while this occurs.
 
### Load Bank 1–8
Eight extra image folders, each assigned to a function key (F1–F8). You can pre-load all eight before you begin, then switch between them live during playback by pressing the matching key. Switching banks does not interrupt the current image — the change takes effect on the next advance.
 
### Include Subfolders
A toggle at the bottom of the **Load ▾** menu. When enabled, loading any folder (Main or Banks) will also include images from all nested subfolders inside it. Off by default.
 
### Restore Last Loaded
Reloads every source you had open the last time you closed the program — local folders and Are.na channels alike. Folders that have been moved, renamed, or are on a disconnected drive are skipped and listed in a summary. Are.na channels are re-fetched live, so any new images added to the channel since your last session will appear automatically.
 
### Clear All Loaded
Removes every currently loaded source — Main folder or Are.na channel, Trigger folder, and all Banks — and stops playback. A confirmation dialog appears before anything is cleared. The Start button is disabled until new images are loaded.
 
---
 
## Playing Images
 
### Start / Pause
Click **Start** to begin automatic playback. Click **Pause** to freeze on the current image. The timer keeps track of the beat so resuming does not restart the clock from scratch.
 
### Advancing Manually
You can advance to the next image at any time, even while the slideshow is running:
 
| Key | What it does |
|---|---|
| **Enter** | Next image |
| **Left Arrow** | Previous image |
| **Right Arrow** | Next image |
| **Space** | Pause or Resume |
 
When you manually advance while the slideshow is running, the next automatic advance still happens at the original scheduled time — your manual tap does not reset the timer.
 
### Return to Main Folder
Press **Backspace** to switch back to the Main folder immediately and jump to the next image in the main queue.
 
### Triggering Images on Demand
Press **1 through 9** to show a specific image from your trigger folder. The image is held on screen — the slideshow keeps timing in the background but does not show anything new until you dismiss the trigger.
 
Press **Enter** to dismiss the trigger. The slideshow then advances to the **next** image in the queue, not the one that was showing before.
 
### Blanking the Screen
Press **0** to hide whatever is on screen without pausing the timer. The queue continues advancing silently. Press any advance key (Enter, Right Arrow) to un-blank — the display shows the **next** image in the queue.
 
- In **Collage Mode**, blanking clears the entire canvas. Un-blanking starts fresh from the current queue position.
- In **Screensaver** and **XP Trails** modes, blanking pauses the animation and clears the canvas. Un-blanking resumes with the next image.
---
 
## Switching Banks Live
 
Once you have loaded banks using **Load ▾ → Load Bank 1–8**, press **F1 through F8** at any time to switch the active image pool to that bank. The current image stays on screen — the new bank takes effect on the next advance.
 
Press **Backspace** at any time to return to the Main folder.
 
If the Pop-Out Controls window is open, bank buttons (labelled F1, F2, etc.) appear in the navigation row automatically for each loaded bank.
 
---
 
## Background
 
The **Background ▾** dropdown controls what appears behind your images. It is divided into three sections.
 
> **Compatibility note:** Gradient and image backgrounds are not available when Kuleshov Mode, Two Images Classic, Collage Mode, Screensaver Mode, or XP Trails Mode is active. They are also not available while any Effect is enabled. Similarly, Effects are disabled while a gradient or image background is active.
 
### Solid Color
Six preset options plus **Custom…** which opens a colour picker.
 
### Gradient
Select **Edit Gradient…** to open the gradient editor.
 
- The row of colour swatches represents each colour stop. Click any swatch to change it.
- **+ Add Stop** adds a new colour stop. **− Remove last** removes the last one. Minimum two stops.
- Choose a direction: **Left → Right** or **Top → Bottom**.
- The live preview at the bottom updates as you make changes.
- Click **Apply** to set the gradient. Click **Cancel** to discard.
Select **Clear Gradient/Image** to remove the gradient and return to the current solid colour.
 
### Image Background
Click **Load Image…** to pick any image file as your background. Choose how it fills the window:
 
- **Fit: Stretch** — stretches the image to exactly fill the window. May distort proportions.
- **Fit: Crop** — fills the window while keeping proportions, cropping the edges.
- **Fit: Tile** — repeats the image at its original size to cover the window.
Click **Clear Gradient/Image** to remove the background image and return to solid colour.
 
---
 
## Speed
 
The **Speed ▾** dropdown controls how fast images advance during automatic playback.
 
### Quick Presets
Choose from 20, 50, 90, or 120 images per minute. The equivalent time-per-image is shown next to each option.
 
### Custom…
Enter any images-per-minute value you like, including decimals.
 
### Record Speed…
The most accurate way to set speed. Opens a small floating window.
 
1. Press **Enter** each time you want an image to advance — do this in time with music, a metronome, or your own natural pace.
2. After at least 3 taps, the **Apply** button becomes available.
3. Click **Apply** to set the average interval between your taps as the new speed.
The window shows a running count of taps and the current average in images per minute and seconds per image. Click **Cancel** to discard without changing speed.
 
### Tempo Override (Up / Down Arrow Keys)
While the slideshow is playing, hold or press **Up Arrow** to run at **2× speed** and **Down Arrow** to run at **0.5× speed**. The Speed menu lets you choose between two activation modes:
 
- **Hold to activate** — speed is modified only while the key is held down.
- **Press to toggle** — press once to activate, press again to deactivate.
---
 
## Scale
 
Click **Scale ▾** to open a small floating panel with a vertical slider.
 
- Drag the slider **up** to make images larger, **down** to make them smaller.
- The percentage is shown above the slider and updates live.
- Quick buttons set the scale to **50%**, **100%**, or **150%** instantly.
- Click **Close** to dismiss the panel. The panel can stay open while you continue using the slideshow.
When **Kuleshov Mode** or **Two Images Classic** is active, the Scale panel also shows a **Pane Gap** slider that controls the width of the space between the two image panels.
 
---
 
## Motion
 
Click **Motion ▾** to open the motion settings panel. These controls apply to **Screensaver Mode** and **XP Trails Mode**.
 
### Motion Speed
A vertical slider from 0.5 to 10 pixels per frame. Higher values make the image move faster across the screen.
 
### Advance on Wall Hit
When enabled, the slideshow automatically advances to the next image in the queue every time the image bounces off any edge of the window. Off by default.
 
---
 
## Styles
 
### Centered (default)
The image sits in the middle of the screen with equal space on all sides. The Scale slider controls how large the image appears.
 
### Crop to Window
The image fills the entire screen edge to edge, cropping the sides or top/bottom as needed.
 
### Stretch to Window
The image is stretched to fill the exact dimensions of the window. Proportions are not preserved.
 
### Kuleshov Mode
The screen is split into two side-by-side panels. Each advance updates **one panel at a time**, alternating left and right. The gap between panels is adjustable via the Scale panel.
 
> Not available when a gradient or image background is active.
 
### Two Images Classic
The same two-panel layout as Kuleshov Mode, but **both panels update at the same time** on every advance.
 
> Not available when a gradient or image background is active.
 
### Collage Mode
Images accumulate on screen at random positions, layered on top of each other. The first image each session is placed centred. Up to 50 tiles can be visible at once — once the limit is reached, the oldest tile is removed as each new one arrives.
 
> Not available when a gradient or image background is active.
 
### Screensaver Mode
The current image drifts around the window and bounces off the edges, DVD-style. Each advance loads the next image in the queue and continues from the same position and direction the previous image was moving.
 
**U key — Reposition:** teleports the image to a new random position and direction without advancing the queue.
 
Use the **Motion ▾** panel to adjust speed and enable wall-hit advances.
 
> Not available when a gradient or image background is active.
 
### XP Trails Mode
Similar to Screensaver Mode, but the image leaves ghost stamps on the canvas as it moves. Stamps accumulate over time and are never erased — the canvas builds up layer after layer as the image bounces around. Each advance loads the next image and continues from the same position; the trail history remains on screen. Can be CPU heavy so may be choppy on lower end computers or with higher resolution images.
 
**U key — Reposition:** advances to the next image and places it at a new random position without clearing the trail.
 
Use the **Motion ▾** panel to adjust speed and enable wall-hit advances.
 
> Not available when a gradient or image background is active.
 
---
 
## Effects
 
The **Effects ▾** dropdown applies visual processing to your images. Multiple effects can be active at the same time.
 
> **Compatibility note:** Effects are not available when a gradient or image background is active. Gradient and image backgrounds are not available while any effect is enabled.
 
### Drop Shadow
Adds a soft drop shadow behind the image. Options:
- **Shadow Colour…** — opens a colour picker for the shadow.
- **Shadow Settings…** — opens a panel to adjust angle, distance, blur radius, and opacity.
### Inner Glow
Adds a soft glow along the inside edges of the image. Options:
- **Glow Colour…** — opens a colour picker for the glow.
- **Glow Settings…** — opens a panel to adjust radius, feather, and opacity.
### Black & White
Converts the image to greyscale.
 
### Gradient Map
Remaps the image's luminance through a custom colour gradient, replacing tones with colour. Click **Edit Gradient Map Colours…** to open the gradient map editor and set the colour stops.
 
### Threshold
Converts the image to pure black and white using a luminance cutoff. Click **Threshold Settings…** to adjust the cutoff level.
 
### Dither
Applies a pixel-art style ordered dither to the image. Click **Dither Settings…** to adjust the scale of the dither pattern.
 
---
 
## Screenshot
 
Press **P** to save a rendered image of the current display to your **Pictures/IMGPLYR Screenshots** folder. The screenshot does not include the control bar. **XP Trails Mode** currently does not work with this feature.
 
To change the save folder, go to **Settings ▾ → Screenshot Folder…**
 
---
 
## Settings
 
### Fullscreen (F11)
Puts the window in fullscreen on whichever monitor it is currently on. Press **Escape** to exit.
 
### Hide Controls (C)
Hides the control bar so the image fills the entire window. Press **C** again to bring it back. All keyboard shortcuts continue to work while the bar is hidden.
 
### Order: Random / Order: Alphabetical
- **Random** (default) — shuffles the folder; every image is shown once before anything repeats.
- **Alphabetical** — plays images in filename order, A to Z.
### Screenshot Folder…
Opens a folder browser to choose where screenshots are saved. Default is **Pictures/IMGPLYR Screenshots**.
 
### Pop Out Controls
Opens the control bar as a separate floating window. The main bar is hidden when the pop-out is open. See [Pop-Out Controls](#pop-out-controls) below.
 
### Edit Keybindings…
Opens the keyboard shortcut editor. See [Customising Keyboard Shortcuts](#customising-keyboard-shortcuts).
 
### Export Session Settings…
Saves all current settings to a `.imgplyr` file that you choose. The file captures everything: loaded folder and Are.na channel paths, speed, image order, display style, scale, background, motion settings, and every effect with its full sub-settings (shadow angle, glow radius, gradient map colours, etc.). The file is plain JSON and can be opened in any text editor.
 
### Import Session Settings…
Loads a `.imgplyr` file and applies all settings to the current session. Local folders are re-validated for existence, Are.na channels are re-fetched live, and anything not found is listed in a summary dialog. All menus and checkbuttons update to reflect the restored state.
 
### Open Current Image in Folder
Opens the folder containing the currently displayed image in your system file browser, with the image selected where supported.
 
### Help / Shortcuts
Opens a quick reference inside the app.
 
---
 
## Pop-Out Controls
 
**Settings ▾ → Pop Out Controls** moves the control bar into a floating window that can be positioned anywhere — including a second monitor while the main window is fullscreen.
 
**Top row:** Load ▾ · Start/Pause · Background ▾ · Speed ▾ · Scale ▾ · Motion ▾ · Styles ▾ · Effects ▾ · Settings ▾
 
**Bottom row:** ◄ Back · Next ► · ↩ Main · one button per loaded bank (F1, F2, etc.)
 
All keyboard shortcuts work when the pop-out window has focus. To close the pop-out and restore the main bar, click the × or go to **Settings ▾ → Dock Controls** inside the pop-out.
 
---
 
## Customising Keyboard Shortcuts
 
**Settings ▾ → Edit Keybindings…** opens a scrollable table of every action and its current shortcut, divided into two sections: standard actions and effect toggles.
 
1. Click the text box next to the action you want to rebind. It turns **yellow**.
2. Press the key you want to use. The box turns **green**.
3. Click **Save** to apply all changes.
**Right-click** any field to clear its binding (sets it to unset). Unset fields are shown in grey with `— unset —`.
 
**Revert to Defaults** resets every shortcut in the editor (you still need to click **Save**). **Cancel** discards all changes. Your shortcuts are saved and restored automatically on every launch.
 
### Effect Toggle Bindings
The bottom section of the keybindings editor lists one entry for each effect — Drop Shadow, Inner Glow, Black & White, Gradient Map, Threshold, and Dither. These are all **unset by default**. Assign any key you like; pressing it will toggle that effect on or off exactly as if you had clicked the checkbutton in the Effects menu.
 
---
 
## Default Keyboard Shortcuts
 
| Key | Action |
|---|---|
| **Enter** | Advance to the next image |
| **Right Arrow** | Advance to the next image |
| **Left Arrow** | Go back to the previous image |
| **Space** | Pause / Resume |
| **Backspace** | Return to Main folder |
| **0** | Blank / un-blank the display |
| **C** | Hide or show the control bar |
| **F11** | Fullscreen |
| **Escape** | Exit fullscreen |
| **F1 – F8** | Switch to Bank 1–8 |
| **1 – 9** | Show trigger image |
| **Enter** *(while trigger active)* | Dismiss trigger, advance to next image |
| **A** | Style: Centered |
| **S** | Style: Crop to Window |
| **D** | Style: Stretch to Window |
| **F** | Style: Kuleshov Mode |
| **G** | Style: Two Images Classic |
| **H** | Style: Collage Mode |
| **J** | Style: Screensaver Mode |
| **K** | Style: XP Trails Mode |
| **U** | Reposition (Screensaver or XP Trails) |
| **P** | Screenshot |
| **Up Arrow** | Tempo: 2× speed |
| **Down Arrow** | Tempo: 0.5× speed |
| *(unset)* | Effect: Toggle Drop Shadow |
| *(unset)* | Effect: Toggle Inner Glow |
| *(unset)* | Effect: Toggle Black & White |
| *(unset)* | Effect: Toggle Gradient Map |
| *(unset)* | Effect: Toggle Threshold |
| *(unset)* | Effect: Toggle Dither |
 
> Style shortcuts **F**, **G**, **H**, **J**, and **K** are automatically disabled when a gradient or image background is active, or when any effect is enabled. All shortcuts are the defaults and can be changed via **Settings ▾ → Edit Keybindings…**
 
---
 
## Your Settings Are Saved
 
IMGPLYR remembers two things automatically between sessions:
 
**Last loaded sources** — every folder and Are.na channel you had loaded (Main, Trigger, and Banks) is remembered. Use **Load ▾ → Restore Last Loaded** to reload them all at once. Are.na channels are always re-fetched fresh, so you get any new images added since your last session.
 
**Custom keyboard shortcuts** — any shortcuts you change in the editor are saved and restored automatically every time you open the program.
 
If a remembered folder has been moved, renamed, or is on a disconnected drive, IMGPLYR skips it and tells you which ones it could not find.
 
### Exporting and Importing Sessions
For full portability — including background, speed, style, effects, and all sub-settings — use **Settings ▾ → Export Session Settings…** to save a `.imgplyr` file. Share it, back it up, or load it on another machine using **Settings ▾ → Import Session Settings…**
 
---
