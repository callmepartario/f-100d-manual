# AN/APR-25 Radar Homing and Warning Receiver

## Introduction

The AN/APR-25 is a Radar Warning and Homing Receiever. This is a piece of equipment which is designed to detect incoming radar and guidance signals and inform the pilot of any threats.


## Theory of Operation

### Theory of Radar

To understand the AN/APR-25 theory of operation it is important to understand the basics of radar.

![Image of Basic Radar Operation]()

The principle operation of radar is to send out a small burst of radiation (usually microwaves) in a direction and measure the time it takes to receive any reflected radiation. The speed of the radiation is known so the time can be used to estimate the distance to whatever reflected the radiation.

#### Carrier Frequency (Band)

The carrier frequency is the frequency of the radiation used for detection of objects. Each pulse contains a burst of these radiation at the carrier frequency.

![Image of Radar Pulse]()

The carrier frequency can be broadly categorised into categories known as bands. The bands for the AN/APR-25 are listed below (note these are similar to NATO bands but not exactly identical):

| BAND  | Frequency (GHz)
|-------|----------------
| India | 7 - 11
| Golf  | 4.4 - 5.8
| Echo  | 2.4 - 3.6

Whenever radar is refered to be in any of these bands it simply means that the radiation it emits falls within the limits of the band.

#### Pulse Repetition Frequency (PRF)

It is not enough to send one pulse of radiation as the energy contained within one pulse is very small so it can be difficult to detect. To improve this and to continually update what the radar is detecting the radar will send a stream of pulses.

The rate at which these pulses are transmitted is known as the pulse repetition frequency. Along with the band the pulse repetition frequency  

### Equipement

The AN/APR-25 uses four antennas to detect incoming radiation. There are two antennas on the nose to detect incoming radiation from the front half and two antennas on the tail to detect incoming radiation from the rear half.

The antennas route to three amplifiers - one for each band. The AN/APR-25 cannot detect 

The band is the first category the AN/APR-25 uses to sort threats. Different detected threats are displayed based on their band.

### Pulse Repetition Frequency (PRF)

It is important to discuss pulse repetition frequency as it is important for categorising threats and is important to radar operation.

The pulse repetition frequency of an radar is 

## Billboard

![Bill Board Controls Image](./img/billboard.png)

### POWER

This button switches the system on, it can take approximately 10-30 seconds (check) for the system to warm up.

### ACT/PWR

This indicates if there are any Charlie band signals detected which match that of a Fan-Song emitting guidance signals. If there is a correlated fan-song on the [Azimuth Display](#azimuth-display) the correlated signal will flash at 3 Hz.

When pressed this button does nothing.

### AAA/AI

This light illuminates when the lower half of the Echo band is triggered, this usually indicates Anti-Aircraft Artillery Fire Control Radars or E Band Airborne Intercept Radars.

### G LORO

This light illuminates when the Fan-Song E (Golf Band Fan-Song) switches to its Lobe On Receive Only, this is to counter jamming and results in the sound switching from the characteristic rattle-snake sound to a steady tone.

### AI

This indicates if there is an India band airborne intercept radar detected and what type the system has categorised.

#### AI WX

This illuminates when a radar with a connical scanning type radar is detected. This is usually indicative of an all weather fighter.

#### AI DAY

This is supposed to represent day fighters with range only radars, like that the F-100D super sabre has. However this RHAW equipement was invented before the widespread use of monopulse radars as such these more advanced radars do not trip the AI WX detection circuitry leading them to be incorrectly classified as AI DAY fighters despite having much more advanced radars.

### SAM Indications Bands (I,G,E)

#### Band Disable

Pressing the respective band button triggers the band disable circuitry. This allows the operator to remove all band indications from the scope and audio completely.

To re-enable the band simply press the button again. There is no indication that the band is disabled so take care to ensure it is set correctly so as to not miss threats.

#### Indications

The threat indications are in the form of two lights on the button, one at the top and one at the bottom. The top light indicates a high pulse repetition frequency for the given threat and the bottom light indicates the low pulse repetition frequency.

As a general rule low pulse repetition frequency is used for acquistion or long range tracking and high pulse repetition frequency is used for shorter range targeting and launch.

Each threat indication is displayed when a radar is detected which matches the pulse repetition frequency of the threat's high or low setting. However other radars can erroneously trigger the threat detection if their pulse repetition frequency coincides with the thread frequencies. 

Each threat indicated for each band are listed below. 

| Button | Band | Indicated Threat
|--------|------|------------------
| I SAM  | India| Low Blow (SA-3)
| G SAM  | Golf | Fan-Song E (SA-2)
| E SAM  | Echo | Fan-Song (early) (SA-2)

**Note currently the Echo Band Fan-Song is not present in the game as such any Echo band threat indications are erroneous.**

### LAUNCH

The launch indication is given when Charlie band guidance activity is detected and correlated to a threat fan-song which has the aircraft centered in its beam.

### AAA Defeat

This button blanks out the lower half of the Echo band effectively disabling Anti-Aircraft Artillary Radars commonly found in this band.

## Azimuth Display


