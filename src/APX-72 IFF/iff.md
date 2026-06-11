# AN/APX-72 IFF AIMS System

## Introduction

The AIMS system, which utilizes an AN/APX-72 receiver/transmitter (transponder), is used to automatically identify the airplane in response to coded interrogations. Depending on interrogation mode, the reply is transmitted in modes 1, 2, 3/A, 4, or airplane altitude reporting in mode C.

<!-- REWORD THIS AND FIGURE OUT WHERE TO PUT IT!!! -->
!!! note
    Due to engine limitations, the settings on the panel have no effect in DCS. However, they are exposed to external tools, such as SRS.

## Controls

![iff image](./img/iff.png) <!-- REPLACE THIS IMAGE -->

<!-- Master Switch Mode Selection Switch Test Switches code selectors mode 1 code selectors mode 3A mode 4 enable switch mode 4 code select switch -->

1. [Mode 4 Function Switch](#mode-4-function-switch)
2. [Master Switch](#master-switch)
3. [Reply Light](#reply-light)
4. [Test Light](#test-light)
5. [Mode 4 Indication Switch](#mode-4-indication-switch)
6. [Mode Selection Switches](#mode-selection-switches)
7. [Monitor-Radiation Test Switch](#monitor-radiation-test-switch)
8. [Mode 4 Selector Switch](#mode-4-selector-switch)
9. [Identification Switch](#identification-switch)
10. [Mode 1 Code Selectors](#mode-1-code-selectors)
11. [Mode 3/A Code Selectors](#mode-3a-code-selectors)

### Mode 4 Function Switch

The mode 4 CODE selector has the following positions:
| Selector Position | Function
|-------------------|---------
| A                 | Code A
| B                 | Code B
| HOLD              | Provide a means of retaining the mode 4 code for an additional flight (unless intentionally retained, the code is automatically returned to zero when power is removed after landing)
| ZERO              | Manually zeroize mode 4 code

!!! note
    The mode 4 code selector knob must be pulled out to be moved to ZERO.

### Master Switch
| Master Switch Position | Function
|------------------------|---------
| OFF                    | System off
| STDBY                  | Powered on, in standby
| NORM                   | Normal receiver sensetivity
| LOW                    | Low receiver sensitivity
| EMER                   | Activates emergency operation.

!!! note
    The master switch knob must be pulled out to be moved to the EMER position.

### Reply Light

When the transmitter-reciever responds properly to a mode 4 interrogation, the mode 4 REPLY light (green) illuminates.

### Test Light

A green TEST light illuminates to indicate proper operation of each tested mode during the self-test, or when the (radiation) monitor switch is set to the MON (monitor) position.

### Mode 4 Indication Switch

The audio/light switch has been moved from OFF to AUDIO or LIGHT (no audio signal provided).

### Mode Selection Switches

The mode selection switches M-1, M-2, M-3/A, and M-C have three positions:

| Mode Selection Switch Positions | Function
|---------------------------------|---------
| TEST (forward, momentary)       | Initiates a self-test of the mode (provided the airborne test set is installed)
| ON (center)                     | 
| OUT (aft)                       | 

### Monitor-Radiation Test Switch

The RAD TEST position is used by maintenance personnel during ground checks. In flight, leave this switch in the OFF position.

### Mode 4 Selector Switch

Mode 4 is selected by placing the mode 4 enable switch from OUT to ON. Mode 4 codes are preset in the mode 4 computer prior to missions via a code changer key.

### Identification Switch

The identifier switch enables transmission of identification of position (I/P) signals in response to interrogations in modes 1, 2, or 3/A, for 15-30 seconds. Transmission of I/P signals can be accomplished in three ways:

- When the switch is momentarily placed in the IDENT position
- When the switch is at MIC and the microphone button is momentarily pressed
- When the switch is at MIC and the command radio tone button is pressed (while command radio is on)

### Mode 1 Code Selectors

The two mode 1 selectors provide 32 possible code selections.

### Mode 3/A Code Selectors

The four mode 3/A selectors provide for 4096 code selections.

## Normal Operation

_Information forthcoming._
