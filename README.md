# M901D · Unsorted

Ward-Beck Systems M901D, 1995|28. Wiki page: [M901D on WBSps.ca](https://wardbecksystems.github.io/WBSps.ca/PAGES/M901D.html)

| Folder | What is in it | Files |
|---|---|---|
| [SCHEMATICS/](SCHEMATICS/) | electrical drawings: schematics, functional diagrams, component layouts, wiring | 1 |
| [MECHANICAL/](MECHANICAL/) | front panels, cover plates, metalwork, assemblies; the front panel as vectors | 1 |
| [PINOUTS/](PINOUTS/) | the RTO-144 connector: connection sheets, connector layouts, rear views | 3 |
| [MANUALS/](MANUALS/) | manuals, manual pages, price lists, brochures, documents | 3 |
| [PHOTOS/](PHOTOS/) | photographs of the module | 1 |
| [SOFTWARE/](SOFTWARE/) | program listings, firmware, the plugin | 1 |
| [KICAD/](KICAD/) | KiCad schematics traced from the drawings, the symbol, PCB projects | 2 |
| [OCR/](OCR/) | the note of every file: date, origin, title block, OCR text | 2 |

<!-- module data: tools/module_specs.py, tools/forum_quotes.py -->

**On the WBSps forum (2006|39 - 2014|47):** [1 topic](FORUM.md): what owners and technicians said about it.

## Circuit description

From [1995 - M901D - 901-01-006 - COMPONENT LAYOUT.wp](MANUALS/1995%20-%20M901D%20-%20901-01-006%20-%20COMPONENT%20LAYOUT.wp) page 1 (read by OCR; check against the pages). As data: [`CircuitDescription.json`](CircuitDescription.json).

<details><summary>Read it</summary>

Configuration Jumper Table 5 Parts List 5-1 to 5-15 6 P1,P2 Connector Layouts 6-1 to 6-2

7 Drawings:

Front Panel Layout B 901-04-008 Functional B 901-01-006 Schematic B 901-02-011/1 Schematic B 901-02-011/2 Schematic B 901-02-011/3 Component Layout B 901-06-004 Input Sensitivities

Line: -10 to +10 dBu.

Mic: -68 to -24 dBm (150 ohms).

Mic Padded to Line: 0 to +10 dBu.

Frequency Response +/-0.25 dB from 20 Hz to 20 kHz.

Noise

Line: Greater than 82 dB signal to noise ratio for +4 dBu input sensitivity.

Mic: -125 dB EIN at -60 dBm sensitivity.

(measured over 20 Hz to 20 kHz bandwidth)

Harmonic Distortion

Less than 0.15% from 20 Hz to 20 kHz attest level.

Less than 0.03% at 1 kHz attest level.

Source Impedances

Line: 600 ohms or less, balanced/unbalanced.

Mic: 150 ohms, balanced/unbalanced.

Input Impedances

Line: Greater than 20000 ohms, balanced.

Mic: Greater than 1500 ohms, balanced.

Output Impedances Less than 60 ohms at insert and direct outputs.

Load Impedances 10000 ohms or greater, balanced.

Output Level -6 dBu (nominal) unbalanced.

Power Requirements +/-24 volts dc. 120 mA nominal.

Ambient Temperature: 0 to 50 degrees Celsius.

Dimensions: 1.5&quot; wide x 16.2&quot; high x 6.6&quot; deep.

(38 mm x 410 mm x 168 mm)

Weight: 560 grams (1.25 lbs.).

The M901D is a cost effective module for the Renaissance series of radio consoles. Two microphone and two line amplifiers can be configured to provide a single stereo or two mono microphone inputs, or two stereo line inputs.

The input source selector allows two separate stereo inputs to be connected to the input module. Each input has it's own preamplifier, allowing individual sensitivity trimming of the discrete source inputs.

The sensitivity controls are front panel accessible. These continuously variable controls provide adjustment for microphone input sensitivities from -68 to 24 dBu, and line sensitivities from -10 to +10. When microphone preamplifiers are used as line amps; the input sensitivity range is 0 to +10 dBu.

Solid-state switching after the preamplifiers allows low noise source selection. The source selection is then routed to the module connector for insertion of optional processing.

The cue bus feed is connected to the insert return line so that pre-fade listening of source material can take place before any input module processing.

Direct left and right channel outputs are provided at the module connector. These direct feeds maybe optionally used for multitrack applications or to feed the console mix-minus system.

The output from this module maybe assigned to either of two stereo program buses.

The module also contains an assignable monophonic post VCA bus output. This bus is used by the console mix-minus system. Assignment to the mix-minus bus is via a front panel switch.

Unitary control of most module functions is also available at the module connector for machine control as well as external control inputs.

Outgoing control signals are furnished as open collector paths to control common when activated. Comprehensive internal module logic allows intelligent control of external machines, with all outgoing control signals following module source selection (source A or B).

A momentary closure to control common (through an open collector transistor), is provided when the module is turned on or off for both theA orB source. This totals four independent outputs, one start and stop signal for both theA and B module sources.

An additional sustained closure to common is provided for both theA and B input sources that is active when the main channel is on is also provided for external use. These outputs are also internally assignable to one or all of three internal console muting buses. These buses run to the M905 monitor modules in the console system for muting the monitor speakers.

The internal bus structure of the console also has a cue control bus. If a module is assigned to this bus, putting the module into cue will activate the auto cue function in the M905A control room monitor module.

The lamp internal to the channel off button is uncommitted and is brought out on the module connector. This is intended for utilization as a tally indicator for external machinery.

Module control inputs are also configured to activate when a closure to control common is provided. The module can be turned on and off, the cue can be toggled, and the source can be selected between A and B by simply grounding the appropriate module connector pin.

Program bus assignment is also possible external to the module. Again, a closure to control common will effect this assignment. to change a previous bus assignment, the electronic latches require clearing before loading them with new bus assignments. A closure to common will also perform this function. External control of the VCA within each module is also brought out to the edge connector. Application of a voltage between 0 and 5 volts DC will bring the attenuator from no external attenuation to full attenuation from the current fader position. This feature can be of benefit for automated cross-fading.

The M901D Input Module is packaged ina 1.5&quot; wide x 16.2&quot; high x 6.6&quot; deep.

This module derives its power from the console system bipolar +/-24 volt power supplies. 1) Source &quot;B Select

Depressing this momentary switch (SW4), enables the &quot;B&quot; input source and disables the &quot;A&quot; input source selection (if it was selected). Double pressing the active switch will cancel the selection.

2) Source &quot;A&quot; Select

Depressing this momentary switch (SW3), enables the &quot;A&quot; input source and disables the &quot;B&quot; input source selection (if it was selected). Double pressing the active switch will cancel the selection. This source is selected automatically when power is supplied to the module.

3) P1 Bus Assignment Switch

This electronically latched, momentary switch (SW2), assigns the stereo audio signal to the program 1 stereo mix bus. This assignment is performed automatically on module power up.

4) Mix-Minus Assign Switch

Depressing this alternate action switch assign's the module's output to the Mix-Minus Bus.

**5) Q**

This momentary electronic switch assigns the pre-fader signal to the console's stereo cue bus. This provides a pre-fade listen feed for cueing.

**6) OFF**

This switch turns off the audio feeds from the console mixing buses, and contains an externally accessible lamp for machine tally purposes.

**7) ON**

This momentary switch enables the audio feeds to the console mixing buses.

8) &quot;B&quot; Source Right Channel Sensitivity Control

This front panel accessible screwdriver trim control allows adjustment of the right channel microphone/line preamplifier sensitivity.

9) &quot;B&quot; Source Left Channel Sensitivity Control

This front panel accessible screwdriver trim control allows adjustment of the left channel microphone/line preamplifier sensitivity.

10) &quot;A&quot; Source Right Channel Sensitivity Control

This front panel accessible screwdriver trim control allows adjustment of the right channel line preamplifier sensitivity.

11) &quot;A&quot; Source Left Channel Sensitivity Control

This front panel accessible screwdriver trim control allows adjustment of the left channel line preamplifier sensitivity.

12) P2 Bus Assignment Switch

Switch SW5, a momentary switch controlling an electronic latch, actuates the assignment of the module output to the Program 2 bus in the console. 13) Main Channel Fader

This 105mm Penny and Giles linear fader controls the main channel voltage controlled amplifiers. Inputs

The M901D is capable of selecting between two stereo sources, two microphone inputs or two line inputs. By selectively configuring the inputs, it is possible to use the module to provide; a mono microphone and stereo line input, a stereo microphone and stereo line input, and two stereo line inputs. The table on the following page details the jumper configurations for various source possibilities.

The normal configurations are those which place the module edge connector inputs on their normal inputs on the source selector (i.e. the &quot;A&quot; inputs are line inputs and the &quot;B&quot; inputs are microphone inputs). Whereas the optional configuration places the &quot;B&quot; right input (on the edge card connector) on the &quot;A&quot; input source selector. The 'X' on the table details over which pins the shorting jumper should be placed.

The &quot;A&quot; input amplifiers comprised of U3 and U4 and associated components area balanced input differential amplifier with a 20 dB sensitivity range. Input levels of between -10 and +10 dBu can be adjusted to the system operating level of -6 dBu.

The &quot;B&quot; input amplifiers are single chip balanced microphone preamplifiers. The input circuit consists of common mode resistors R39 and R40 for U5 and R51 and R52 for U6 which allow the simplexing of phantom power on condenser microphones, depending on configuration by jumpers LK7 and/or LK8. The jumpers at U5; LK28 and LK29 (LK30 and LK31 for U6), area loss network for using the B inputs as line inputs. In addition to this fixed loss network, again change is also implemented with LK10 and L11 for realizing the line input configuration. An additional loss network on the output of each &quot;B&quot; preamplifier further augments the line input capabilities of the preamplifiers. Zener diodes CR18 through CR25 act as hard limiters to transients generated when plugging and unplugging condenser microphones with phantom power supplied to the preamplifier. This protects the preamplifiers from damage.

On power application to the module, a reset circuit comprised of R14, CR7, C104, and C136 globally resets all of the logic circuitry on the module (see B 901-02-011/2). This reset signal directly sets the &quot;A&quot; source flip-flop in U1 and resets the &quot;B&quot; source latch on U1. This is the initial input source selection. Selection of the &quot;B&quot; source is enabled by closing SW4 to control common. Switch bounce is controlled by U29 sections E and F, a Schmidt trigger inverter. This clean switching signal is coupled to the toggle input of U1, and via CR3 to the reset input of the &quot;A&quot; latch. This connection provides electronic alternate action operation for the source selection.

By double switching the currently active switch, it too is disabled. The allows both sources to be turned off, a function not normally available with a mechanically interlocked switch.

External A orB source selection is available at edge card connector P2 pin 26 and pin 25 respectively. Selecting source &quot;A&quot; this way directly sets the &quot;A&quot; latch, and resets the &quot;B&quot;. The converse is also true.

Source selection is tallied via illumination in the associated pushbutton. For the &quot;A&quot; source, a logic 0 at tag A on R183 turns Q17 on. This transistor sources current to the base of Q16 through R181 and R182. This shorts out DS6 and prevents it from illuminating. The lamps are all connected in series and powered by a constant current source consisting of Q24 and R193 through R195. This source provides approximately 20mA of current for the series LED string. Illumination is performed this way to maintain constant current consumption no matter the number of lamps on in the LED string.

The source audio is switched into the node of U9 and U10 through U7 and U8, a pair of analog multiplexors. Integrated circuit U9 and U10 drive the insert outputs to a -6dBu level for the insertion of optional processing.

Attenuator

A linear attenuator, ATT1 (on drawing B 901-02-011/3), controls two voltage controlled amplifiers (VCA); U17 and U18.

The insert return audio is AC coupled to the non-inverting input of U17 through C65. The gain of U17 is controlled by the voltage present at pin 11, which is bypassed to control common by C119. Trim control R108 is used to adjust the gain cell symmetry to minimize VCA distortion. Trim adjustment of the control feed through is done with R106. Resistors R233 through R236, CR72 and CR73 and Q29 and Q30 area bipolar emitter follower to boost the current output abilities of the VCA.

U18 operates similarly, except R241 allows fine adjustment of the level balance between the left and right channels.

The VCA characteristic is tailored to give a familiar audio taper to the level adjustment with a control amplifier comprised of U25 and U26 and associated components.

Bus Assignment

Solid state active bus assignments are performed by U22 through U24. These switches are controlled by the control logic in the module, and are active when the channel is switched on, the fader is brought up from infinity, and when the bus has been assigned.

The Program 1 bus maybe assigned to either a &quot;speech&quot; ora &quot;music&quot; busby moving programming jumpers LK12 and LK13. The assignment to the mix-minus bus is controlled by front panel switch SW6. This alternate action switch controls the mix-minus bus assignment solid-state switch. It is imperative that jumper LK20 be in position 1-2, otherwise no mix-minus audio will be impressed on it's summing bus when the channel is on.

Channel Control Logic

Channel On

Momentary operation of the channel on switch SW7, will produce a negative going pulse at U11 pin 13, resulting indirectly setting one of the flip flops in U14. Alternatively, a momentary closure of P2 pin 44 to ground will have the same effect.

Once the flip flop is preset, it's output at pin 15 changes from logic 0 to logic 1. This enables the VCA control amplifier, the Channel On lamp, and the program assignment bus controls (U30 sections A and D, and CR62, CR65 and CR71).

An open collector transistor, Q5 or Q6 is latched on, again depending on source selection, when the channel is on. These outputs can be used for external muting and signalling functions and are capable of sinking 20mA to control common.

A logical OR is realized with CR43 through CR45, and CR46 through CR48. These OR gate inputs are assignable to the internal muting buses in the console through a series of user-programmable links; LK1 through LK7. Notice that source A can mute a different bus configuration that source B.

Turning the channel on also causes a momentary low impedance path to ground to be enabled via an open collector transistor. This is intended for machine control applications, and is logically steered to follow the input source selection. Transistors Q1 through Q4 handle this task, and are capable of sinking 20mA to control common.

Channel Off

Momentary operation of the Channel Off switch SW8, or momentary ground closure of the External Off control input at connector P2 pin 44 will result ina negative going pulse at U11 pin 11. This results ina direct reset of the &quot;A&quot; section of the flip flop U14. This produces a direct reset of the &quot;A&quot; section of U14, producing a logic 0 at pin 15. This disables the VCA amplifier, disables the bus switches and extinguishes the Channel On lamp.

A momentary closure to control common via an open collector transistor which follows source selection is available at module connector P2 pin 36 and P2 pin 35 for theA and B inputs respectively.

The lamp integral to the Channel Off switch is uncommitted and available at module connector P2 pins 45 and 46. This can be used for external machine tally purposes (CD ready indicators, for example).

In addition to the normal channel pushbutton off, operated by the Channel Off function detailed above, the channel output is also disabled whenever the channel attenuator is moved to the infinite position (∞). This disables the VCA control amplifier and the Program Bus switches. However, the tally lamps for Channel On, muting controls and bus assignment switches remain unaffected.

The B section of U14 is used to control the solid state cue switches. The flop-flop will change state each time a negative going transition occurs at pin 3 of U11. Consequently, with each input pulse, the Cue channel toggles on and off.

This alternate action can be invoked by either momentarily closing Cue switch SW1 (Q), or momentarily grounding the external Cue control input at module connector P2 pin 41.

The status of the Cue channel is indicated by DS3, integral to SW1.

An additional feature ensures that the Cue channel is switched off whenever the attenuator is moved into or away from the infinity position: regardless of the prior state of the cue channel. The control signal for this action is initiated by the change of state of the end of travel switch integral to the attenuator. The resulting level change is processed through U11 section C and D, U13, and U12C.

All logic control inputs are buffered to guard against switch bounce and spurious noise.

Power Supply Decoupling

Please refer to drawing B 901-02-011/3.

An active decoupling network consisting of Q25 through Q28, U28 and associated components decouple the ±24 volt power supply down to the ±18 volts, and +6 volts required for use in the module. CR51 and CR52 protect the module in the event of power supply reversal. Three terminal regulator U28 provides 6 volts nominal for utilization by the logic circuitry within the module. The -22 volt power supply is used to drive the LED current source. ATT1 Fader P&amp;G PGF3210

C1 Capacitor 0.1 uF/100 V Sprague K104K20X7RFVBWN C2 &quot; 0.1 uF/100 V &quot; &quot; C3 &quot; 0.1 uF/100 V &quot; &quot; C4 &quot; 0.1 uF/100 V &quot; &quot; C5 &quot; 68 uF/10 V ITT 68M10

C6 &quot; 68 uF/10 V &quot; &quot; C7 &quot; 22 pF Philips 638-10229 C8 &quot; 10 pF &quot; 638-10109 C9 &quot; 10 uF/25 V ITT 10M25

**C10 &quot; SOT**

C11 &quot; 10 uF/25 V ITT 10M25 C12 &quot; 10 pF Philips 638-10109 C13 &quot; 33 uF/16 V ITT 33M16 C14 &quot; 68 uF/10 V &quot; 68M10 C15 &quot; 68 uF/10 V &quot; &quot;

C16 &quot; 22 pF Philips 638-10229 C17 &quot; 10 uF/25 V ITT 10M25

**C18 &quot; SOT**

C19 &quot; 10 pF Philips 638-10109 C20 &quot; 10 uF/25 V ITT 10M25

C21 &quot; 10 pF Philips 638-10109 C22 &quot; 33 uF/16 V ITT 33M16 C23 &quot; 47 uF/50 V Philips 03590015 C24 &quot; 47 uF/50 V &quot; &quot; C25 &quot; 47 uF/50 V &quot; &quot;

C26 &quot; 47 uF/50 V &quot; &quot; C27 &quot; 47 uF/50 V &quot; &quot; C28 &quot; 47 uF/25 V ITT 47M25 C29 &quot; 47 uF/25 V &quot; &quot; C30 &quot; 220 pF Philips 638-03221

C31 &quot; 68 uF/10 V ITT 68M10 C32 &quot; 47 uF/50 V Philips 03590015 C33 &quot; 47 uF/50 V &quot; &quot; C34 &quot; 47 uF/50 V &quot; &quot; C35 &quot; 47 uF/50 V &quot; &quot; C36 Capacitor 47 uF/25 V ITT 47M25 C37 &quot; 47 uF/25 V &quot; &quot; C38 &quot; 220 pF Philips 638-03221 C39 &quot; 68 uF/10 V ITT 68M10 C40 &quot; 0.1 uF/100 V Sprague K104K20X7RFVBWN

C41 &quot; delete C42 &quot; 47 pF Philips 638-34479

**C43 &quot; SOT**

C44 &quot; 0.1 uF/100 V Sprague K104K20X7RFVBWN C45 &quot; 0.1 uF/100 V &quot; &quot;

C46 &quot; 47 pF Philips 638-34479 C47 &quot; 33 uF/16 V ITT 33M16 C48 &quot; 47 pF Philips 638-34479

**C49 &quot; SOT**

C50 &quot; 33 uF/16 V ITT 33M16

C51 &quot; 0.1 uF/100 V Sprague K104K20X7RFVBWN C52 &quot; 47 pF Philips 638-34479 C53 &quot; 0.1 uF/100 V Sprague K104K20X7RFVBWN C54 &quot; 0.1 uF/100 V &quot; &quot; C55 &quot; delete

C56 &quot; 0.1 uF/100 V Sprague K104K20X7RFVBWN C57 &quot; 0.1 uF/100 V &quot; &quot; C58 &quot; 1 uF/35 V ITT 1M35 C59 &quot; 0.1 uF/100 V Sprague K104K20X7RFVBWN C60 &quot; 1 uF/35 V ITT 1M35

C61 &quot; 0.1 uF/100 V Sprague K104K20X7RFVBWN C62 &quot; delete C63 &quot; 47 pF Philips 638-34479 C64 &quot; 22 uF/25 V Siemens 85200 C65 &quot; 10 uF/25 V ITT 10M25

C66 &quot; 150 pF Philips 638-70151 C67 &quot; 22 uF/25 V Siemens 85200 C68 &quot; 22 uF/25 V &quot; &quot; C69 &quot; 150 pF Philips 638-70151 C70 &quot; 10 uF/25 V ITT 10M25

C71 &quot; 22 uF/25 V Siemens 85200 C72 &quot; 47 pF Philips 638-34479 C73 &quot; 0.1 uF /100V Sprague K104K20X7RFVBWN C74 &quot; 10 uF/25 V ITT 10M25 C75 &quot; 0.1 uF /100V Sprague K104K20X7RFVBWN

C76 Capacitor 47 pF Philips 638-34479 C77 &quot; delete C78 &quot; delete C79 &quot; delete C80 &quot; delete

C81 &quot; delete C82 Capacitor 33 uF/16 V ITT 33M16 C83 &quot; delete C84 &quot; delete C85 &quot; delete

C86 &quot; delete C87 &quot; 33 uF/16 V ITT 33M16 C88 &quot; 0.1 uF/100 V Sprague K104K20X7RFVBWN C89 &quot; 0.1 uF/100 V &quot; &quot; C90 &quot; 0.1 uF/100 V &quot; &quot;

C91 &quot; delete C92 &quot; 0.1 uF/100 V Sprague K104K20X7RFVBWN C93 &quot; 0.1 uF/100 V &quot; &quot; C94 &quot; 0.1 uF/100 V &quot; &quot; C95 &quot; 0.1 uF/100 V &quot; &quot;

C96 &quot; 2.2 uF/20 V ITT 2.2M20 C97 &quot; 2.2 uF/20 V &quot; &quot; C98 &quot; 22 uF/25 V Siemens 85200 C99 &quot; 22 uF/25 V &quot; &quot; C100 &quot; 47 uF/25 V Philips 03556479

C101 &quot; 22 uF/25 V Siemens 85200 C102 &quot; delete C103 &quot; 1 uF/35 V ITT 1M35 C104 &quot; 47 uF/25 V Philips 03556479 C105 &quot; 47 pF Philips 638-34479

C106 &quot; delete C107 &quot; delete C108 &quot; delete C109 &quot; delete C110 &quot; delete

C111 &quot; 0.1 uF/100 V Sprague K104K20X7RFVBWN C112 &quot; 0.1 uF/100 V &quot; &quot; C113 &quot; 10 uF/25 V ITT 10M25 C114 &quot; 10 uF/25 V &quot; &quot; C115 &quot; 10 uF/25 V &quot; &quot;

C116 Capacitor 10 uF/25 V ITT 10M25 C117 &quot; 6.8 uF/16 V &quot; 6.8M16 C118 &quot; 6.8 uF/16 V &quot; &quot; C119 &quot; 0.33 Sprague 2C20X7R334M050B C120 &quot; 0.1 uF/100 V &quot; K104K20X7RFVBWN

**C121 &quot; 0.33 &quot; 2C20X7R334M050B**

C122 &quot; 0.1 uF/100 V &quot; K104K20X7RFVBWN C123 &quot; 0.1 uF/100 V &quot; &quot; C124 &quot; 0.1 uF/100 V &quot; &quot; C125 &quot; 0.1 uF/100 V &quot; &quot;

C126 &quot; delete C127 &quot; 33 uF/16 V ITT 33M16 C128 &quot; 33 uF/16 V &quot; &quot; C129 &quot; 10 uF/25 V &quot; 10M25 C130 &quot; 10 uF/25 V &quot; &quot;

C131 &quot; 10 uF/25 V &quot; &quot; C132 &quot; 10 uF/25 V &quot; &quot; C133 &quot; 10 uF/25 V &quot; &quot; C134 &quot; 10 uF/25 V &quot; &quot; C135 &quot; 10 uF/25 V &quot; &quot;

C136 &quot; 47 uF/25 V Philips 03556479 C137 &quot; delete C138 &quot; 0.1 uF/100 V Sprague K104K20X7RFVBWN C139 &quot; 82 pF Philips 638-58829

**C140 &quot; SOT**

C141 &quot; 82 pF Philips 638-58829 C142 &quot; 82 pF &quot; &quot; C143 &quot; 0.1 uF/100 V Sprague K104K20X7RFVBWN C144 &quot; 47 pF Philips 638-34479 C145 &quot; 47 pF &quot; &quot;

C146 &quot; 47 pF &quot; &quot; C147 &quot; 47 pF &quot; &quot; C148 to C154 &quot; 0.1 uF/100 V Sprague K104K20X7RFVBWN

CR1 Diode National 1N4148 CR2 delete CR3 to CR17 Diode National 1N4148 CR18 to CR25 &quot; &quot; 1N752A

**CR26 &quot; &quot; 1N4148**

CR27 Diode National 1N4003

**CR28 &quot; &quot; 1N4148**

CR29 Diode National 1N4003

**CR32 &quot; &quot; 1N4003**

CR33 to CR36 &quot; &quot; 1N4148 CR37,CR38 delete CR39 Diode &quot; 1N4003

**CR40 &quot; &quot; &quot;**

CR41 to CR48 &quot; &quot; &quot; CR49 delete CR50 Diode &quot; 1N4148

**CR52 &quot; &quot; &quot;**

CR53 to CR56 &quot; &quot; 1N4148 CR57 delete CR58 to CR70 Diode &quot; 1N4148 CR71 delete CR72 to CR75 Diode &quot; 1N4148

CR76 delete CR77 Diode &quot; 1N4003

**CR78 &quot; &quot; &quot;**

CR79 to CR85 &quot; &quot; 1N4148

DS1-DS6 LED, Yellow H.P HLMP1401 DS7 LED-T1, Red DS8 Lamp, Min Flange 387

LK1-LK20 Connector, 3 Pin, Male Berg 929705-01-03 LK21-LK22 delete LK23 Connector, 3 Pin, Male Berg 929705-01-03 LK24 delete LK25 PCB Link

LK26-LK31 Connector, 3 Pin, Male Berg 929705-01-03 LK32-LK37 PCB Link LK38 delete LK40-LK43 Connector, 3Pin Maale Berg 929705-01-03

Q1 to Q4 Transistor National 2N3904

**Q6 &quot; &quot; 2N6731**

Q7 Transistor National 2N3906

**Q8 &quot; &quot; 2N3906**

Q9 delete Q10 Transistor &quot; 2N3906 Q11 delete

Q12 Transistor National 2N3904

**Q32 &quot; &quot; 2N3906**

R1 SIP Resistor 10K Bourns 15-002 R2 SIP Resistor 39K &quot; 15-014 R3 Resistor 1/4W 5% 3K3 Philips CR25

**R5 &quot; &quot; 10K &quot; &quot;**

R6 &quot; &quot; delete

**R10 &quot; &quot; 3K3 &quot; &quot;**

R11 &quot; &quot; delete

**R18 &quot; 1/4W 1% 100K &quot; &quot;**

R19 Resistor 1/4W 1% 4K75 Philips MRS25F

**R20 &quot; 1/4W 1% 4K75 &quot; &quot;**

R21 Resistor SOT R22 &quot; 1/4W 5% 15K Philips CR25

**R23 &quot; &quot; 1K &quot; &quot;**

R24 Potentiometer 5K Piher PT10H 5K R25 Resistor 1/4W 5% 100K Philips CR25

R26 &quot; delete

**R35 &quot; &quot; 1K &quot; &quot;**

R36 Potentiometer 5K Piher PT10H 5K R37 Resistor 1/4W 5% 100K Philips CR25 R38 &quot; delete

**R46 &quot; &quot; 4.7 &quot; &quot;**

R47 Potentiometer 500 Piher PT10H 500 R48 delete R49 Resistor 1/4W 5% 2K2 Philips CR25

**R50 &quot; &quot; 470 &quot; &quot;**

R51 Resistor 1/4W 1% 6K81 Philips MRS25F

**R57 &quot; 1/4W 5% 4.7 &quot; CR25**

R58 Resistor 1/4W 5% 300 Philips CR25 R59 Potentiometer 500 Piher PT10H 500 R60 delete

R61 Resistor 1/4W 5% 2K2 Philips CR25

**R70 &quot; &quot; 100K &quot; &quot;**

R71 Resistor 1/4W 5% 22K Philips CR25

**R72 &quot; &quot; 100K &quot; &quot;**

R73 SIP Resistor 10K Bourns 15-002 R74 Resistor 1/4W 5% 3K3 Philips CR25

**R80 &quot; &quot; 39K &quot; &quot;**

R81 Resustor 1/4W 5% 27K Philips CR25

**R87 &quot; &quot; 15K &quot; &quot;**

R88 SIP Resistor 10K Bourns 15-002 R89 Resistor 1/4W 5% 15K Philips CR25

**R90 &quot; &quot; 100K &quot; &quot;**

R91 Resistor 1/4W 5% 15K Philips CR25

**R92 &quot; &quot; 10K &quot; &quot;**

R93 delete R94 delete R95 delete

R96 delete R97 Resistor 1/4W 5% 15K Philips CR25

**R99 &quot; &quot; 15K &quot; &quot;**

R100 &quot; &quot; delete

R101 Resistor 1/4W 5% 150K Philips CR25

**R103 &quot; &quot; 15K &quot; &quot;**

R104 delete

**R105 &quot; &quot; 10M &quot; &quot;**

R106 Potentiometer 100K Piher PT10V 100K R107 delete R108 Potentiometer 500K Piher PT10V 500K R109 Resistor 1/4W 5% 470K Philips CR25

**R110 &quot; &quot; 150K &quot; &quot;**

R111 Resistor 1/4W 5% 22K Philips CR25

**R112 &quot; &quot; 15K &quot; &quot;**

R113 delete

**R114 &quot; &quot; 10M &quot; &quot;**

R115 Potentiometer 100K Piher PT10V 100K

R116 delete R117 Potentiometer 500K Piher PT10V 500K R118 Resistor 1/4W 5% 470K Philips CR25

**R120 &quot; &quot; 20K &quot; &quot;**

R121 Resistor 1/4W 5% 20K Philips CR25

**R122 &quot; &quot; 100K &quot; &quot;**

R123 delete R124 delete

**R125 &quot; 1/4W 5% 100K &quot; CR25**

R126 delete R127 delete

**R128 &quot; 1/4W 5% 100K &quot; CR25**

R129 delete

**R131 &quot; 1/4W 1% 15K &quot; &quot;**

R132 delete

**R134 &quot; 1/4W 1% 15K &quot; &quot;**

R135 delete

R136 Resistor 1/4W 1% 15K Philips MRS25F

**R139 &quot; 1/4W 5% 20K &quot; CR25**

R140 &quot; delete

R141 delete R142 delete R143 Resistor 1/4W 1% 10K Philips MRS25F

**R147 &quot; 1/4W 1% 47K5 &quot; &quot;**

R148 &quot; delete R149 &quot; delete R150 &quot; delete

R151 Resistor 1/4W 1% 47K5 Philips MRS25F

**R153 &quot; 1/4W 5% 1K &quot; CR25**

R154 &quot; delete

**R160 &quot; 1/4W 1% 28K7 &quot; &quot;**

R161 Resistor 1/4W 1% 28K7 Philips MRS25F

**R169 &quot; 1/4W 5% 33K &quot; &quot;**

R170 to R174 delete

R175 Resistor 1/4W 5% 22K Philips CR25

**R179 &quot; &quot; 4K7 &quot; &quot;**

R180 Resistor 1/4W 5% 100K Philips CR25

**R190 &quot; &quot; 22K &quot; &quot;**

R191 Resistor 1/4W 5% 22K Philips CR25

**R200 &quot; &quot; 2.2 &quot; &quot;**

R201 Potentiometer 5K Piher PT10V 5K R202 Resistor 1/4W 5% 100 Philips CR25

**R205 &quot; 1/4W 1% 137 &quot; &quot;**

R206 &quot; delete

**R208 &quot; &quot; 100 &quot; &quot;**

R209 &quot; delete

**R210 &quot; SOT**

R211 Resistor 1/4W 5% 22K Philips CR25 R212 &quot; delete

**R213 &quot; 1/4W 5% 22K &quot; &quot;**

R214 &quot; delete R215 &quot; delete

R216 &quot; delete R217 &quot; delete R218 &quot; delete R219 &quot; delete R220 delete

R221 Resistor delete R222 &quot; 1/4W 5% 2K2 Philips CR25

**R230 &quot; &quot; 30 &quot; &quot;**

R231 Resistor 1/4W 1% 1K Philips MRS25F

**R240 &quot; 1/4W 5% 68 &quot; CR25**

R241 Potentiometer 5K Piher PT10V 5K R242 Resistor 1/4W 5% 16K Philips CR25

**R254 &quot; &quot; 100K &quot; &quot;**

R255 &quot; &quot; delete

**R258 &quot; &quot; 22K &quot; &quot;**

R259 Resistor 1/4W 5% 22K Philips CR25

**R264 &quot; &quot; 6.8 &quot; &quot;**

R265 Potentiometer 5K Piher PT10V 5K R266 Resistor 1/4W 5% 4K7 Philips CR25

**R287 &quot; &quot; 39K &quot; &quot;**

SW1 to SW5 Switch Licon 39-22100 SW6 A/A Switch &quot; SW7 Switch Dialco 554-3221-311

**SW8 &quot; &quot; 554-3221-211**

U1 Integrated Circuit National 74HC74N

**U3 &quot; &quot; &quot; LM833**

U5 &quot; &quot; Analog SSM2017P

U7 &quot; &quot; National 74HC4053N

U9 &quot; &quot; Signetics NE5534N

U11 &quot; &quot; National 74HC14N

**U15 &quot; &quot; &quot; 74HC125N**

U16 Integrated Circuit National 74HC125N U17 &quot; &quot; Analog SSM2018P

U19 &quot; &quot; Signetics NE5534N U20 &quot; delete

U21 &quot; delete U22 &quot; &quot; National 74HC4053N

**U25 &quot; &quot; &quot; LF353N**

U27 &quot; &quot; &quot; delete

</details>

<!-- /module data -->

## Manuals and documents

_Manuals and manual pages, price lists, RTO-144 connection sheets, brochures, ads and other document scans._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/12_b_N67PR0HXtjDcazOKS1eCKOyTSo4E/view" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=12_b_N67PR0HXtjDcazOKS1eCKOyTSo4E" width="240" alt="19xx - M901D - DOC - File_057.png"></a><br><sub>19xx - M901D - DOC - File_057</sub></td></tr>
</table>

## KiCad

_KiCad: a schematic (`.kicad_sch`) traced from each electrical drawing, the module symbol (`.kicad_sym`) and its PCB projects. Traced schematics are the line work only: redraw with symbols over them._

- [M901D.kicad_sym](KICAD/M901D.kicad_sym)
- [index.html](KICAD/index.html)

## Software

- [index.html](SOFTWARE/index.html)

---
Archive: Anthony Peter Kuzub · [WBSps.ca](https://WBSps.ca) · [WBSps.Kuzub.com](https://WBSps.Kuzub.com)
