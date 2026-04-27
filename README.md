<img src="https://raw.githubusercontent.com/mhf93/imgplyr/refs/heads/main/imgplyr%20logo%20gif.gif">


# IMGPLYR
 Image Slideshow Performance Software
 
**Version 1.5**  
© 2026 John Zobele | A zobele.co Project
 
---
 
## What is IMGPLYR?
 
IMGPLYR is an image slideshow player built for live use. Load a folder of images and play them back automatically on a timer, advance them manually at your own pace, switch between different image sets on the fly, and display them in a variety of visual styles — all without stopping the show.
 
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
 
## The Control Bar
 
All controls live in the bar at the top of the window. From left to right:
 
**Load ▾** · **Start/Pause** · **Background ▾** · **Speed ▾** · **Scale ▾** · **Styles ▾** · **Settings ▾** 
 
The **status bar** on the right shows live information — which image you are on, which bank or folder is active, speed confirmations, and other feedback.
 
---
 
## Loading Images
  
### Load Main
Your primary image folder. This is what plays by default.
 
### Load Trigger
A special folder for images you want to display on demand using the number keys. Name the files `1.png`, `2.jpg`, `3.png`, and so on up to `9`. When you press the corresponding number key, that image is displayed immediately and held until you advance the queue.
 
### Load Bank 1–8
Eight extra image folders, each assigned to a function key (F1–F8). You can pre-load all eight before you begin, then switch between them live during playback by pressing the matching key. Switching banks does not interrupt the current image — the change takes effect on the next advance.
 
### Restore Last Session
Reloads every folder you had open the last time you closed the program. Folders that have been moved, renamed, or are on a disconnected drive are skipped and listed in a summary. Everything else loads exactly as you left it.
 
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
Press **Backspace** to switch back to the Main folder immediately and jump to the next image in the main queue. Useful if you have been browsing banks and want to return to the primary slideshow.
 
### Triggering Images on Demand
Press **1 through 9** to show a specific image from your trigger folder. The image is held on screen — the slideshow keeps timing in the background but does not show anything new until you dismiss the trigger.
 
Press **Enter** to dismiss the trigger. The slideshow then advances to the **next** image in the queue.
 
### Blanking the Screen
Press **0** to hide whatever is on screen without pausing the timer. The queue continues advancing silently. Press any advance key (Enter, Right Arrow) to un-blank — the next image in the queue is shown, not the one that was there before blanking.
 
In **Collage Mode**, blanking clears the entire canvas. Un-blanking starts fresh from the current position in the queue.
 
---
 
## Switching Banks Live
 
Once you have loaded banks using **Load ▾ → Load Bank 1–8**, press **F1 through F8** at any time to switch the active image pool to that bank. The current image stays on screen — the new bank takes effect on the next advance.
 
Press **Backspace** at any time to return to the Main folder.
 
If the Pop-Out Controls window is open, bank buttons (labelled F1, F2, etc.) appear in the navigation row automatically for each loaded bank.
 
---
 
## Background
 
The **Background ▾** dropdown controls what appears behind your images.
 
### Solid Color
Six preset options plus **Custom…** which opens a colour picker so you can choose any colour.
 
### Gradient
Select **Edit Gradient…** to open the gradient editor.
 
- The row of colour swatches represents each colour stop in the gradient. Click any swatch to change it.
- Click **+ Add Stop** to add more colours. Click **− Remove last** to take one away. You need at least two stops.
- Choose a direction: **Left → Right**, **Top → Bottom**, or **Diagonal**.
- The preview at the bottom updates as you make changes.
- Click **Apply** to set the gradient as your background. Click **Cancel** to discard.

> Gradient backgrounds are not available when Kuleshov Mode, Two Images Classic, or Collage Mode is selected. Those style options will be greyed out in the Styles menu while a gradient is active.
 
### Image Background
Click **Load Image…** to pick any image file to use as your background. Then choose how it fills the window:
 
- **Fit: Stretch** — stretches the image to exactly fill the window. May distort proportions.
- **Fit: Crop** — fills the window while keeping the image proportions, cropping the edges.
- **Fit: Tile** — repeats the image at its original size to cover the window.
Click **Clear Image** to remove the background image and return to a solid colour.
 
> Image backgrounds are not available when Kuleshov Mode, Two Images Classic, or Collage Mode is selected.
 
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
 
---
 
## Scale
 
Click **Scale ▾** to open a small floating panel with a vertical slider.
 
- Drag the slider **up** to make images larger, **down** to make them smaller.
- The percentage is shown above the slider and updates live.
- Quick buttons set the scale to **50%**, **100%**, or **150%** instantly.
- Click **Close** to dismiss the panel. The panel can stay open while you continue using the slideshow.
When **Kuleshov Mode** or **Two Images Classic** is active, the Scale panel also shows a **Pane Gap** slider that controls the width of the space between the two image panels.
 
---
 
## Styles

 
### Centered (default)
The image sits in the middle of the screen with equal space on all sides. The Scale slider controls how large the image appears within that space.
 
### Crop to Window
The image fills the entire screen edge to edge. The proportions are preserved — the sides or top and bottom are cropped as needed to fill the frame. There are no borders or gaps.
 
### Stretch to Window
The image is stretched to fill the exact dimensions of the window. Proportions are not preserved. Works well for abstract images or textures where distortion does not matter.
 
### Collage Mode
Images accumulate on screen at random positions, layered on top of each other. Up to 50 images can be visible at once — once that limit is reached, the oldest image fades off as each new one arrives.

 
> Not available when a gradient or image background is active.
 
### Kuleshov Mode
The screen is split into two side-by-side panels with a gap between them. Each advance updates **one panel at a time**, alternating left and right. The other panel keeps its previous image.
 
The gap width is adjustable using the **Pane Gap** slider in the Scale panel.
 
> Not available when a gradient or image background is active.
 
### Two Images Classic
The same two-panel layout as Kuleshov Mode, but **both panels update at the same time**. Each advance replaces both images simultaneously with the next two from the queue.
 
> Not available when a gradient or image background is active.
 
---
 
## Settings
 
The **Settings ▾** dropdown holds display and control options.
 
### Fullscreen (F11)
Puts the window in fullscreen. 
Press **Escape** to exit fullscreen.
 
### Hide Controls (C)
Hides the control bar so the image fills the entire window. Press **C** again (or use the same option in the Pop-out control menu) to bring it back. All keyboard shortcuts continue to work while the bar is hidden.
 
### Order: Random / Order: Alphabetical
Controls the order images play in.
 
- **Random** (default) — shuffles the folder so every image is shown once in a random order before anything repeats.
- **Alphabetical** — plays images in filename order, A to Z. Switching between these during playback takes effect immediately without restarting.
### Pop Out Controls
Opens the control bar as a separate floating window. The main bar is hidden when the pop-out is open. The pop-out can be dragged to any position or monitor.
 
### Edit Keybindings…
Opens the keyboard shortcut editor. See [Customising Keyboard Shortcuts](#customising-keyboard-shortcuts).
 
### Help / Shortcuts
Opens a quick reference of all keyboard shortcuts inside the app.
 
---
 
## Pop-Out Controls
 
**Settings ▾ → Pop Out Controls** moves the control bar into a small floating window that can be positioned anywhere — including a second monitor while the main window is fullscreen on your display.
 
The pop-out has two rows:
 
**Top row:** Load ▾ · Start/Pause · Background ▾ · Speed ▾ · Scale ▾ · Styles ▾ · Settings ▾
 
**Bottom row:** ◄ Back · Next ► · ↩ Main · then one button per loaded bank (F1, F2, etc.)
 
Bank buttons appear automatically as you load banks and disappear if no banks are assigned. The Start/Pause button and the status strip at the bottom keep in sync with the main window.
 
All keyboard shortcuts work when the pop-out window is the one in focus.
 
To close the pop-out and restore the main bar, click the × on the pop-out window, or go to **Settings ▾ → Dock Controls** inside the pop-out.
 
---
 
## Customising Keyboard Shortcuts
 
**Settings ▾ → Edit Keybindings…** opens a table of every action and its current shortcut.
 
**To change a shortcut:**
1. Click the text box next to the action you want to rebind. It turns yellow.
2. Press the key you want to use. The box turns green and shows the new key.
3. Click **Save** to apply all changes.
**Revert to Defaults** resets every shortcut back to its original assignment in the editor. You still need to click **Save** for the changes to take effect.
 
**Cancel** closes the editor without saving any changes.
 
Your custom shortcuts are saved automatically and will still be there the next time you open the program.
 
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
| **Enter** *(while trigger is active)* | Dismiss trigger, advance to next image |
| **A** | Switch to Centered style |
| **S** | Switch to Crop to Window style |
| **D** | Switch to Stretch to Window style |
| **F** | Switch to Kuleshov Mode |
| **G** | Switch to Two Images Classic |
| **H** | Switch to Collage Mode |
 
> The **F**, **G**, and **H** shortcuts are automatically disabled when a gradient or image background is active.
 
---
 
## Supported Image Formats
 
IMGPLYR can display the following image types:
 
PNG · JPG / JPEG · GIF · BMP · PPM · PGM · WEBP
 
---
 

 
