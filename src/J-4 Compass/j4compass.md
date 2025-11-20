# J-4 Compass

<!-- 
This entire section needs to be reviewed as far as order of sections, titles of sections and the numbers on the image.
Im torn as far as the layout of the numbers marked on the controls image. either to do it left to right in order or number
the elements on said control in the order of logical use in practice. i.e. power then function then adjustments ect ect.
-->

## Introduction - Compass Components

### Remote Compass Transmitter

The remote compass transmitter is the magnetic sensing device of a slaved heading system. It does not function during non-slaved operation. This unit is mounted
at a remote spot in the aircraft where it is free from magnetic disturbances. The magnetic sensing element is pendulously suspended on a universal joint within a sealed bowl so that within a pitch attitude of ± 30° it continuously responds to gravity. To prevent excessive swinging, the bowl is filled with a damping fluid. 

The sensing element picks up the earth's lines of magnetic force and produces electrical signals which are used to orient and maintain the slaved systems to magnetic north. During turns, periods of acceleration or deceleration, and when the pitch attitude exceeds ± 30°, the sensing element produces erroneous signals because it is displaced from the horizontal plane. However, with the stability provided by the gyro, these false signals have little effect on the heading indications. When straight and level flight is again resumed, accurate signals are once again transmitted for proper orientation.

### Gyro

The gyro acts as the stabilizing component in all heading systems by using the gyroscopic property of rigidity in space. The universal, horizontally mounted gyroscope maintains a fixed position as the aircraft turns, and the turning motion around the gyro is electrically relayed to one or more heading indicators.

### Erection Mechanism

An erection mechanism is an integral part of all heading systems and is used to maintain the spin axis of the gyro in a horizontal plane. The most common type consists of an electrolytic switch and an erection torque motor. If the spin axis of the gyro tilts out of the horizontal plane for any reason, the electrolytic switch sends  lectrical signals to the erection torque motor which applies the force to precess the gyro back to the horizontal plane. Thus any heading errors caused by the spin axis tilting out of the horizontal plane are corrected by the erection mechanism. 

A second torque motor is used to precess the gyro in azimuth if the system is slaved. This slaving torque motor uses the signals from the remote compass transmitter to precess the spin axis of the gyro until it is aligned with magnetic north-south and then functions as necessary to keep the spin axis in this north-south alignment.

### Amplifier

The amplifier is the coordinating and distributing center of electrical signals for heading systems. During slaved operation the signals produced by the remote compass transmitter are amplified, phase detected, and sent as correction signals to the slaving torque motor, or in the case of the N-1 system, the master indicator. 

The signal is amplified to increase its strength and phase detected to determine 180° ambiguity. The ambiguity must be resolved since the signals produced are the same strength on any reciprocalheading. If the phase detection circuit fails, the heading system may slave in 180° out of phase. 

Next, the amplifier provides correction signals to keep the slaved heading systems oriented to magnetic north. These signals are directed from the remote compass transmitter either to the slaving torque motor or the master indicator. The amplifier also provides high voltage to the slaving torque motor for fast slaving. Initial slaving is at a fast rate for rapid orientation and usually lastsa specific time. However, some systems stay in fast slave only until the heading system is oriented to magnetic north. After fast slaving ends, the systems go into their normal slaving rate which is about 1 ° to 3 ° per minute.

### Thermal Relay

A thermal relay is incorporated into the slaving circuit to control the fast-slave cycle. When the system is switched to the **MAG** position, the relay heats and closes after a brief delay, supplying high voltage to the slaving torque motor for rapid alignment of the gyro to magnetic north. After the fast-slave period ends, the relay cools and reopens, returning the system to its normal slaving rate. Because the relay must cool fully before another fast-slave cycle can occur, repeated switching between **MAG** and **DG** without sufficient cooling time may prevent proper slaving and result in heading errors.

## Controls

![j4 image](./img/j4compass.PNG) <!-- REPLACE THIS IMAGE -->

1. [Synchronizer Control Knob](#synchronizer-control-knob)
2. [Function Selector Switch](#function-selector-switch)
3. [Annunciator](#annunciator)
4. [Latitude Correction Knob](#latitude-correction-knob)
5. [Hemisphere Switch](#hemisphere-switch)

### Synchronizer Control Knob

The synchronizer control knob is used to rotate the heading pointer during slaved or non-slaved operation for rapid orientation of the heading system.

### Function Selector Switch

The function selector switch is a two-position switch marked **MAG** and **DG**. When the switch is in the **MAG** position, the signals from the remote compass transmitter are being used and the system functions as a slaved heading system. When the switch is in the **DG** position, the system is operated in non-slaved mode. Automatic fast slaving occurs for approximately 15 seconds after power is initially applied or whenever the function selector switch is moved from the **MAG** to **DG** and then back to the **MAG** position.

**Note:** Straight and level flight must be maintained for 15 seconds before attempting to fast-slave the compass indicator. This should permit the rate-switching gyro to restore the magnetic slaving signal to the compass system and allow the compass indicator to synchronize with the correct magnetic heading.

**Caution:** Two minutes must elapse when switching from the magnetic mode to the directional gyro mode and back to the magnetic mode. This is for cooling of the thermal relay that controls the fast-slave cycle. If the relay is not cooled to permit another complete fast-slave cycle, the indicator may stop at an erroneous reading.

### Annunciator

The annunciator indicates the direction to rotate the [synchronizer control knob](#synchronizer-control-knob) for rapid alignment of the heading pointer during slaved operation.

### Latitude Correction Knob

The latitude correction knob provides a manual latitude input to the gyro system to counteract [apparent precession](#apparent-precession). It is required only during **DG** operation and should be set to the aircraft’s approximate latitude.

### Hemisphere Switch

The hemisphere switch is set by the ground crew and is not accessable to the pilot.

## Heading System Errors

All heading systems are subject to errors produced by gyro drift, and real and [apparent precession](#apparent-precession). If provisions for correction are incorporated in the design of the system, all these errors will be negligible.

### Real Precession

During turns and periods of acceleration and deceleration, forces are produced which combine with the force of gravity to cause the erection mechanism and the remote
compass transmitter to induce errors in the heading system. However, once straight and level flight is resumed, the remote compass transmitter and the erection mechanism are able to seek a true gravity and to correct any errors that developed. To reduce errors that would develop during turns because of real precession, the slaving control was added to some heading systems. The slaving control cuts out the remote compass transmitter circuit and the erection circuit to prevent these errors from occurring. During non-slaved operation the remote compass transmitter is not in use; therefore, no errors are induced from this source. The erection mechanism will induce errors during turns and changes of airspeed, but these errors are corrected when straight and level unaccelerated flight is resumed. The slaving control, if part of the system, prevents real precession errors that occur in turns by interrupting the erection mechanism circuit
during the turn.

### Gyro Drift

Internal forces such as friction and rotor imbalance cause precession of the gyro spin axis in both tilt and turn. Since all heading systems, slaved or non-slaved, have an erection mechanism, the tilting of the spin axis is corrected and no errors result. If the spin axis of the gyro turns, a heading error is present. In the slaved
systems, the signals from the remote compass transmitter are used to reorient the system to magnetic north and thus to eliminate the heading error. During non-slaved operation, there is no automatic alignment and errors accumulate unless the system is reoriented manually. To reduce the amount of gyro drift errors, better gyros have been developed with drift rates of less than + 1 ° / hour. In most non-slaved systems not designed for use at all latitudes, the allowable drift rate is about ±4° /hour.

### Apparent Precession

A horizontal, universally mounted gyroscope is affected by apparent precession anywhere between the equator and the poles. The higher the latitude the greater the gyro
will appear to precess. The exact amount of precession in degrees per hour can be computed by the trignometric equation: 15° times the sine of the latitude. Using the preceding relationship, the apparent precession at 30° latitude would be 7.5/hour; at the poles the rate would be 15°/hour. The precession appears clockwise in the northern hemisphere and counterclockwise in the southern hemisphere.

Apparent precession causes the spin axis of the gyro both to tilt and turn. Any tilting is cor rected by the erection mechanism in both the slaved and non-slaved systems. Apparent precession that causes the spin axis to turn is corrected by the signals from the remote compass transmitter during slaved operation. During non-slaved
operation, latitude correction is used to reduce errors caused by apparent precession. If latitude correction is available for all latitudes, the heading system can be operated in the non-slaved mode with very little error. If latitude correction is not available, non-slaved systems will accumulate heading errors, the extent of error depending on the latitude.

### Fast Slaving Error

In slaved systems with an automatic fast slave cycle, errors develop if the aircraft is turned or accelerated during the cycle. The remote compass transmitter produces
erroneous signals during turns and periods of acceleration, and because of the fast slaving rate the heading indicator will present errors similar to those of the magnetic compass. During normal slaving these errors are not present because of the slow slaving rate. Note that systems with a slaving control are not affected by the fast slaving rate in turns if the aircraft is turning at a rate sufficient to cut out the remote compass transmitter and the erection mechanism.

## Normal Operation

1. Confirm the hemisphere switch has been properly set by ground crew before flight.

2. Turn the [function selector switch](#function-selector-switch) to **MAG** for normal, slaved operation.

3. Maintain straight and level flight for at least 15 seconds to allow the remore compass transmitter and gyro to stabilize.

4. If the heading indication is incorrect, rotate the [syncronizer switch](#synchronizer-switch) in the direction indicated by the [annunciator](#annunciator) until the heading pointer aligns with the magnetic heading.

5. If operating in **DG**, adjust the [latitude correction knob](#latitude-correction-knob) to the aircraft's current latitude to minimize [apparent precession](#apparent-precession).

6. If switching between **MAG** and **DG** allow 2 minutes to elapse before returning the switch to **MAG** to ensure the thermal relay cools and the flast-slave cycle can operate correctly.
