# 12V to 5V 2A Flybuck-Converter
. The PCB is based on the recommended layout from the LMR36520 documentation, with components from the associated evaluation board. 

The LMR36520 is an adjustable buck regulator with an input range between 12V and 24V for normal usage, but supporting 6V-60V transients, at an output of up to 2A. In the configuration laid out in this repository, the board will output at 5V up to 2A. However, the output voltage can be easily adjusted by changing the RFBT resistor based on the documentation of the LMR36520, which will be linked below. 

RFBT1 & RFBT2 are wired in series, parallel to RFBT, to allow an alternative way to set the desired output voltage by varying resistances. 

#Components:
U3: 
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


