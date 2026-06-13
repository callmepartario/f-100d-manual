# AIM-9 Sidewinder

## Introduction

The AIM-9 sidewinder is a short range infrared guided missile introduced in 1956. It is the primary air-to-air weapon for the F-100D.

The Sidewinder is a passive infrared guided missile. The missile is aimed using the [A-4 Gunsight](./a-4-gunsight.md#a-4-gunsight) with the sight [mechanically or electrically caged](./a-4-gunsight.md#mechanical-cage-lever).

The missile generates a tone based on received infrared radiation into its seeker, which is transmitted to the pilot headphones. A low growl indicates little to no infrared radiation detected, and a higher-and-louder growl indicates a heat source, indicated a possible detected target. The growl only indicates the ability for the seeker to track, but not anything about range, or whether the missile can maneuver to the target.

The F-100D can carry two Sidewinders on a Type IX launcher on each of the inboard pylons, for a total of four missiles.

### Sidewinder Types

The F-100D historically carried 3 different variants of the AIM-9 Sidewinder, although some later variants are backwards compatible: AIM-9L and AIM-9M Sidewinders are compatible with minor rail modifications that were made to other aircraft in the 1990s.

#### AIM-9B

Introduced in 1957 this is the first sidewinder to be put into service. It saw significant use during the Vietnam War.

#### AIM-9E

Introduced in 1969, this variant boasted peltier cooled seeker for better thermal sensitivity, increased seeker track rate, and improved maneuverability. The seeker gimbal-limit was improved from 25° to 40°, making it significantly more effective against maneuvering targets.

Additionally, the max launch G was increased from 2–7.33 G, allowing launches during maneuvering, overcoming a key shortcoming that plagued the AIM-9B.

#### AIM-9J

Introduced in 1972, the J contniued to improve the seeker max track rate, and a time between launch and missile maneuvering reduced from 0.5 to 0.3 seconds.

## Controls

This panel is responsible for:

- Managing the firing sidewinder order
- Changing sidewinder volume
- Jettisoning sidewinders
- Making the sidewinders safe when not in use.

![Missile Control](./img/missile_control_panel.png)

1. [Missile Volume Control](#missile-volume-control)
2. [Station Bypass](#station-bypass)
3. [Missile Master](#missile-master)
4. [Safe Launch](#safe-launch)

### Missile Volume Control

This adjust the volume of the Sidewinder in the headset.

### Station Bypass

In the event of a defective Sidewinder the store can be stepped to the next Sidewinder by using the station bypass switch.

### Missile Master

This three position switch is normally in the standby position with it spring loaded for the reset position.

| Position             | Description
|----------------------|-------------
| Reset (sprungloaded) | Resets the firing order of the sidewinders moving the firing order back to the first Sidewinder (left pylon right sub-pylon).
| Standby              | Maintains the Sidewinder in a warmed up state while keeping the missile safe. The audio can still be heard in this position.
| Ready                | Arms the Sidewinder for launch bringing it to the ready state.

### Safe Launch (Jettison)

Pressing and holding this button starts the Sidewinder [jettison](#Jettison) process, firing all Sidewinders (without fuzing or guidance) in their [firing](#Firing) order with a 0.5 second delay between each.

## Operation

### Setup

<!---
TODO Gun-Missile Switch
-->

The [Gun-Missile Switch](./guns.md#gun-missile-switch) in the MISSILE position provides warmup and gyro power to the missiles. The [Missile Master Switch](#missile-master) sets the ready state of the missiles. In STBY mode, the Sidewinder is kept warmed up and ready. In this position missile audio can be heard but the firing circuits are not armed.

Sidewinder volume is adjusted using the Missile Control [Volume Control](#missile-volume-control).

### Firing

To arm the missiles, confirm the [Gun-Missile Switch](./guns.md#gun-missile-switch) is in the MISSILE position, and set the [Missile Master Switch](#missile-master) to the READY position. A Sidewinder tone should be heard, and the [status display lights](./armament-control-panels.md#status-display-lights) should indicate a Sidewinder is ready for firing.

Sidewinders are fired in the following order, and correspond to [status display lights](./armament-control-panels.md#status-display-lights).

![Sidewinder Firing Order](./img/sidewinder_firing_order.png)

!!! warning
    Releasing the trigger before the launch sequence is complete will cause the missile to be **trashed**. Once the trigger is pressed, an irreversible process begins: the seeker is uncaged and the gas generator is fired, expending the missile's usability. Bypass unusable missiles using the [station bypass](#station-bypass) switch.
