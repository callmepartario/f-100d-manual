# AIM-9 Sidewinder

## Introduction

The AIM-9 sidewinder is a short range infrared guided missile, introduced in 1956. It is the primary air-to-air weapon for the F-100D.

The F-100D can carry two Sidewinder Missiles on a Type IX launcher on each of the inboard pylons, for a total of four Sidewinders.

The sidewinder is a passive infrared guided missile. The missile is aimed using the [A-4 Gunsight](./a-4-gunsight.md#a-4-gunsight) with the sight [mechanically or electrically caged](./a-4-gunsight.md#mechanical-cage-lever).

The missile generates a tone based on received infrared radiation into its seeker. This tone is transmitted to the pilot headphones. A low growl indicates little to none infrared radiation detected and a high/louder growl indicates a heat source and a possible detected target. The growl only indicates the ability for the seeker to track and does not indicate anything about range or whether the missile is able to maneuver to the target.

### Sidewinder Types

The F-100D can carry 3 different variants of the AIM-9 sidewinder listed below.

#### AIM-9B

Introduced in 1957 this is the first sidewinder to be put into service. Seeing significant action in Vietnam.

#### AIM-9E

This variant was introduced in 1969. It had a small increase in maneuverability and seeker track rate. The seeker gimbal-limit was improved from 25 degrees to 40 degrees making it much more effective against maneuvering targets.

This variant also used a peltier cooled seeker allowing for better thermal sensitivity.

Importantly the max launch G was increased from 2 G to 7.33 G to allow launching while maneuvering something which plagued the early use of the AIM-9B.

#### AIM-9J

This variant was introduced in 1972 and improved on the AIM-9E by increasing the seeker max track rate again. The time between launch and missile maneuver was reduced to 0.3 seconds from 0.5 in previous versions.

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

This adjust the volume of the sidewinder in the headset.

### Station Bypass

In the event of a defective sidewinder the store can be stepped to the next sidewinder by using the station bypass switch.

### Missile Master

This three position switch is normally in the standby position with it spring loaded for the reset position.

Actuating reset will reset the firing order of the sidewinders moving the firing order back to the first sidewinder (left pylon right sub-pylon).

Standby will maintain the sidewinder in a warmed up state while keeping the missile safe. The audio can still be heard in this position.

Ready will arm the sidewinder for launch bringing it to the ready state.

### Safe Launch

Pressing this switch will fire all sidewinders safe (no fuzing or guidance) in their firing order with a 0.5 second delay.

## Operation

### Setup

<!---
TODO Gun-Missile Switch
-->

The [Gun-Missile Switch](./armament-control-panels.md#gun-missile-switch) in the Missile position provides warmup and gyro power to the missiles. The [Missile Master Switch](#missile-master) sets the ready state of the missiles. In the STBY the sidewinder is kept warmed up and ready. In this position missile audio can be heard but the firing circuits are not armed.

Sidewinder volume can be adjusted using the Missile Control [Volume Control](#missile-volume-control).

### Firing

To arm the missiles check the [Gun-Missile Switch](./armament-control-panels.md#gun-missile-switch) is in the Missile position and put the [Missile Master Switch](#missile-master) into the READY position.

A Sidewinder tone should be heard and the [status display lights](./armament-control-panels.md#status-display-lights) should indicate a Sidewinder ready to be fired.

Below is the order in which sidewinders are fired, this also corresponds to the light displayed on the [status display lights](./armament-control-panels.md#status-display-lights).

![Sidewinder Firing Order](./img/sidewinder_firing_order.png)

### Jettison

Jettison of sidewinders is not possible the conventional way due to them being mounted on a rail. Thus to be jettisoned they must be fired un-armed without guidance. To do this simply press and hold the [Safe Launch](#safe-launch) for the duration of the jettison process. This will cause the sidewinders to launch one by one with 0.5 second intervals until all the sidewinders are safely jettisoned.