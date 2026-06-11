# A-4 Gunsight

![Gunsight Gif](./img/gunsight.gif)

## Introduction

The A-4 Gunsight is a lead computing optical sight. This system has a gyro to assist in computing the lead solution for aerial gunnery. It's primary input is the range which can be achieved either from the onboard APG-30 radar system or manually by the pilot using the optical sight to range.

The system can also be used for ground attack using either a fixed sight where pre-calculated depression tables can be used or the inbuilt automatic bombing mode.

## Controls

### Mechanical Cage Lever

The mechanical cage lever cages the sight to the boresight. With the sight mechanically caged the reticule is fixed and the size of the reticule is determined by the wingspan lever.

![Mechanical Cage Lever](./img/mechanical_cage_lever.png)

### Electrical Cage Button

Pressing the electrical cage button stabilizes the reticule by providing the fire control system with a range of 850 feet. The rigidity of the sight is increased to reduce reticule movement during hard maneuvering.

If this button is depressed the [Sight Selector Switch](#1-sight-selector-switch) automatically moves to the gun position.

### Range Dial

The range dial indicates the current target range in feet being used by the sight. The source of this range can either be the radar or manually if the manual range setting is used.

![Range Dial Image](./img/A4_sight_range_dial.png)

### Radar Range Sweep Knob

The Range Sweep Knob labeled dial 6 below, is found next to the Auxiliary Release Buttons and is used to reduce the maximum lock-on distance for the radar to prevent the radar from locking onto undesirable objects such as the ground or ground objects. During normal operation at altitudes 6000 feet or more above the terrain, the rheostat should be at MAX.

| Range Limit | Setting (feet)
|-------------|--------
| MIN         | 3000
| MAX         | 9000

The value linearly changes between the min and max settings.

### Sight Dimmer

The brightness of the sight pipper can be adjusted using the Sight Dimmer rheostat labeled dial 7 below.

### Sight Filament Selector Switch

The primary or secondary filament in the dual-filament sight reticle bulb
can be selected by the sight filament selector switch labeled 1 in the image below. It
should be moved to SECONDARY if the primary filament fails. The switch is powered by the secondary bus and the tertiary bus.

![Radar Range Sweep Knob Image](./img/aux_panel.png)

### Manual Ranging Control (Throttle)

The throttle grip is normally in the full counter-clockwise position for automatic radar ranging. Twisting the throttle grip clockwise decreases the range from the max manual range of 2700 feet to a minimum of 12000 feet.

To return the ranging to automatic operation simply rotate the throttle full counter-clockwise.

![Manual Ranging Control (Throttle) Image](./img/throttle_rotation.png)

### Wingspan Lever

The wingspan lever changes the size of the reticule to match the angular size of a target at the current indicated range. Setting this to the wingspan of the target can either confirm the radar ranging is correct or be used to manually range by changing the manual ranging until the pipper width matches the target.

Due to the added equipment in the F-100D there is a mechanical linkage which connects the interactive wingspan lever with the actual wingspan lever of the A-4 sight.

![Wingspan Lever Image](./img/wingspan-lever.png)

### Radar Lock-On Light

When the radar range gate has achieved lock-on the lock light will illuminate.

![Radar Lock-On Light Image](./img/lock-on.png)

### Radar Reject Button

The radar reject button is found on the control stick. If the pilot wishes to reject the current radar lock (for example the current range is much lower or higher than the desired target range) the pilot can press the radar reject button. The radar will continue to increase scan range until it either finds a target or reaches max range where it will then begin the scan again at minimum range.

Pressing the radar reject button will cause the [Sight Selector Switch](#1-sight-selector-switch) to move to the guns position.

### Sight Selector

![Sight Selector Image](./img/sight_selector_switch.png)

#### 1. Sight Selector Switch

There are three options rocket, gun, bomb. 

| Mode   | Range (feet)  | Electrically Caged
|--------|---------------|-------------------
| Gun    | range from radar or manual | Free to move unless electrical cage is depressed
| Rocket | fixed 850     | Caged to [ECSL](#electrically-caged-sight-line-ecsl) + Depression Angle
| Bomb   | fixed 850     | Caged to [ECSL](#electrically-caged-sight-line-ecsl) + 10 degrees - used with [automatic bombing mode](#bomb-air-to-ground-automatic)

If the [radar reject button](#radar-reject-button) is depressed this switch automatically moves to the gun position.

#### 2. Sight Depression

This sets the depression from the boresight in [NATO MILS]() when either in the rocket or bomb mode.

#### 3. Target Speed Switch

This switch sets the effective velocity of the own aircraft and the closure rate for the sight calculations. Each setting is phrased in terms of the target velocity.

| Mode | Own Speed (knots) | Target Speed (knots) | Closure Rate (knots)
|------|-------------------|----------------------|---------------------
| TR   | 300               | 200                  | 100
| HI   | 600               | 500                  | 100
| LO   | 600               | 200                  | 400

## Operation

The A-4 gunsight can be used in either air to air or air to ground operation. To select the mode of operation the [sight selector](#sight-selector) is used - each modes of operation are described below.

Note if the sight select mode is in manual, the armament mode is in bombs or napalm, and the bomb-arm switch is in SAFE the gunsight pipper will extinguish to indicate that a dud would be dropped off the aircraft.

### Gun (Air-to-Air)

With the [sight selector](#sight-selector) in Gun and the sight mechanically uncaged the rate gyro inside the sight controls the pipper location to provide a gunnery solution based on the set range. The [target speed switch](#3-target-speed-switch) should be set on the closest target speed: HI for High Speed Targets, LO for Low Speed Targets and TR for Tracking Shots where the attacking aircraft is similar speed to the target.

#### Ranging

The range is controlled either manually using the [throttle twist](#manual-ranging-control-throttle) or automatically by the radar.

The radar automatically locks onto any sufficiently strong reflections including the ground. The range is indicated on the [range dial](#range-dial). If the range indicated is not that of the desired target, the target can be rejected using the [radar reject button](#radar-reject-button) this will cause the range sweep to increase and look for targets, if no targets are found and the range sweep reaches the max range it will begin again at the minimum radar range.

The range can be validated in radar ranging or calculated in manual ranging mode by using the [wingspan lever](#wingspan-lever) to set the wingspan of the current target on the gunsight. Then the target is at the correct range when the wingspan matches the inside radius of gunsight reticule tick marks.

#### Gunnery

In order to achieve accurate air-to-air gunnery the sight must be allowed to stabilize. The sight must be kept on the target for 1 - 2 seconds. This allows the gyro to settle on the correct solution for the current attack geometry, firing before the sight is stabilized will result in a miss.

### Rocket (Air-to-Ground Manual)

With the [sight selector](#sight-selector) in Rocket and the sight mechanically uncaged the Sight Depression controls the depression (in mils) of the pipper from the [electrically caged sight line](#electrically-caged-sight-line-ecsl).

In this mode the sight can be used in this mode for manual bombing or rocket attacks.

### Bomb (Air-to-Ground Automatic)

The A-4 sight has a mode for automatic bombing. This method makes use of the inbuilt gyroscope calculate the target position and matches this to an inbuilt mechanical computer using information such as airspeed to calculate the bomb trajectory. Once the the bomb trajectory coincides with the target position the bomb release signal is sent.

The bombsight works the principle that the line of sight rate corresponds to the slant range to the target. To facilitate this the pipper is automatically depressed by 10 degrees in the bomb mode. The pilot must then keep this on the target for the system to measure the line of sight rate. One the parameters are met the sight extinguishes and the bomb is released.

Note that the electrical cage must be held up until the target is in the sight to protect the gyros. Then the target must be _smoothly_ followed under the pipper to get an accurate measurement. Any jerks or bumps may cause the bombs to release prematurely.

## Sight Lines Definitions

### Fuselage Reference Line (FRL)

The defined reference line for pitch for the aircraft. Every other line is referenced from this line.

### Mean Fixed Bore Line (MFBL)

The mean fixed bore line is a line drawn from the average position of the gun muzzles drawn parallel to the average boresight of the guns.

![Mean Fixed Bore Line Image](./img/mean_fixed_bore_line.png)

### True 0 Prediction Sight Line (T0PSL)

The line drawn from the A-4 sight position parallel to the [Mean Fixed Bore Line](#mean-fixed-bore-line-mfbl).

### 0 Prediction Sight Line (0PSL)

A line depressed by some angle from the [True 0 Prediction Sight Line](#true-0-prediction-sight-line-t0psl) to harmonize this line and the [Mean Fixed Bore Line](#mean-fixed-bore-line-mfbl) at some distance usually 2000 ft.

### Electrically Caged Sight Line (ECSL)

A line depressed by 1.1 mils from the [0 Predication Sight Line](#0-prediction-sight-line-0psl) to account for bullet drop at approximately 850 feet.

This sight line is what is used when the sight is electrically or mechanically caged.