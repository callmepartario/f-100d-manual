# A-4 Gunsight

![Gunsight Gif](./img/gunsight.gif)

## Introduction

The A-4 Gunsight is a lead computing optical sight. This system has a gyro to assist in computing the lead solution for aerial gunnery. It's primary input is the range which can be achieved either from the onboard APG-30 radar system or manually by the pilot using the optical sight to range.

The system can also be used for ground attack using various fixed sight modes where pre-calculated depression tables can be used.

### Sight Lines

#### Fuselage Reference Line (FRL)

The defined reference line for pitch for the aircraft. Every other line is referenced from this line.

#### Mean Fixed Bore Line (MFBL)

The mean fixed bore line is a line drawn from the average position of the gun muzzles drawn parallel to the average boresight of the guns.

![Mean Fixed Bore Line Image](./img/mean_fixed_bore_line.png)

#### True 0 Prediction Sight Line (T0PSL)

The line drawn from the A-4 sight position parallel to the [Mean Fixed Bore Line](#mean-fixed-bore-line-mfbl).

#### 0 Prediction Sight Line (0PSL)

A line depressed by some angle from the [True 0 Prediction Sight Line](#true-0-prediction-sight-line-t0psl) to harmonize this line and the [Mean Fixed Bore Line](#mean-fixed-bore-line-mfbl) at some distance usually 2000 ft.

#### Electrically Caged Sight Line (ECSL)

A line depressed by 1.1 mils from the [0 Predication Sight Line](#0-prediction-sight-line-0psl) to account for bullet drop at approximately 850 feet.

This sight line is what is used when the sight is electrically or mechanically caged.

## Controls

### Mechanical Cage Lever

The mechanical cage lever cages the sight to the boresight. With the sight mechanically caged the reticule is fixed and the size of the reticule is determined by the wingspan lever.

![Mechanical Cage Lever](./img/mechanical_cage_lever.png)

### Electrical Cage Button

Pressing the electrical cage button stabilizes the reticule by providing the fire control system with a range of 850 feet. The rigidity of the sight is increased to reduce reticule movement during hard maneuvering.

If this button is depressed the [Sight Selector Switch](#1-sight-selector-switch) automatically moves to the gun position.

### Range Dial

The range dial indicates the current target range in feet being used by the sight. The source of this range can either be the radar or manually if the manual range setting is used.

![Range Dial Image](./img/range_dial.png)

### Radar Range Sweep Knob

This is used to reduce the maximum lock-on distance for the radar to prevent the radar from locking onto undesirable objects.

| Range Limit | Setting (feet)
|-------------|--------
| MIN         | 3000
| MAX         | 9000

The value linearly changes between the min and max settings.

![Radar Range Sweep Knob Image](./img/aux_panel.png)

### Manual Ranging Control (Throttle)

The throttle grip is normally in the full counter-clockwise position for automatic radar ranging. Twisting the throttle grip clockwise decreases the range from the max manual range of 2700 feet to a minimum of 12000 feet.

To return the ranging to automatic operation simply rotate the throttle full counter-clockwise.

![Manual Ranging Control (Throttle) Image](./img/throttle_rotation.png)

### Wingspan Lever

The wingspan lever changes the size of the reticule to match the angular size of a target at the current indicated range. Setting this to the wingspan of the target can either confirm the radar ranging is correct or be used to manually range by changing the manual ranging until the pipper width matches the target.

Due to the added equipement in the F-100D there is a mechanical linkage which connects the interactable wingspan lever with the actual wingspan lever of the A-4 sight.

![Wingspan Lever Image]()

### Radar Lock-On Light

When the radar range gate has achieved lock-on the lock light will illuminate.

![Radar Lock-On Light Image]()

### Radar Reject Button

If the pilot wishes to reject the current radar lock (for example the current range is much lower or higher than the desired target range) the pilot can press the radar reject button. The radar will continue to increase scan range until it either finds a target or reaches max range where it will then begin the scan again at minimum range.

Pressing the radar reject button will cause the [Sight Selector Switch](#1-sight-selector-switch) to move to the guns position.

![Radar Reject Button Image]()

### Sight Selector

![Sight Selector Image](./img/sight_selector_switch.png)

#### 1. Sight Selector Switch

There are three options rocket, gun, bomb. 

| Mode   | Range (feet)  | Electrically Caged
|--------|---------------|-------------------
| Gun    | range from radar or manual | Free to move unless electrical cage is depressed
| Rocket | fixed 850     | Caged to [ECSL](#electrically-caged-sight-line-ecsl) + Depression Angle
| Bomb   | fixed 850     | Caged to [ECSL](#electrically-caged-sight-line-ecsl) + Depression Angle

If the [radar reject button](#radar-reject-button) is depressed this switch automatically moves to the gun postion.

#### 2. Sight Depression

This sets the depression from the boresight in [NATO MILS]() when either in the rocket or bomb mode.

#### 3. Target Speed Switch

This switch sets the effective velocity of the own aircraft and the closure rate for the sight calculations. Each setting is phrased in terms of the target velocity.

| Mode | Own Speed (knots) | Target Speed (knots) | Closure Rate (knots)
|------|-------------------|----------------------|-------------------------------------------
| TR   | 300               | 200                  | 100
| HI   | 600               | 500                  | 100
| LO   | 600               | 200                  | 400

## Operation

How to use.


**TODO: Note to self - If the armament selector is in BOMB/NAPALM and the sight is in manual, the sight will go out if the bomb arming knob is not set in an ARMED position.**

**TODO UPDATE: MAYBE it may depend on the version of the sabre.**
