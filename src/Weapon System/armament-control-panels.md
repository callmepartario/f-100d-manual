# Armament Control Panels

## Introduction

The armament control panels are a group of panels responsible for selecting ordinance for weapons delivery and indicating information about the weapon systems.

These consist of:

- [Gun Missile Switch](#gun-missile-switch)
- [Status Display Lights](#status-display-lights)
- [Armament Selector Panel](#armament-selector-panel)
- [Pylon Loading Control Panel](#pylon-loading-control-panel)


## Gun Missile Switch

The gun missile switch controls electrical power for the upper, lower guns and the missiles. 


![Gun Missile Switch](./img/gun_missile_switch.png)

| Position | Description
|----------|-------------
| MISSILES | The missile selection provides power to the [Missile Control Panel](./aim-9-sidewinder.md#controls) and thus the missiles. Reference [AIM-9 Sidewinder Section](aim-9-sidewinder.md) for missile operation.
| SAFE     | Removes power from the weapons system rendering it **safe**.
| UPPER    | Energises the second trigger detent and **arms** upper guns.
| ALL      | Energises the second trigger detent and **arms** upper and lower guns (all).
| LOWER    | Energises the second trigger detent and **arms** lower guns.
| POD      | Pod selection is unused on the F-100D 

**Note: Gun missile firing circuits are inhibited when weight is on the wheels.**

With the gun missile switch in any position the gun camera can be actuated by using the first trigger detent. See the [Gun Camera Section]() for details.

## Status Display Lights

The status display lights indicate various information about the current state of the weapon system.

![Status Display Lights Image](./img/status_display_lights.png)

| Light | Purpose 
|-------|---------
| TER EMPTY | This indicates (if a TER is mounted on an inner pylon) if a TER is empty of bombs
| CBU EMPTY | This indicates (if a CBU Dispenser is mounted) if the CBU dispenser is fully depleted
| Missile | This indicates if a missile is ready to be fired. The missiles are listed in firing order.

## Armament Selector Panel

This panel is responsible for:

- Selecting weapons
- Sight and Bombing Modes
- Fuzing Options
- Pylon Selection

### Controls

![Armament Selector Panel](./img/armament_controls.png)

1. [Stores Selector](#stores-selector)
2. [Mode Selector](#mode-selector)
3. [Bomb Arm Switch](#bomb-arm-switch)
4. [Station Release Selection Switches](#station-release-selection-switches)

#### Stores Selector

This selects the desired weapons to be released. When a store type is selected the pylons selected for release are determined by the [Pylon Loading Control Panel](#pylon-loading-control-panel) settings. Stores with matching types are armed for release.

#### Mode Selector

This determines the release type for air-to-ground weapons. The sight and radar are powered in any position other than OFF.

| Position | Description
|----------|--------------
| OFF      | Weapons, Sight and Radar are unpowered.
| SIGHT & RADAR | Sight and Radar are Powered and can be used with guns or missiles.
| MANUAL |  Sight and Radar are Powered. Bomb-button is energized and can send release pulses to either the [Aircraft Weapons Release System](./aircraft-weapons-release-system.md) if on, otherwise the [Basic Armament Control Circuitry](./basic-armament-control-circuitry.md).
| LABS | Sight and Radar are Powered. Bomb-button is energized and can send activation signals to the [LABS]() for the normal LABS mode (LOFT).
| LABS ALT | Sight and Radar are Powered. Bomb-button is energized and can send activation signals to the [LABS]() for the alternate LABS mode (Over-the-Shoulder).
| LADD | Sight and Radar are Powered. Bomb-button is energized and can send activation signals to the [LABS]() for the low altitude drouge delivery LABS mode.

#### Bomb Arm Switch

This controls the bomb-arming solenoids in the pylons. This only affects bomb and napalm arming.

| Setting | Fuzes | High Drag Tail Kit Deployed (if bomb has one)
|---------|-------|-------------
| SAFE    | NONE  | NO
| NOSE    | NOSE, CENTER | NO
| TAIL    | TAIL, CENTER | YES
| NOSE & TAIL | NOSE, CENTER, TAIL | YES

#### Station Release Selection Switches

These 7 switches simply break the circuit between the aircraft systems and the pylon firing or jettisoning circuitry.

When a pylon is in the NORM position the release circuitry is used. When a pylon is in the JETT position the jettison circuitry is instead used.

**Important Note: these turning these switches off do not remove them from the [Aircraft Weapons Release System Circuit](./aircraft-weapons-release-system.md#station-release-selection-switches) firing order.** Thus disabling some of these while using the AWRS can result in a hung weapon release sequence.

## Pylon Loading Control Panel

This panel stores the weapon type information mounted on each pylon as a 7 position switch such that the [Armament Selector Panel](#armament-selector-panel) can correctly select pylons by weapon type.

### Controls

![Pylon Loading Control Panel](./img/pylon_loading_panel.png)

1. Left Inboard Weapon Setting
2. Left Intermidiate Weapon Setting
3. Left Outboard Weapon Setting
4. Right Inboard Weapon Setting
5. Right Intermidiate Weapon Setting
6. Right Outboard Weapon Setting
7. Pylon Loading Control Panel Latch and Cover

The controls 1-6 all control what the wiring considers mounted to the aircraft. These are automatically set by ground grew upon re-arm or spawn.

**Setting any of these to incorrect loading may result in in-advertant release of weapons.**

There are 1-9 possible weapon mountings. These mostly match the weapon types found on the [Stores Selector](#stores-selector).

| Number | Ordinance | Notes
|--------|-----------|---------
| 1 | Empty | Nothing Loaded
| 2 | Fuel Tanks | Important for G-Limit and Jettison
| 3 | Bombs |
| 4 | Dispensers |
| 5 | Rockets |
| 6 | Special Weapons | Nuclear Ordinance
| 7 | Missiles | This is functionally the same as empty as the missiles are not control by the armament control panels
| 8 | Napalm |
| 9 | Inoperative | Functionally the same as Empty
