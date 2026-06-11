# Electrical System

![electrical system diagram](./img/electrical_system.png)

## Introduction

The F-100D features two mostly separated electrical systems: the [AC System](#ac-system) powered by the AC Generator or external power, the [DC System](#dc-system) powered by the DC Generator, Battery or external power.

These systems are powered independently however in the event of failures it's possible to partially power failed system using the still working system.

## DC System

The DC System normally receives power from the battery and DC generator. Optionally power can also be received from external power if connected.

### DC Generator

The engine driven DC generator provides power to the DC systems under normal operation.

!!! note
    The DC generator connects at approximately 40% engine RPM.

!!! note
    The DC generator only needs to be reset if an electrical fault causes it to trip off the line.

### Battery Bus

The battery bus is connected directly to the battery, so that essential equipment powered by this bus is operable as long as battery power is available, **regardless of battery switch position**.

The battery is 24 Volt, 24 ampere hour battery. The DC Generator nominally outputs 28 Volts.

The battery bus is connected to the battery bus through the primary bus tie in relay. This relay is energized by the battery bus connecting the battery bus to the primary bus.

If there is not enough power on the battery bus the battery will not be connected, however if the primary bus is being energized from elsewhere (DC generator or External Power) the battery bus can be kept connected even if the battery has insufficient power to keep the relay energized. Turning the battery switch off under this condition will disconnect the primary bus from the battery bus and the battery will no longer be able to be charged.

### Primary Bus

Primary bus powers the most essential equipment. Energized by battery bus when battery switch is ON, or energized by DC generator or external power. Energized by transformer-rectifier if DC generator fails.

### Secondary Bus

Secondary bus powers less essential equipment. Energized by primary bus when DC generator power, DC ground power or transformer-rectifier power is available to close the secondary bus tie-in relay, where then it is powered by the primary bus.

### Tertiary Bus

Tertiary bus powers non-essential equipment. Energized by primary bus when external power or DC generator power is available to close bus tie-in relay, where then it is powered by the primary bus.

## AC System

### AC Generator

The engine driven AC generator provides power to the AC systems under normal operation. The AC generator is driven by a constant speed drive driven by the engine.

!!! note
    The constant speed drive takes up to a minute at idle power to come up to speed so that the AC generator can come on the line. To expedite this process the pilot can advance the throttle up to 72% (or until the generator comes online).

!!! note
    The AC generator needs to be reset if an electrical fault causes it to trip off the line or the AC generator switch is placed into the off position.

### Main Three-Phase AC Bus (115V)

Main three-phase AC bus powers essential equipment which demands AC power. Power is provided by the engine driven AC generator.

### AC Instrument Buses (115V and 26V)

There are two instrument buses which power vital instrument equipment. Due to their important these AC buses can both be powered by the [DC primary bus](#primary-bus) using the [standby instrument inverter](#standby-instrument-inverter)

### Controls and Indications

### AC Load Meter

Current AC generator load as a percentage of its maximum load.

![acload](./img/acload.png)

### DC Load Meter

Current DC generator load as a percentage of its maximum load.

![dcload](./img/dcload.png)

### INST A.C. POWER OFF Light

![instacoff](./img/instacpowerofflight.png)

Indicates when instrument AC buses are not receiving sufficient electrical power. 

### A.C. GENERATOR OFF

![acoff](./img/acgenoff.png)

Indicates when the AC generator is off the line either because of insufficient drive RPM or a fault has tripped the generator.

### D.C. GENERATOR OFF
![dcoff](./img/dcgenoff.png)

Indicates when the DC generator is off the line either because of insufficient drive RPM or a fault has tripped the generator.

### Standby Instrument Inverter
![stbyinv](./img/stbyinv.png)

Transfers [AC instrument bus power](#ac-instrument-buses-115v-and-26v) over to the standby instrument inverter. The is a small power interruption as the standby instrument inverter comes up to speed.