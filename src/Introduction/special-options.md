# Special Options
Various special options have been added for user quality of life and customization. The following parts below will explain each special option in depth. 

These options are located in the xx of DCS World with the DCS: F-100D Super Sabre Selected from the left side module tray.


## Gameplay

![special options image](./img/special_options-1.png)

### Cockpit Camera Shake
The cockpit camera shake can be adjusted on this slider as an overall multiplier to global cockpit camera shake.

### Pylon Control Armament Assistance

This decides how the [pylon loading control panel](../Weapon_System/armament-control-panels.md#pylon-loading-control-panel) is setup.

| Setting  | Pylon Loading Assistance
|----------|--------------------------
| OFF      | None - up to pilot
| ON SPAWN | Set automatically on spawn. After rearming it is up to the pilot to set
| FULL     | Set automatically on spawn and after rearming complete.

### Autostart Mode
FULL will opt out of any auto start assistance for a complete cold-and-dark start. ENGINE ONLY sets all other switches, knobs, and settings for start; thus, the engine is the only required item for a complete start.

## External Customization Options
### Victory Kill Markings
Aircraft victory kill markings on the side of the nose portion of the fuselage account (currently) for single player air-to-air and air-to-ground kills. 

Enable Kill/Victory Markings will turn off this feature if unchecked.

## Cockpit Configuration Options

### Seat Position
Adjusting this slide will move the default seat height (and viewpoint). 0 is lowered, while 100 is raised.

### Air Start Gun Selector
This option will adjust the default setting of the Gun Selector Knob. Options are SAFE, GUNS UPPER, GUNS LOWER, GUNS ALL, or MISSILE.

### Gun Camera Selector
To set the default position of the gun camera selector knob, change to Off, GUN CAM ONLY, STRIKE CAM ONLY, OR BOTH. 

## Cockpit Customization Options
In order to enable dynamic instrument panel gauge positions, check Enable Custom Instrument Panel. You can then either randomize between known historical layouts, or enter your own custom panel ID. Visit [www.GrinnelliDesigns.com/dash-creator](https://grinnellidesigns.com/dash-creator/) to create a unique layout ID and paste it in the Custom Instrument Panel ID text field.

## Gun Camera Settings

![special options gun](./img/special_options-2.png)

### Disable Gun Camera Recording
Turning the option to off will disable all gun recording and not generate video files.

### Gun Camera Effects
To adjust the default gun camera effects, select between off (to remove entirely), or vintage.

### Overrun Time
This slider will adjust how long the gun cameras will continue to record after trigger release. Adjust between 0 and 3 seconds.

### Start Delay Adjust
This slider will adjust the time between trigger release and the start of the preset run time. Adjust between 4 to 30 seconds.

### Preset Run Time
Adjusts the run time of the gun camera after start delay. Adjust from 2 to 30 seconds.

!!! note
    Total Camera run time after the release of the trigger is the total of both time interval settings (6 to 63 seconds) including the preset overrun time of 0 to 3 seconds.

!!! warning
    Cameras will save AVI recordings in "%userprofile%/Saved Games/DCS F-100D" in the respective folder for the camera.

## Strike Camera Settings

![special options strike](./img/special_options-3.png)

### Disable Strike Camera Recording
Turning the option to off will disable all gun recording and not generate video files.

### Strike Camera Effects
To adjust the default Strike camera effects, select between off (to remove entirely), or vintage.

### Overrun Time
This slider will adjust how long the gun cameras will continue to record after pickle release. Adjust between 0 and 3 seconds.

### Forward Camera Elevation
The forward camera elevation can be adjusted from 0 degrees to 20 degrees down.


### Forward Camera Focal Length
The forward camera uses a variable focal length lens, adjustable from 20mm (wide) to 80mm (narrow).


### Rear Camera Start Delay
The delay of the start of the rear camera recording after pickle press.

### Rear Camera Elevation Mode
The rear camera elevation can be adjusted from 0-25 degrees for the upper range, or 45-60 degrees for the lower range.

### Rear Camera Upper Elevation
Change the camera elevation from 0-25 degrees down.

### Rear Camera Lower Elevation
Change the camera elevation from 45-60 degrees down.
### Rear Camera Focal Length
The rear camera uses a variable focal length lens, adjustable from 17mm (wide) to 68mm (narrow).
### Rear Camera Speed
This setting will change the playback rate of the output footage. 100% is real-time.

!!! warning
    Lower playback rates increase RAM usage of rear camera.


