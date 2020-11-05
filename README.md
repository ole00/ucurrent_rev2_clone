# ucurrent_rev2_clone

A cheap clone of uCurrent revision 2. 


![Board image](https://github.com/ole00/ucurrent_rev2_clone/raw/main/img/ucurrent_rev2_clone.jpg "uCurrent rev2 clone")

Here are gerbers and a CAD file for uCurrent rev. 2 as originally presented
in Silicon Chip magazine 2009/04 and also on alternatezone web site:

http://www.alternatezone.com/electronics/ucurrent/

The reasons for producing this cone were as follows:
* I could not buy the product anymore (available only in Australia)
* I could not find the original rev. 2 gerbers
* An enhanced Gold version of uCurrent was available, but it seemed a bit more
  complicated to build and also a bit more expensive.
* I could not find some replacement parts in Europe (like the box/case and the exact 
  10 mOhm shunt resistor), therefore had to accomodate few small changes

## Changes
* double sided PCB with a single silk screen: dirt cheap to manufacture  
* uses a bit different case/box, just purely to get a cheap localy available replacement
* uses an alternative 10 mOhm shunt resitir with lower tollerance (1% only), but
  has a bit higher power parameter (1W at 70 deg. C, original is 0.5W part). Another
  option is to use 1.5 W resistor of the same series.
* top mounted LED: wanted to re-use some of my 0805 (or 0603) diodes in my junk box and
  did not want to spend extra for reverse mounted LED.
* the LED uses 1K resistor rather than 470R

## BOM
I bought the components mainly in RS-Components, just because it was convenient (
not cheapest though, I'm sure you can optimise the costs when bought elsewhere).

<pre>
Rs Stock  Description                                     Units
1920789   Plastic enclosure Z70 ABS                           1
7599403   LMV321AS5X Op Amp SOT23-5                           1
1546145   Switch Slide DP3T, JS203011CQN                      2
7861102   MAX4239ASA+ Op Amp SOIC8                            1
1854719   CR2032 holder                                       1
6624236   TPS3809L30DBVT Volt Supervisor SOT23                1
1929802   CMK-R010-1.0 Resistor ISA-PLAN 1206 R010 1% 1206    1
6621000   ERA6APB753V Resistor 75k 0805 0.1%                  1
6620603   ERA6ARB243V Resistor 24K 0805 0.1%                  1
.. TBC ..

</pre>
