# Electrical System

![electrical system diagram](./img/electrical_system.png)

## Introduction

The F-100D features two mostly separated electrical systems: the [AC System](#ac-system) powered by the AC Generator or external power, the [DC System](#dc-system) powered by the DC Generator, Battery or external power.

These systems are powered independently however in the event of failures it's possible to partially power failed system using the still working system.

## Controls

## DC System

The DC System receives power from the battery and DC generator. Optionally power can also be received from external power if connected.

### Battery Bus

The battery bus is connected directly to the battery, so that essential equipement powered by this bus is operable as long as battery power is available, **regardless of battery switch position**.

The battery is 24 Volt, 24 ampere hour battery. The DC Generator nominally outputs 28 Volts.

The battery bus is connected to the battery bus through the primary bus tie in relay. This relay is energised by the battery bus connecting the battery bus to the primary bus.

If there is not enough power on the battery bus the battery will not be connected, however if the primary bus is being energised from elsewhere (DC generator or External Power) the battery bus can be kept connected even if the battery has insufficient power to keep the relay energised. Turning the battery switch off under this condition will disconnect the primary bus from the battery bus and the battery will no longer be able to be charged.

### Primary Bus

The primary bus powers the most essential equipment to the aircraft. Under normal operation it is powered by the DC Generator, but can be powered by the battery or 

| Power Source | Condition
|--------------|------------
| DC Generator | Normal Operation
| External Power | Ground Power Connected
| Battery Bus | Battery has enough voltage and battery switch is on
| Rectifier | DC Generator Failure

### Secondary Bus

### Tertiary Bus

## AC System

### Main Three-Phase AC Bus (115V)

### Three-Phase AC Instrument Bus (115V)

### Single-Phase AC Instrument Bus (26V)