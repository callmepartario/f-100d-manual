# AN/AWE-1 Aircraft Weapons Release System (AWRS)

## Introduction

The AWRS provides selectable weapons release quantity and intervals. The AWRS is active any time the release quantity switch is not in the off position. When the AWRS is active any bomb pulse by the [bomb-button]() or [Low Altitude Bombing System]() will result in the AWRS being used to sequence bomb or rocket release.

When the AWRS is not active the [basic armament system circuitry]() is instead used.

## Modes

There are two possible release modes: Ripple/Step. Each release mode is responsible for producing pulses which are then distributed according to the release type. The table below describes how pulses are produced and forwarded to the release type upon receiving each input signal - either from the bomb button or LABS release cue.

| Release Mode | Number of Pulses |
|--------------|------------------|
| Step         | Input signal produces only one pulse |
| Ripple       | Input signal produces a sequence of pulses with intervals specified by the [Release Interval Switch]() and [Multiplier Switch](). The sequence length is the setting on the [Quantity Selector Switch]() provided the input signal is held on the entire duration of the sequence. If the input signal is released early (ie bomb-button released) the sequence immediately stops. | 

There are 3 possible release types. Each type acts on sequence pulses.

| Release Type | Pulses |
|--------------|--------|
| Single | Each pulse will result in a single bomb being released from the next valid pylon in the release sequence if one exists. |
| Pairs | Each pulse will result in a pair bombs/rockets being released from the next valid pair of pylons in the sequence if one exists. |
| Salvo | Each pulse will result in every valid/selected pylon releasing a bomb/rocket if the pylon is not empty. |

## Controls

### AWRS Quantity Selector Switch

With the Quantity Selector Switch in the OFF position electrical power is removed from the AWRS system making it inactive. With the Quantity Selector Switch set to any numbered position the AWRS is active and energized.

The selected number provides the AWRS with the quantity of release pulses in ripple modes: Ripple - Single, Ripple - Pairs, and Ripple - Salvo.