# AGM-45 Shrike

## Introduction

The AGM-45 Shrike is an anti-radiation guided air to ground missile, introduced in 1965 and employed heavily during the Vietnam war.

The F-100F could carry one Shrike Missile on each of the inner pylons. The F-100D never strictly carried the Shrike missile however the pylon used existed on both models and the avionics between the two are very similar which would allow the same modifications justifying its presence in the game.

The Shrike is passive and guides on the signals radiated by the enemy surface radars. This makes it an ideal weapon for suppressing and destroying surface to air missile and anti-aircraft radars. The antenna inside the shrike is fixed but provides direction information to incoming radar signals allowing the missile to guide to a target provided the radar is within the field of view of the seeker.

## Shrike Settings

### Radio Seeker

The radio seeker of the shrike determines what radars can be tracked. To target specific radar systems narrow band radio seekers were used. These seekers could be swapped out to attack the specific threat dictated by the mission.

![seeker selection screen]()

### Dive Bypass

In addition to the radio seekers the shrike has two possible guidance modes which have an effect on the trajectory of the missile: loft and dive bypass.

![seeker loft screen]()

#### Loft - Dive Bypass (disabled)

When launched the guidance is initially disabled. Once the missile passes climbs above 18,000 ft and then descends below 18,000 ft barometric will the seeker and guidance then be activated. At this point the missile will track anything within it's field of vision that falls within it's radio seeker band.

This mode is intended for stand-off however without additional computer assistance like that added later in the F-4D this mode is difficult to attain accuracy.

#### Dive Bypass - Dive Bypass (enabled)

Due to the aforementioned difficulty a solution was sought in the field to improve the accuracy of the shrikes. The dive bypass modification was made and this enables the radio seeker and guidance at launch. Sacrificing range for improved accuracy.

Shrikes fired with this setting will guide immediately so for best results it is best to point the missile as close to the target elevation and azimuth as possible.

To assist this the [shrike steering needles](#course-and-glideslope-needles) can be used.

### Marker Smoke

Marker smoke can be added to the shrike to assist with locating surface radars in the event of a near miss. Upon impact the shrike will burn a white phosphorous charge to produce a column of smoke indicating the impact point.

![marker smoke option]()

## Controls and Indications

### Audio

The audio of the shrike is generated from the incoming pulses of radiation similar to how the [Radar Homing and Warning Receiver](../RHAW/RHAW.md#audio-generator) generates audio.

Any audio indicates incoming signals detected by the radio seeker which can be used by the guidance system to home the missile on the source of the signal.

### Course and Glideslope Needles

When there is a valid shrike powered and selected the course and glideslope needles indicate the error in pitch and yaw between the seeker boresight and the detected incoming radiation. This allows the pilot to steer the aircraft onto the source of the radiation.

### Sidewinder Volume Knob

The sidewinder volume knob can be used to adjust the Shrike audio heard in the headset.

## Operation

### Setup & Firing

1. [Sight Mode]() - Manual
2. [Armament Mode]() - Shrike
3. [Pylon Arm]() - Armed for each pylon

One the Shrike is setup the pilot can point the aircraft at a radiation source to hear the radiation through the Shrike, this indicates a good track. The [needles](#course-and-glideslope-needles) will also become active and point to the source.

To fire depress the weapon release until the missile completes the launch sequence.
