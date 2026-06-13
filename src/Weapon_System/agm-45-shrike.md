# AGM-45 Shrike

## Introduction

The AGM-45 Shrike is an anti-radiation guided air to ground missile, introduced in 1965 and employed heavily during the Vietnam war.

The F-100F could carry one Shrike Missile on each of the inner pylons. The F-100D never strictly carried the Shrike missile. However, the pylon used existed on both models and the avionics between the two are very similar, and would allow the same modifications, justifying its presence in the game.

The Shrike is passive, and guides on the signals radiated by the enemy surface radars. This makes it an ideal weapon for suppressing and destroying surface to air missile and anti-aircraft radars. The antenna inside the Shrike is fixed, but provides direction information to incoming radar signals allowing the missile to guide to a target provided the radar is within the field of view of the seeker.

## Shrike Settings

### Radio Seeker

The radio seeker of the Shrike determines what radars can be tracked. Narrow band radio seekers were used target specific radar systems. These seekers could be swapped out to attack the specific threat dictated by the mission. The RF Guidance Unit can be changed on the AGM-45 in the mission settings and in the weapon rearming menu by clicking the orange triangle in the top left corner of the Shrike icon and selecting a Guidance Unit.

![seeker selection screen](./img/shrike_seeker_select.png)

### Dive Bypass

In addition to the radio seekers. the Shrike has two guidance modes that affect trajectory of the missile: loft and dive bypass (direct attack). These settings can also be found in the same menu as the Guidance Seeker options.

![seeker loft screen](./img/shrike_attack_mode.png)

#### Loft—Dive Bypass (disabled)

When launched, guidance is initially disabled. If the missile climbs above 18,000 feet (barometric), and then descends below 18,000 feet will the seeker and guidance then be activated. At this point, the missile tracks anything in its field of vision and within the seeker band.

This mode is intended for stand-off, but without additional computer assistance (for example, what was added later in the F-4D), this mode is difficult to attain accuracy.

#### Dive Bypass—Dive Bypass (enabled)

Due to the aforementioned difficulty, a solution was developed to improve the Shrike accuracy in the field. The dive bypass modification enables radio seeker and guidance at launch, sacrificing range for improved accuracy.

Shrikes fired with this setting will guide immediately. For best results, use the [course and glideslope needles](#course-and-glideslope-needles) to point the missile as close to  target elevation and azimuth as possible.

### Marker Smoke

Marker smoke can be added to the Shrike to assist with locating surface radars in the event of a near miss. Upon impact, the shrike burns a white phosphorous charge, producing a column of smoke at the impact point. This setting can be found in same menu where Guidance and attack modes are found labeled "WP Marker Charge".

![marker smoke option](./img/shrike_white_smoke.png)

## Controls and Indications

### Audio

The audio of the shrike is generated from incoming pulses of radiation. similar to how the [Radar Homing and Warning Receiver](../RHAW/RHAW.md#audio-generator) generates audio.

Any audio indicates incoming signals detected by the radio seeker. These signals are used by the guidance system to home the missile on the source of the signal.

### Course and Glideslope Needles

When a Shrike is powered and selected, the [course and glideslope needles](#course-and-glideslope-needles) will indicate the error in pitch and yaw between the seeker boresight and the detected incoming radiation. This allows the pilot to steer the aircraft onto the source of the radiation and by keeping the vertical and horizontal deviations bars centered you is pointed at the detected signal.

![shrike course needles](./img/shrike_course_gauge.png)

### Sidewinder Volume Knob

The sidewinder volume knob on the missile control panel adjusts Shrike audio in the headset.

## Operation

### Setup & Firing

1. [Sight Mode]()—Manual
2. [Armament Mode]()—Shrike
3. [Pylon Arm]()—Armed for each pylon

Once the Shrike is set up, point the aircraft at a radiation source to hear the radiation through the Shrike, indicating a good track. The [needles](#course-and-glideslope-needles) will activate and provide additional guidance toward the source.

To fire, depress the weapon release button on the flight stick until the missile completes its launch sequence.
