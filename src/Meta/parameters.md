# Parameters

Parameters can be used by DCS missions and plugins to read the internal state of the aircraft.

| Parameter              | Description
|------------------------|--------------
| TACAN_CHANNEL          | Number of the [TACAN](../ARN-72%20TACAN/tacan.md) channel (X-channels only). |
| COMM_FREQ              | Frequency of the [UHF Radio](../ARC-34%20Command%20Radio/command-radio.md) in Hz |
| RADIO_COMPASS_FREQ     | Frequency of the [AN/ARN-6 Radio Compass](../ARN-6%20Radio%20Compass/radio-compass.md) in Hz. |
| AFTERBURNER_STATE      | Afterburner [throttle detent](../Introduction/stick-and-throttle.md#throttle) position: _(0)_ Unlit; _(1)_ Lit (Ignition failures failure are not indicated.) |
| ENGINE_RPM             | 0-100, engine RPM in %. |
| FLAP_STATE             | 0-1, average position: _(0)_ Flaps retracted; _(1)_ Flaps fully extended |
| GEAR_STATE             | 0-1, average position: _(0)_ Gear retracted; _(1)_ Gear extended |
| TRANSPONDER_CODE       | Transponder Code given for Mode 3 code given as a number. If the IFF is unable to respond (off or in standby), the value is 0. |
| GUN_MISSILE_SWITCH     | Position of the Gun/Missile Switch with positions: _(0)_ MISSILES; _(1)_ SAFE; _(2)_UPPER; _(3)_ALL; _(4)_ LWR; _(5)_ POD |
| MODE_SELECT_SWITCH     | Position of the Mode Selector with positions: _(0)_ OFF; _(1)_ SIGHT & RADAR; _(2)_ MANUAL; _(3)_ LABS; _(4)_ LABS ALT; _(5)_ LADD |
| ARMAMENT_SELECT_SWITCH | Position of Armament Selector with positions: _(0)_ OFF; _(1)_ RKTS; _(2)_ BOMBS; _(3)_ DISP; _(4)_ NAPALM; _(5)_ SPL STORES; _(6)_ INOP/SHRIKE; _(7)_ TANK JETT; _(8)_ DISP JETT; _(9)_ PYLON JETT
