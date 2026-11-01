# BetterManual HDR

Fork of [obs1dium/BetterManual](https://github.com/obs1dium/BetterManual) focused on HDR exposure bracketing, tested on the **A5000** (ILCE-5000, firmware 1.10). It installs as a separate app (`com.obsidium.bettermanual.hdr`), so it can coexist with the original.

Changes:

* **Armed bracketing**: configure step (EV), picture count and delay once; from then on every shutter press runs the whole series. Settings survive app restarts. The bracket icon turns yellow while armed; select it and press enter to disarm.
* **Aperture priority bracketing**: the camera meters on each shutter press, no need to set a manual exposure first.
* **Native bracket**: 3-picture series with 0.3/0.7/1/2/3 EV steps use the camera's own continuous bracket drive mode (much faster). Other series fall back to shifting the shutter speed from the app.
* **Countdown** configurable from 2 to 10 seconds.
* **Left/right keys** select the previous/next parameter on cameras without touch screen.
* Fixed even EV steps (e.g. 2.0EV) producing 0/+2/+6 instead of 0/-2/+2.

ISO must be set to manual for bracketing. Outside bulb mode the camera caps exposures at 30s, which limits the brightest picture in dark scenes.

The original README follows.

---

# Note: This app  is not actively maintained anymore.

# BetterManual

This app is intended to ease shooting in manual and aperture priority mode with (legacy) prime lenses on the A5100 camera. It uses the [OpenMemories Framework](https://github.com/ma1co/OpenMemories-Framework).
**While the app may work on other cameras, it was written specifically for use with the A5100.**
**Do not try to install it on cameras without a dedicated manual mode!**

## Installation ##

Use [Sony-PMCA-RE](https://github.com/ma1co/Sony-PMCA-RE) or install through [sony-pmca.appspot.com](https://sony-pmca.appspot.com/apps).

## Usage and features ##

Features are accessed using either the touch screen or the control wheel.

### Shooting modes ###

Touch the mode indicator on the top left to toggle between manual and aperture priority mode.
The icon directly below it allows you to cycle between single shot, low speed and high speed burst modes.

### Shooting parameters ###

The following parameters can be configured directly: Shutter speed, aperture, ISO, exposure compensation.
Using the control wheel: Press the down button to select the parameter you'd like to change, then turn the wheel to change its value. Additionally, the enter button allows you to toggle between manual and automatic ISO and set a minimum shutter speed in aperture priority mode.
Using the touch screen: Swipe left/right or up/down to change parameters. Tap once to toggle between manual and automatic ISO or set the minimum shutter speed.

### Interface ###

Press the up button to cycle through display modes. This will toggle the histogram, metering display and rule of 3rds grid lines.

### Focus magnification ###

Use the zoom lever to activate focus magnification and zoom in or out. Half-pressing the shutter button ends focus magnification. You can change the position of the preview rectangle by either using the control wheel or swiping the touch screen. The enter button centers the preview rectangle.

### Other features ###

The app also includes simple timelapse and exposure bracketing modes. Touch the icon on the left side and follow the on-screen instructions.

Long exposure noise reduction is disabled (normally forced in single shot mode for exposures >= 1" and in bulb mode on the A5100).

Exit the app using the help/trash button.

The app remembers the configured settings across multiple runs.
