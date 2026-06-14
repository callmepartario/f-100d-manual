# Gun Camera

## Introduction

The KB-3 gun camera on the [A-4 gunsight](../Weapon_System/a-4-gunsight.md), is an electrically-driven, magazine-type, 16 mm motion picture camera that photographs the reticle and target simultaneously.

## Enable Gun Camera Recording

Enable recording in the F-100D [Special Options](../Introduction/special-options.md) menu.

Gun camera recordings are generated when the trigger's first detent is pressed. Recordings are saved in `%userprofile%/Saved Games/DCS F-100D` at the end of the mission.

!!! note
    The gun camera and [strike cameras](../Strike%20Camera/strike_camera.md) only record when the view is in the cockpit.

## Controls

![Gun Camera](./img/strike_cam_controls.png)

1. [Camera Selection Dial](#camera-selection-dial)
2. [Camera Timer](#camera-timer)

### Camera Selection Dial

On a real F-100D, this dial controlled for adjusting the camera under bright, hazy, or dull lighting conditions. In this simulated F-100D, it selects the cameras enabled for recording.

| Selection  | Description |
|------------|-------------|
| **STRIKE** | Enables [strike camera](../Strike%20Camera/strike_camera.md) recordings. |
| **GUN**    | Enables gun camera recordings. |
| **BOTH**   | Enables [strike camera](../Strike%20Camera/strike_camera.md) and gun camera recordings. |

### Camera Timer

During missile firing, two adjustable timer control recording after the trigger is released. 

| Interval           | Length (seconds) | Description |
|--------------------|------------------|-------------|
| **START DELAY**    | 4–30             | Begins when the trigger is released. Set it using the large timer knob. |
| **PRESET RUNTIME** | 2–30             | Begins after the start delay ends. Set it using the the small timer knob. |
| **OVERRUN**        | 0–3              | Begins after the runtime. |

!!!note
    You can set default intervals in the F-100D [Special Options](../Introduction/special-options.md) menu.

<!--### Ground Crew Operation TODO—How to change film, does film refresh when rearming? -->
