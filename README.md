# ucurrent_rev2_clone

A cheap clone of uCurrent revision 2. 


![Board image](https://github.com/ole00/ucurrent_rev2_clone/raw/main/img/ucurrent_rev2_clone.jpg "uCurrent rev2 clone")

Here are gerbers and a CAD file for uCurrent rev. 2 as originally presented
in Silicon Chip magazine 2009/04 and also on alternatezone web site:

http://www.alternatezone.com/electronics/ucurrent/

The reasons for producing this clone were as follows:
* I could not buy the product anymore (available only in Australia)
* I could not find the original rev. 2 gerbers
* An enhanced Gold version of uCurrent was available, but it seemed a bit more
  complicated to build and also a bit more expensive.
* I could not find some replacement parts in Europe (like the box/case and the exact 
  10 mOhm shunt resistor), therefore had to accomodate few small changes

## Changes
* double sided PCB with a single silk screen: dirt cheap to manufacture  
* uses a bit different case/box, just purely to get a cheap localy available replacement
* uses an alternative 10 mOhm shunt resistor with lower tollerance (1% only), but
  has a bit higher power parameter (1W at 70 deg. C, original is 0.5W part). Another
  option is to use 1.5 W resistor of the same series.
* top mounted LED: wanted to re-use some of my 0805 (or 0603) diodes in my junk box and
  did not want to spend extra for reverse mounted LED.
* the LED uses 1K resistor rather than 470R

## BOM
I bought the components mainly in RS-Components, just because it was convenient (
not cheapest though, I'm sure you can optimise the costs when bought elsewhere).

<pre>
Seller  StockId   Description                                     Units
RS      1920789   Plastic enclosure Z70 ABS                           1
RS      7599403   LMV321AS5X Op Amp SOT23-5                           1
RS      1546145   Switch Slide DP3T, JS203011CQN                      2
RS      7861102   MAX4239ASA+ Op Amp SOIC8                            1
RS      1854719   CR2032 holder                                       1
RS      6624236   TPS3809L30DBVT Volt Supervisor SOT23                1
RS      1929802   CMK-R010-1.0 Resistor ISA-PLAN 1206 R010 1% 1206    1  R1
RS      6620495   ERA6ARB103B Resistor 10K 0805 0.1%                  1  R2
RS      6621000   ERA6APB753V Resistor 75K 0805 0.1%                  1  R3
RS      6620833   ERA6APB102V Resistor  1K 0805 0.1%                  2  R4, R5
Farnell 1469860   CRCW0805100KFKEA Resistor 100K 0805 1%              2  R6, R7
RS      6662358   CPF0805B10RE Resistor 10R 0805 0.1%                 1  R8
RS      6620603   ERA6ARB243V Resistor 24K 0805 0.1%                  1  R11
RS      1985684   RT0805FRE07100RL Resistor 100R 0805 1%              3  R9, R10, R12
RS      7007897   SML-211DTT86 LED Orange 1.8V 0805                   1
Rs      6480957   C0805C104K4RACTU Capacitor 100nF 0805 10% 16V       3  C1, C2, C3
Ebay    Speaker Terminal Binding Post For 4mm Banana Plug Socket      4
Ebay    Self tapping screws 2.9x8mm (Size No 4)                       2
Any     CR2032 battery                                                1


Notes / Optional parts:
RS      1929967  VMK-R010-1.0-U Resistor 0.01R 1% 1206 1.5W           1  R1 replacement
R4 can be replaced by any 0805 resistor of 470 - 1k value, 1 - 5 %    1  R4 replacement
R6, R7 might be cheaper to buy on Ebay due to lower shipping costs
LED - any 0805 led with Forward voltage around 2V should work
Male M3 Hex Hexagonal Brass Pillars PCB Threaded Standoff 13mm + 6mm  2 From Ebay
M3 Bolts black 7mm length, head matching the self tapping screws      2 From Ebay

</pre>

## Assembly
solder the parts in the following order:
* ICs (U1, U2, U3)
* passives except LED
* battery holder
* bannana plug solder tags (cut them to size first)
* LED on the top side of the PCB
* slide switches (ensure the CK letters are facing the top ebge of the PCB)
* optionally install extra 2 standoffs into the case. You might need to
  heat the standoffs to help to melt the case a bit while screwing them in.
  Check the standoff_detail.jpg in the img directory.

## Notes
* The original unaltered documentation in PDF format is located in the doc directory.
  It contains additional information and schematic.
* The design file can be modified in gEDA PCB CAD software. It is a free 
  and multiplatform tool. http://pcb.geda-project.org/
* The gerbers zip file can be uploaded to most of the cheap asian online manufacturing
  services without modifications. It is a dual layer PCB, 1.2 or 1.6 mm thickness. 
  Please DO NOT use Red color to clearly distinguish this is a clone.

