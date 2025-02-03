# 12V to 5V 2A Flybuck-Converter
This PCB is based on the recommended layout from the LMR36520 documentation, with components from the associated evaluation board. 

The LMR36520 is an adjustable buck regulator with an input range between 12V and 24V for normal usage, but supporting 6V-60V transients, at an output of up to 2A. In the configuration laid out in this repository, the board will output at 5V up to 2A. However, the output voltage can be easily adjusted by changing the RFBT resistor based on the documentation of the LMR36520, which will be linked below. 

RFBT1 & RFBT2 are wired in series, parallel to RFBT, to allow an alternative way to set the desired output voltage by varying resistances. 

Due to the high heat output of converting to 5V 2A, I will use 2oz of copper weight on the outer layers to allow for greater heat dissipation. I will also be adding external heatsinks attached via thermal pads to the front and back to further improve heat dissipation. 

The large amount of unused board is to allow for a greater ground plane to improve head dissipation, and also to spread out components so hand soldering is easier. While this design is only 2 layers, it may worth it to increase it to 4 layers for more heat dissipation, with both center layers used as extended ground planes. However, I chose against this due to the increased cost.

As of 03/02/2025 this design is untested, I will update this repository when I have had the PCB produced and tested the design. 

I will be ordering this PCB from JLCPCBs and the components from Digikey. 

# Development Images:

![PCB Top Layer](https://github.com/Billy5691-2/Buck-Converter/blob/main/PCB_Top.jpg?raw=true)

![PCB Bottom Layer](https://github.com/Billy5691-2/Buck-Converter/blob/main/PCB_Bottom.jpg?raw=true)


# Components:
Buck: 
Texas Indstruments - LMR36520ADDAR

Inductor:
TDK Corporation -SPM10065VT-100M-D
10uH, 8.1A


CIN1, CIN2:
TDK Corporation - CGA6M3X7S2A475K200AB
4.7uF, 100V

CVcc:
TDK Corporation - C1608X5R1E105K080AC
1uF, 25V

CVBoot:
KYOCERA AVS - KGM15BR71E104KT
0.1uF, 25V

CO1, CO2, CO3:
Samsung Electro Mechanics - CL32A226KAJNNNE
22uF, 25V

CHF1:
Murata Electronics - GRM21AR72A224KAC5L
0.22uF, 100V

CINB:
Panasonic Electronic Components - EEE-TG2A220UP
22uF, 100V

RFBT:
YAGEO - RC0603FR-07100KL
24.9K Ohm

RFBT (3.3V Recommended Alternative): 
YAGEO - RC0603FR-0746K4L
46.4k Ohm

RFBB:
YAGEO - RC0603FR-0724K9L
100K Ohm

Barrel Jack:
Kycon - KLDX-0202-BC
2.5mm-5.5mm, Positive Center

#References:
LMR36520:
https://www.ti.com/lit/ds/symlink/lmr36520.pdf

LMR36520EVM:
https://www.ti.com/lit/ug/snvu677/snvu677.pdf

Inspiration:
https://www.instructables.com/DIY-High-Efficiency-5V-Output-Buck-Converter/


