# ARC-34 UHF Command Radio

## Introduction
<!-- Link the AN/AIC-10 Amp to its own page -->
The onboard radio, powered by the aircraft’s primary bus, enables voice communication within the 225.0 to 399.9 MHz frequency range. Audio signals are processed through the AN/AIC-10 communication amplifier. The system features a control panel with access to 20 preset channels, while also allowing manual frequency selection without altering any preset values.

This radio system employs two receivers: a primary receiver responsible for standard communications, and a guard receiver fixed to a dedicated emergency frequency. The guard frequency is factory-set and cannot be changed without removing the remote-control unit from the aircraft. When selecting a new frequency, an automatic tuning mechanism synchronizes both the transmitter and receiver, completing the tuning cycle in approximately four seconds.

## Controls

![radio image](./img/command_radio.png)

1. [Frequency Knobs](#frequency-knobs)
2. [Manual-Preset-Guard Sliding Selector](#manual-preset-guard-sliding-selector)
3. [Volume Control](#volume-control)
4. [Preset Channel Selector Switch](#preset-channel-selector-switch)
5. [Function Switch](#function-switch)
6. [Tone Button](#tone-button)
7. [Frequency Card](#frequency-card)

### Frequency Knobs

At the top of the radio panel, just below the four frequency display windows, are four small frequency selector knobs. Each knob, when turned, adjusts the numeral in its corresponding window, changing the overall frequency. This system allows manual selection of any of the 1,750 available frequencies within the 225.0 to 399.9 MHz range. The frequency 243.0 MHz is reserved as a guard channel.

### Manual-Preset-Guard Sliding Selector

The sliding selector controls the method of command radio frequency selection. It is operated by sliding the control through a limited arc across the face of the panel. This control has three positions, **MANUAL**, **PRESET**, and **GUARD**, and is arranged so that when it is in any one position, the other two positions are masked by a semitransparent green glass.

| Selection  | Description |
|------------|-------------|
| **MANUAL** | The preset channel is deactivated and a mask is removed from in front of the four small windows across the top of the panel, revealing the numerals that make up an operating frequency set by the [frequency knobs](#frequency-knobs). |
| **PRESET** | Masks the 4 small windows above the [frequency knobs](#frequency-knobs) and deactivates the manually selected frequency. This activates the [20 preset channels](#default-preset-channels) controlled by the channel selector switch. |
| **GUARD**  | Automatically tunes the transmitter and main receiver to the default guard frequency 243.0 MHz. |

### Volume Control

The volume control regulates the sound level of the signal being heard in the headphones from both command receivers. Adequate control of volume is provided, but the volume may not be reduced below a fixed level.

### Preset Channel Selector Switch

The channel selector switch controls the selection of [20 preset frequencies](#default-preset-channels) by channel number. When the switch is rotated, channel numbers from 1 through 20 appear in the channel indicator window, above the selector. This window is masked when the [sliding selector control](#manual-preset-guard-sliding-selector) is placed in any position other than **Preset**.

### Function Switch

Rotating the command radio function switch from **OFF** turns the command radio on. When the switch is at **MAIN**, only the main receiver is audible in the headphones. In the **BOTH** position, the guard receiver and the main receiver are heard simultaneously. The **ADF** position is operable only with the ADF system and will disconnect the signal from the AN/ARN-6.

<!-- Perhaps we should better describe the ADF operation?? -->
| Selection | Description |
|-----------|-------------|
| **OFF**   | The radio is inoperative |
| **MAIN**  | Only the main receiver is audible in the headphones. |
| **BOTH**  | The guard receiver and the main receiver are heard simultaneously in the headphones. |
| **ADF**   | Direction finding is enabled and will disconnect the signal from the [AN/ARN-6 Radio Compass](../ARN-6%20Radio%20Compass/radio-compass.md). |

### Tone Button

When the command radio is operating, a continuous tone signal may be transmitted by pressing the tone button. This occurs on the frequency that is set on the transmitter, and it interrupts reception. A side tone is audible in the headphones while the button is depressed. This feature may be used for direction-finding operations in conjunction with other airplanes and ground stations.

### Frequency Card

![freqcard](./img/freqcard.png)

## Remote Channel Indicator

![radio image](./img/remote-channel-indicator.png)

<!-- IDK where I should put this yet... -->
The remote channel indicator is synchronized to the command radio control panel. The face of the indicator has four windows for display of channel number and frequency. When the [selector control](#manual-preset-guard-sliding-selector) is at **PRESET**, two of the indicator windows are used to display the number of the preset command radio channel. When the selector control is at **MANUAL**, the four indicator windows display the frequency (in MHz) of the selected channel. With the selector control at **GUARD**, the two center windows show the letters "GD". All indicator windows are blank when power is off.

## Default Preset Channels
<!-- NOTE: There is an invisible character used to space the table -->
| Preset Channel | Frequency (MHz) |⠀⠀⠀⠀| Preset Channel | Frequency (MHz)  |
|:--------------:|:---------------:|:---:|:--------------:|:---------------: |
| Channel 1      | 225.0           |     | Channel 11     | 235.0            |
| Channel 2      | 226.0           |     | Channel 12     | 236.0            |
| Channel 3      | 227.0           |     | Channel 13     | 237.0            |
| Channel 4      | 228.0           |     | Channel 14     | 238.0            |
| Channel 5      | 229.0           |     | Channel 15     | 239.0            |
| Channel 6      | 230.0           |     | Channel 16     | 240.0            |
| Channel 7      | 231.0           |     | Channel 17     | 241.0            |
| Channel 8      | 232.0           |     | Channel 18     | 242.0            |
| Channel 9      | 233.0           |     | Channel 19     | 243.0            |
| Channel 10     | 234.0           |     | Channel 20     | 244.0            |

## Normal Operation

A complete operational check of the command radio may
be made as follows:

1. Before takeoff, check frequencies to be used against
those listed on [frequency card](#frequency-card).

2. Check settings of buttons on frequency control drum
with frequency card. To do this, open door to which frequency card is attached. The channel number which corresponds to the preset frequency appears in a window at the left of the buttons. The frequency numbers of this channel are listed above the buttons.

3. Check operation of transmitter and main receiver with [sliding selector control](#manual-preset-guard-sliding-selector) in each position.

4. Check operation of the guard receiver using the BOTH position of [function switch](#function-switch).

5. For initial channel selection, select a channel other than the one to be used until warm-up is completed, or after warm-up, switch to another channel and then back to the one desired. If the desired channel is selected before warm-up is completed, reduced performance due to mistuning may result.

6. Adjust [volume](#volume-control) as desired.

7. For manual selection of a frequency that is not included in the preset channels, moving [sliding selector control](#manual-preset-guard-sliding-selector) to MANUAL. Use frequency knobs across top of panel to establish desired frequency. (The function switch
must be at MAIN or BOTH for this operation.)

8. To obtain transmission and reception of guard frequency only, move [sliding selector control](#manual-preset-guard-sliding-selector) to GUARD, and turn [function switch](#function-switch) to MAIN. This will prevent unequal or garbled reception by cutting out the guard receiver that operates when the [function switch](#function-switch) is at BOTH.

## Emergency Operation

### Sudden Loss of Transmission and Reception

If transmission or reception is unsatisfactory, adjust aircraft attitude or heading to improve line-of-sight alignment with the antenna.

### Channel Selection After Engine Shutdown

If it is necessary to select another frequency channel, selection should be done as soon as possible after engine shutdown or engine failure, so that
electrical power is available to complete selection.

### Radio Not Operating

In the case of apparent failure of command radio, attempt operation in alternate positions of [sliding selector control](#manual-preset-guard-sliding-selector) and/or alternate positions of [function switch](#function-switch). Turn equipment off for several minutes; then turn [function switch](#function-switch) to type of operation desired. If the protective relay in the tuning mechanism was responsible, this action will restore operation. Check circuit breaker panel for tripped condition of the AN/AIC-10 amplifier.
