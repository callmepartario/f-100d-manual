# Direction Gyro and Compass

<!-- 
This entire section needs to be reviewed as far as order of sections, titles of sections and the numbers on the image.
Im torn as far as the layout of the numbers marked on the controls image. either to do it left to right in order or number
the elements on said control in the order of logical use in practice. i.e. power then function then adjustments ect ect.
-->

## Introduction

The direction gyro is used navigation, providing a stable heading reference when the aircraft is turning. This gyro is kept aligned to magnetic north through the use of a remote compass, located in the wing, which gradually aligns the direction gyro whenever the aircraft is not turning.

## Components

### Direction Gyro

This is a horizontal gyro, suspended tangent to the ground. In addition to the yaw axis the gyro can freely rotate along the pitch axis to remain tangent to the ground. This allows the direction gyro to keep a fixed heading in space.

The direction gyro drives the indications on the radio compass card:

![radio compass card](./img/radio_compass_card.png)

and the heading indicator needle:

![heading indicator](./img/heading_indicator.png)

While the direction gyro can keep a fixed heading in space for short periods of time, over long time periods it is subject to different forms of drift. Below are the different forms of drift and their sources.

| Drift | Description | Northern Hemisphere Drift | Southern Hemisphere Drift |
|-------|-------------|---------------------------|---------------------------|
| Earth | As the earth rotates depending on the latitude (north/south) the apparent direction of gyro will drift. This can be more clearly understood by considering a gyro very close to the north pole, the gyro remains pointed at a fixed angle in space irrespective of the earth rotation, as such the apparent direction will drift as the earth rotates. | increasing | decreasing |
| Latitude Nut | The earth rate drift can be effectively countered by an offset weight on the gyro, known as the latitude nut. This direction gyro does not have a latitude nut but instead is electronically corrected using the [latitude knob](#latitude-correction-knob) allowing the pilot to adjust the latitude to keep the gyro accurate. | decreasing | increasing |
| Transport Wander | Similar to drift caused by the rotation of the earth, the aircraft can itself increase or decrease the rotation around the earth by flying east or west. Unlike drift from the earth's rotation there is no compensation for this error. | increasing (east) / decreasing (west) | decreasing (east) / increasing (west) |
| Random Wander | Due to imprecision in components and friction the gyro will naturally precess leading to an error of 1° - 3° per hour, there is also no way to correct for this drift. | random | random |

#### Slaving

Notably transport wander and random wander cannot be corrected. For this reason the direction gyro is used in conjunction with the remote compass so that each system can cover the other's weakness. The remote compass which is accurate on average over long timescales can be used to adjust the direction gyro back towards magnetic north an electric motor is used to precess the gyro towards the measured magnetic north. This is known as slaving the direction gyro to the magnetic compass. The modes are described below.

| Mode | Description | Slaving Rate |
|------|-------------|--------------|
| Direction Indicator | Decouples Direction Gyro from magnetic compass, resulting in no correction. | none |
| Slaving | Slowly slaves the Direction Gyro towards the magnetic compass when the aircraft has not been turning for at least 15 seconds. | 1°/minute |
| Fast-Slaving | Quickly slaves the Direction Gyro towards the magnetic compass when the aircraft has not been turning for at least 15 seconds. | up to 360°/minute |

Upon powering on or after the [function selector switch](#function-selector-switch) is switched from **DG** to **MAG** the direction gyro will enter fast slaving mode.

!!! warning
    If fast-slaving is used when the aircraft is accelerating, turning or pitch attitudes beyond ±30° the direction gyro will be slaved towards an erroneous magnetic compass heading.

#### Leveling

As the aircraft moves the gyro will gradually topple since it is pointed at a fixed point in space. This can lead to erroneous readings. Electrolytic switches are used to indicate when the gyro is out of level from gravity and a motor is used to precess the gyro back into the plane tangent to the ground.

### Thermal Relay

A thermal relay is incorporated into the slaving circuit to control the fast-slave cycle. When the system is switched to the **MAG** position, the relay heats and closes after a brief delay, supplying high voltage to the slaving torque motor for rapid alignment of the gyro to magnetic north. After the fast-slave period ends, the relay cools and reopens, returning the system to its normal slaving rate. Because the relay must cool fully before another fast-slave cycle can occur, repeated switching between **MAG** and **DG** without sufficient cooling time may prevent proper slaving and result in heading errors.

### Remote Compass Transmitter (J-4 Compass)

The remote compass is a magnetic field sensing device which detects the current magnetic north relative to the aircraft heading. As described [above](#direction-gyro) this signal on average will give an accurate indication of magnetic north and as such can be used to slowly adjust (slave) the direction gyro towards magnetic north if it has incurred any errors.

The remote compass is pendulously suspended in fluid to damp excess movement. The remote compass pendulum is limited to 30° max angle in any direction. The result is that under normal operation the pendulum will find the level and give an accurate indication of the magnetic north.

Under turning, acceleration or pitch attitudes exceeding ±30° the pendulum will be displaced from the correct value leading to erroneous heading indications for magnetic north. These errors can be observed by looking at the [annunciator window](#annunciator) to see how the measured error swings as the aircraft maneuvers.

## Controls

![j4 image](./img/j4compass.png) <!-- REPLACE THIS IMAGE -->

1. [Synchronizer Control Knob](#synchronizer-control-knob)
2. [Function Selector Switch](#function-selector-switch)
3. [Annunciator](#annunciator)
4. [Latitude Correction Knob](#latitude-correction-knob)
5. [Hemisphere Switch](#hemisphere-switch)

### Synchronizer Control Knob

The synchronizer control knob is used to manually rotate the direction gyro during slaved or non-slaved operation for rapid orientation of the heading system.

### Function Selector Switch

The function selector switch is a two-position switch marked **MAG** and **DG**. When the switch is in the **MAG** position, the signals from the remote compass transmitter are being used and the system functions as a slaved heading system. When the switch is in the **DG** position, the system is operated in non-slaved mode. Automatic fast slaving occurs for approximately 15 seconds after power is initially applied or whenever the function selector switch is moved from the **MAG** to **DG** and then back to the **MAG** position.

!!! note
    Straight and level flight must be maintained for 15 seconds before attempting to fast-slave the compass indicator. This should permit the rate-switching gyro to restore the magnetic slaving signal to the compass system and allow the compass indicator to synchronize with the correct magnetic heading.

!!! caution
    Two minutes must elapse when switching from the magnetic mode to the directional gyro mode and back to the magnetic mode. This is for cooling of the thermal relay that controls the fast-slave cycle. If the relay is not cooled to permit another complete fast-slave cycle, the indicator may stop at an erroneous reading.

### Annunciator

The annunciator indicates the error between the direction gyro and the current sensed magnetic north, the [synchronizer control knob](#synchronizer-control-knob) can be used for rapid alignment of the heading pointer during slaved operation.

!!! note
    During turns or while accelerating the indication may be erroneous.

### Latitude Correction Knob

The latitude correction knob provides a manual latitude input to the gyro system to counteract apparent drift due to the earth's rotation rate. This should be set to the aircraft’s approximate latitude.

### Hemisphere Switch

The hemisphere switch is set by the ground crew and is not accessible to the pilot.

## Normal Operation

1. Confirm the hemisphere switch has been properly set by ground crew before flight.

2. Turn the [function selector switch](#function-selector-switch) to **MAG** for normal, slaved operation.

3. Maintain straight and level flight for at least 15 seconds to allow the remote compass transmitter and gyro to stabilize.

4. If the heading indication is incorrect, rotate the [synchronizer switch](#synchronizer-control-knob) in the direction indicated by the [annunciator](#annunciator) until the heading pointer aligns with the magnetic heading.

5. Adjust the [latitude correction knob](#latitude-correction-knob) to the aircraft's current latitude to minimize direction gyro drift.

6. If switching between **MAG** and **DG** allow 2 minutes to elapse before returning the switch to **MAG** to ensure the thermal relay cools and the fast-slave cycle can operate correctly.
