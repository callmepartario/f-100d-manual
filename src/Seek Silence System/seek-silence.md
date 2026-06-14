# Seek Silence System

## Introduction

The seek silence system permits either normal operation of the [AN/ARC-34 command radio](../ARC-34%20Command%20Radio/command-radio.md) or decoding and coding of voice communications through the command radio. The decoding and coding capability prevents interception of messages when required. The system is powered by the primary bus.

## Controls

![seek silence image](./img/seek_silence.png) <!-- REPLACE THIS IMAGE -->

1. [Power Switch](#power-switch)
2. [Function Switch](#function-switch)
3. [Function Indicator Lights](#function-indicator-lights)
4. [Retransmit Switch](#retransmit-switch)
5. [Zeroize Switch](#zeroize-switch)

### Power Switch

When the power switch is moved from **OFF** to **ON**, power is applied to the seek silence system. The command radio can be operated in the normal manner with the power switch at **OFF**.

### Function Switch

The function switch controls decoding and coding of command radio voice reception and transmission.

| Selection        | Description |
|------------------|-------------|
| **PLAIN**        | Normal operation of the command radio is available, and only uncoded reception and transmission possible. |
| **C/RAD 1**      | The system decodes incoming voice communications, and codes outgoing voice communications through the command radio. |
| _C/RAD 2 (INOP)_ | Inoperable in this simulated F-100D. A mechanical stop prevents the switch from being moved to this position. |

### Function Indicator Lights

Three dimmable, press-to-test type lights indicate the position selected by the [function switch](#function-switch). With power applied to the system, the left (green) light comes on when the **C/RAD 1** position of the function switch is selected; the middle (amber) light comes on when the **PLAIN** position of the function switch is selected.

*The right (green) light is inoperative on these aircraft.*

### Retransmit Switch

This switch has no function in these aircraft. The switch should always be aft (**OFF**), regardless of the position of the function switch.

### Zeroize Switch

The zeroize switch is guarded in the normal, aft **OFF** position. If it becomes necessary to eject, the guard should be raised and the switch held momentarily at the forward **ON** position. This zeros out the ground set codes in the seek silence system.

## Normal Operation

1. Turn the [command radio](../ARC-34%20Command%20Radio/command-radio.md) **ON**. (Refer to Normal Operation of Command Radio.)
2. Move the [power switch](#power-switch) to **ON**.
3. Turn the [function switch](#function-switch) to **PLAIN** and establish communications through normal transmission procedures where possible.
4. Turn the [function switch](#function-switch) to **C/RAD 1** and listen for a steady unbroken tone in the headphones for approximately 2 seconds, followed by a double-pitched broken tone. If a prolonged steady tone is audible, it indicates an improper code setting or equipment malfunction, and the [function switch](#function-switch) should be turned to **PLAIN** and the [power switch](#power-switch) should be turned to **OFF**.
5. Press and hold the mic button for several seconds, then release. The double-pitched broken tone should stop and no further sound is heard in the headphones. If the broken tone continues, press mic button again and hold for several seconds. If the broken tone continues after three such attempts to clear it, move the [function switch](#function-switch) to **PLAIN** and [power switch](#power-switch) to **OFF**.
6. Press and hold the mic button. Wait ½–2 seconds for a single beep tone in the headphones. If beep tone is not heard, press mic button again and wait ½–2 seconds. If beep tone still is not heard, move [power switch](#power-switch) to **OFF** and then to **ON**, and repeat steps 5 and 6. If this fails to produce the beep tone, turn [function switch](#function-switch) to **PLAIN** and [power switch](#power-switch) to **OFF**.
7. When beep tone is audible, begin transmission.
