# Weapon Release Circuitry

## Basic Armament Control Circuitry

The basic armament control circuitry is used to send release signals to the pylons to release rockets, bombs and dispenser. The basic armament system circuitry is used when the [Aircraft Weapons Release System](#anawe-1-aircraft-weapons-release-system-awrs) is **off**.

The basic armament control circuitry can receive bomb pulses from either the [manual delivery mode](./armament-control-panels.md#mode-selector), [automatic sight release](a-4-gunsight.md#bomb-air-to-ground-automatic) release cue, or [Low Altitude Bombing System](./low-altitude-bombing-system.md) release cue. When a bomb pulse is received like the [Aircraft Weapons Release System](./aircraft-weapons-release-system.md) it is up to the [weapons selection circuitry](./armament-control-panels.md#weapon-selection-circuitry) forward the pulses to the correct pylons to release ordinance.

All stations which have their respective [Station Release Selection Switch](./armament-control-panels.md) armed will receive the forwarded bomb pulse. Any stations which instead have jettison selected will instead convert that bomb pulse to a jettison signal jettisoning the ordinance from the pylon (if it can be jettisoned).

## AN/AWE-1 Aircraft Weapons Release System (AWRS)

### Introduction

The AWRS provides selectable weapons release quantity and intervals. The AWRS is active any time the release quantity switch is not in the off position. When the AWRS is active any bomb pulse by the [bomb-button]() or [Low Altitude Bombing System](./low-altitude-bombing-system.md) will result in the AWRS being used to sequence and time bomb or rocket release.

When the AWRS is not active ([Quantity Switch in OFF](#quantity-selector-switch)) the [basic armament system circuitry](#basic-armament-control-circuitry) is instead used.

### Station Release Selection Switches

**For the Aircraft Weapons Release System to function correctly all [Station Release Selection Switches](./armament-control-panels.md#station-release-selection-switches) for the desired weapon type should be moved into either NORM or JETT (depending if armed release or jettison is required).** Failure to do so may result in the Aircraft Weapons Release System getting stuck on a pylon where the ordinance is unable to be released due to the Station Release Selection Switch disconnecting the pylon circuitry.

### Controls

![Aircraft Weapons Release System Panel](./img/awrs_panel.png)

1. [Quantity Selector Switch](#quantity-selector-switch)
2. Power Indicator Light
3. [Release Interval Switch](#release-interval-switch)
4. [Multiplier Switch (x10)](#multiplier-switch-x10)
5. [Mode Select Switch](#modes)

#### Quantity Selector Switch

With the Quantity Selector Switch in the OFF position electrical power is removed from the AWRS system making it inactive. With the Quantity Selector Switch set to any numbered position the AWRS is active and energized.

The selected number provides the AWRS with the quantity of release pulses in ripple modes: Ripple - Single, Ripple - Pairs, and Ripple - Salvo. See [operation](#operation).

#### Release Interval Switch

The release interval switch selects the time interval in milliseconds between subsequent pulses from the AWRS. The release interval can be multiplied by ten using the [Multiplier Switch](#multiplier-switch-x10)

#### Multiplier Switch (x10)

The multiplier switch multiplies the [release interval](#release-interval-switch) by ten with x10 set and x1 otherwise.

### Modes

#### Operation

Release modes are responsible for producing pulses which are then distributed to pylons according to the release type. The table below describes how pulses are produced and forwarded to the release type circuitry upon receiving each input signal - either from the [manual delivery mode]() or [Low Altitude Bombing System](./low-altitude-bombing-system.md) release cue.

| Release Mode | Number of Pulses |
|--------------|------------------|
| Step         | Input signal produces only one pulse |
| Ripple       | Input signal produces a sequence of pulses with intervals specified by the [Release Interval Switch](#release-interval-switch) and [Multiplier Switch](#multiplier-switch-x10). The sequence length is the setting on the [Quantity Selector Switch](#quantity-selector-switch) provided the input signal is held on the entire duration of the sequence. If the input signal is released early (ie bomb-button released) the sequence immediately stops. |

There are 3 possible release types. Each type acts on sequence pulses.

| Release Type | Pulse Result |
|--------------|--------------|
| Single | Single bomb being released from the next valid pylon in the release sequence if one exists. |
| Pairs | Pair of bombs/rockets will be released from the next valid pair of pylons in the sequence if one exists. |
| Salvo | Every valid/selected pylon will release a bomb/rocket if the pylon is not empty.

#### Examples

To assist in understanding the AWRS, below a few examples are shown. Each example assumes there are enough bombs on the plane in the correct configuration to drop the correct number of bombs/rockets.

| Release Mode | Release Type | Quantity Selector Switch | Interval (ms) |  Multiplier Switch  | Result |
|--------------|--------------|--------------------------|---------------|---------------------|--------|
| Ripple       | Single       | 4                        | 60            | x1                  | 4 bombs will be dropped with an interval of 60 ms between them. |
| Ripple       | Single       | 6                        | 100           | x10                 | 6 bombs will be dropped with an interval of 1000 ms (due to x10 switch) between them |
| Ripple       | Pairs        | 3                        | 150           | x1                  | 3 pairs of bombs will be dropped (total 6) with an interval of 150 ms between each pair. |
| Ripple       | Salvo        | 3                        | 45 ms         | x1                  | Assuming the plane is armed with a 1,1,3,3,1,1 MK-82 on each pylon. The first salvo will drop 6 bombs, leaving 0,0,2,2,0,0 on the aircraft. 45 ms later 2 more bombs will drop leaving 0,0,1,1,0,0 and again 45 ms later the remaining 2 bombs will drop. Resulting in a total of 10 bombs being dropped. |

### Station Priority and Sequencing

Bombs/rockets will drop in order of priority alternating sides if two valid pylons of equal priority exist. The further out from the centre the higher the priority the pylon has. This means the outer wing pylons have the highest priority and the inner wing pylons the lowest. The AWRS does not consider any pylons which are not active: either because they do not have the correct weapon type. Once a pylon is empty it is no longer considered valid.

!!! note
    **Rockets/dispenser pods cannot send an empty signal** so once the outer rocket/dispenser pods are empty the AWRS will not automatically step to the inner rocket/dispenser pods as it still assumes they are valid. To use the inner rocket/dispenser pods either Ripple/Step Salvo can be used instead.

!!! warning
    **[Station Release Selection Switches](#station-release-selection-switches) do not effect the Aircraft Weapons Release System pylon validity. These switches simply break the circuit between the Aircraft Weapons Release System and the pylon circuitry. This has the unintended side effect of causing the Aircraft Weapons Release System to get stuck if any of these pylons are set to OFF.**

Below is the priority of each station with a lower number indicating higher priority.

| Left Outer  | Left Middle | Left Inner | Right Inner | Right Middle | Right Outer |
|-------------|-------------|------------|-------------|--------------|-------------|
|  1          | 3           | 5          | 6           | 4            | 2           |

