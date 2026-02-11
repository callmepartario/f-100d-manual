# Fuel System

## Introduction

The fuel system includes three main tanks in the fuselage and a tank in each wing. Drop tanks may be installed on any of the six wing pylons.

Fuel is automatically balanced in the aircraft using a series of valves and float triggered pumps. All fuel ends up in the forward fuselage tank where it is then passed to the engine through the manifold.

All fuel to the engine passes through a 1.6 gallon inverted flight tank which gives fuel for short periods of negative or zero g.

The aircraft has a single point pressure refueling system which allows for both ground and air-to-air refueling of all the aircrafts internal tanks. This system also has provisions for filling 275 and 335 gallon drop tanks on the intermediate pylons allowing for in-flight refueling on these tanks on intermediate pylons. Other tanks on other pylons cannot be refueled this way.

## Fuel Tanks

There are 4 primary fuel tanks.

| Tank | Cells | Capacity (combined in lbs) | Description
|------|-------|----------------|-------------
| Forward Fuselage | Upper, Centre Left, Centre Right, Lower | 2912 | Engine Manifold primarily draws from this tank.
| Intermediate Fuselage | Left, Right | 1391 | These primarily feed into the forward fuselage however in case of [transfer pump](#fuel-transfer-and-scavenge-pumps) failure the right cell can directly feed the engine.
| Aft Fuselage | Centre | 702 | This primarily feeds into the the forward fuselage however in case of [transfer pump](#fuel-transfer-and-scavenge-pumps) failure the aft fuselage can gravity transfer to the intermediate fuselage tank.
| Wing | Left, Right | 2723 | These feed into forward fuselage by gravity and the [scavenge pumps](#fuel-transfer-and-scavenge-pumps)
| External | Up to one per wing pylon | configuration dependent | These feed into the forward fuselage tank via bleed air pressure. Which pair of tanks feeding depends on the [drop tank selector switch](#drop-tank-selector-switch) position.

## Inverted Flight Tank

The inverted flight tank is the direct feed to the engine. The inverted flight tank can be fed either from the manifold, which is inturn fed by the upper and lower forward fuselage tank, or the intermediate fuselage tank.

The geometry of this tank is designed such that when inverted there is still about 1.6 gallons of fuel for short periods of operation. The length of time of operation before flameout depends on the fuel flow as this will directly impact how fast this inverted flight tank is exhausted. Approximate values for afterburner and military thrust are listed below as a rough guideline.

| Power Setting | Time before Flameout (seconds)
|---------------|----------------------
| Afterburner   | 1.5
| Military      | 6.0

## Fuel Booster Pumps

There are a total of three boost pumps, all three are located in the forward tank. Two AC pumps are located in the upper cell and one DC pump is located in the lower cell. These all feed into the fuel supply manifold which can also be gravity fed from the lower forward tank cell.

## Fuel Transfer (and Scavenge) Pumps

There are two transfer pumps. Normally the intermediate and aft tanks transfer to the forward tanks when the level of the forward tank drops. This is to maintain mass balance but also because the primary feed is in the forward tank.

In case of transfer pump failure it may not be possible to transfer all fuel from the intermediate and aft tanks as such the intermediate tank can directly feed the engine by gravity. The aft tank can also transfer using gravity to the intermediate tank for direct feed to the engine in this scenario.

> Due to the volume of fuel flow when the afterburner is operating it is not possible to keep the forward tank full despite transfers from external and internal tanks to the forward tank. Thus the pilot must monitor the forward fuel tank level so as to not cause an engine flame-out due to insufficient fuel in this tank to feed the engine.

## Drop Tanks

Drop tanks can be mounted on any of the wing pylons. However only the 335 gallon and 450 gallon tanks can be refueled when mounted on the intermediate pylons. The list of the available tanks is shown below.

| Tanks (gallon) | Pylons              | Mid-Air Refuelable
|----------------|---------------------|------------
| 200            | All                 | No
| 275            | Intermediate only   | No
| 335            | Intermediate only   | Yes
| 450            | Intermediate only   | Yes

Tanks are pressurised by the engine bleed air when [drop tank selector switch](#drop-tank-selector-switch) is set to any position other than `OFF`. In case of electrical failure the bleed air valves are normally open position allowing fuel transfer from all external tanks simultaneously.

> Due to the volume of fuel flow when the afterburner is operating it is not possible to keep the forward tank full despite transfers from external and internal tanks to the forward tank. Thus the pilot must monitor the forward fuel tank level so as to not cause an engine flame-out due to insufficient fuel in this tank to feed the engine.

## Fuel System Shutoff Valve

The fuel shutoff valve is an electronically acutated valve which can be used to shut off fuel to the engine. In case of valve failure the [fuel system shutoff valve fail light](#fuel-system-shutoff-valve-fail-light) will illuminate.

## Controls and Indicators

### Drop Tank Selector Switch

This selects which external tanks are pressurised by the engine bleed air. In case of electrical failure the bleed air valves are normally open position allowing fuel transfer from all external tanks simultaneously.

### Drop Tank Empty Indicator Light

This indicates there is no longer any fuel pressure from the drop tanks. However since the external tank fuel line is shared with the internal wing tank scavenge pumps this light will go out again once the wing tanks begin to scavenge at about 4000 pounds of fuel. This light will then illuminate again one the wing tanks are empty at about 1500 pounds of fuel.

### Fuel System Shutoff Valve Fail Light

This light will illuminate if the fuel system shutoff valve is stuck as this could restrict fuel flow to the engine.

### Air to Air Refueling Switch

This de-energises the transfer control valves for the internal wing and external fuel tanks, allowing the single point pressure refueling system to refuel these tanks correctly.

> Do not position this to `READY` too soon as this prevents about 25 pounds per minute of fuel from being transfered from the internal wing tanks to the forward tank.

### Air Refueling Indicator Light

This light simply indicates if the [air to air refueling switch](#air-to-air-refueling-switch) is in the ready position. It does not indicate if all the systems are functional.

### Fuel Boot Pump Light

This illuminates if there is less than 5 psi fuel pressure to the engine indicating a condition where one or more fuel boost pumps are non-functional.

### Forward Fuel Quantity Gauge

Indicates total quantity of all forward fuselage tanks.

### Total Fuel Quantity Gauge

Indicates total quantity of all internal tanks.
