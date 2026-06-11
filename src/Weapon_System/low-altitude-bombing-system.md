# AN/AJB-1 Low Altitude Bombing System

## Introduction

The low altitude bombing system was introduced to assist with nuclear weapons delivery. It helps the pilots follow a pre-determined trajectory to delivery nuclear weapons with delivery profiles to assist with escape from the effects of the blast.

## Controls and Indicators
![labs](./img/labs.png)

### Pullup Light

Active when LABS is active before the pullup. Once pullup occurs this light goes out.

### Roll Indicator

Indicates the current desired roll by the system.

### Pitch Indicator

Indicates desired G load in pullup mode and desired pitch angle in pre-pullup mode.

## Operation

All LABS delivery modes share the pullup timer. The pullup timer is the time set by the pilot to indicate the time taken for the aircraft to fly from a know identification point (IP) to the pullup point.

There are two variables which determine pullup timer:

- ground speed
- bomb travel distance
- distance from IP to target

The formula:

`pullup timer = (distance from ip to target - bomb travel distance) / ground speed`

can then be used to figure out what should be set for the pullup timer. Both ground speed and distance from IP to target can be easily chosen during mission planning. The identification point (IP) is chosen to be something that is easy to find and navigate to from the air and near the target area.

Bomb travel distance is determined by the exact release parameters of the bomb: including release angle, true airspeed, target altitude, aircraft altitude, bomb type and wind.

### LABS (Loft)

The LABS mode is the one of the normal delivery types for the labs. It is intended for lofting nuclear weapons long distances. The release angle is 50 degrees which lofts the weapon a long distance towards the target.

### LABS ALT (Over the Shoulder)

The LABS ALT mode is the alternate method for a loft type delivery. It is intended for lofting a nuclear weapon vertically over the target.

The LABS and LABS ALT mode are identical with the exception of the angle of release. Below is a table of release angles:

| Mode     | Delivery Angle (degree)
|----------|-------------------------
| LABS     | 50 (LOFT)
| LABS ALT | 120 (OVER THE SHOULDER)

![Image of Loft Release](./img/labs_loft_delivery.png)

### Low Altitude Drogue Delivery (LADD)

Low Altitude drogue Delivery is for delivery drogue assisted nuclear weapons. At the pullup point the pilot is commanded into a 40 degree climb. The release timer determines the release. Once a period longer than the release timer has passed since the pullup point the bombs will be released.
