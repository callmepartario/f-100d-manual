# AN/AWE-1 Aircraft Weapons Release System (AWRS)

## Introduction

The AWRS provides selectable weapons release quantity and intervals. The AWRS is active any time the release quantity switch is not in the off position. When the AWRS is active any bomb pulse by the [bomb-button]() or [Low Altitude Bombing System]() will result in the AWRS being used to sequence and time bomb or rocket release.

When the AWRS is not active ([Quantity Switch in OFF](#quantity-selector-switch)) the [basic armament system circuitry]() is instead used.

## Modes

### Operation

Release modes are responsible for producing pulses which are then distributed to pylons according to the release type. The table below describes how pulses are produced and forwarded to the release type circuitry upon receiving each input signal - either from the bomb button or LABS release cue.

| Release Mode | Number of Pulses |
|--------------|------------------|
| Step         | Input signal produces only one pulse |
| Ripple       | Input signal produces a sequence of pulses with intervals specified by the [Release Interval Switch](#release-interval-switch) and [Multiplier Switch](#multiplier-switch-x10). The sequence length is the setting on the [Quantity Selector Switch]() provided the input signal is held on the entire duration of the sequence. If the input signal is released early (ie bomb-button released) the sequence immediately stops. | 

There are 3 possible release types. Each type acts on sequence pulses.

| Release Type | Pulse Result |
|--------------|--------------|
| Single | Single bomb being released from the next valid pylon in the release sequence if one exists. |
| Pairs | Pair of bombs/rockets will be released from the next valid pair of pylons in the sequence if one exists. |
| Salvo | Every valid/selected pylon will release a bomb/rocket if the pylon is not empty.

### Examples

To assist in understanding the AWRS, below a few examples are shown. Each example assumes there are enough bombs on the plane in the correct configuration to drop the correct number of bombs/rockets.

| Release Mode | Release Type | Quantity Selector Switch | Interval (ms) |  Multiplier Switch  | Result |
|--------------|--------------|--------------------------|---------------|---------------------|--------|
| Ripple       | Single       | 4                        | 60            | x1                  | 4 bombs will be dropped with an interval of 60 ms between them. |
| Ripple       | Single       | 6                        | 100           | x10                 | 6 bombs will be dropped with an interval of 1000 ms (due to x10 switch) between them |
| Ripple       | Pairs        | 3                        | 150           | x1                  | 3 pairs of bombs will be dropped (total 6) with an interval of 150 ms between each pair. |
| Ripple       | Salvo        | 3                        | 45 ms         | x1                  | Assuming the plane is armed with a 1,1,3,3,1,1 MK-82 on each pylon. The first salvo will drop 6 bombs, leaving 0,0,2,2,0,0 on the aircraft. 45 ms later 2 more bombs will drop leaving 0,0,1,1,0,0 and again 45 ms later the remaining 2 bombs will drop. Resulting in a total of 10 bombs being dropped. |

## Station Priority and Sequencing

Bombs/rockets will drop in order of priority alternating sides if two valid pylons of equal priority exist. The further out from the centre the higher the priority the pylon has. This means the outer wing pylons have the highest priority and the inner wing pylons the lowest. The AWRS does not consider any pylons which are not active: either because they do not have the correct weapon type or because the pylon is disabled. Once a pylon is empty it is no longer considered valid.

Rockets pods cannot send an empty signal so once the outer rocket pods are empty the AWRS will not automatically step to the inner rocket pods as it still assumes they are valid. To use the inner rocket pods either Ripple/Step Salvo can be used or the outer rocket pods can be manually disabled using the [Station Select Switches](./armament-control-panels.md#station-select-switches).

### Priority

| Left Outer  | Left Middle | Left Inner | Right Inner | Right Middle | Right Outer |
|-------------|-------------|------------|-------------|--------------|-------------|
|  1          | 3           | 5          | 6           | 4            | 2           |

## Controls

### Quantity Selector Switch

With the Quantity Selector Switch in the OFF position electrical power is removed from the AWRS system making it inactive. With the Quantity Selector Switch set to any numbered position the AWRS is active and energized.

The selected number provides the AWRS with the quantity of release pulses in ripple modes: Ripple - Single, Ripple - Pairs, and Ripple - Salvo. See [operation](#operation).

### Release Interval Switch

The release interval switch selects the time interval in miliseconds between subsequent pulses from the AWRS. The release interval can be multiplied by ten using the [Multiplier Switch](#multiplier-switch-x10)

### Multiplier Switch (x10)

The multiplier switch multiplies the [release interval](#release-interval-switch) by ten with x10 set and x1 otherwise.
