---
hide: footer
---

# Pneumatic Protocol
###### Author
Beth Fallon

###### Updated
15 February 2018

##### Background Information
Pneumatic protocol for measuring stem embolism and developing xylem vulnerability curves

This method uses vacuum pressure to extract air, presumed to be in the xylem and the result of embolism, from leafy stem section. This outlines 

1. The protocol for setting up an apparatus to measure differences in air volume present in stems and build a proxy hydraulic vulnerability curve 

2. The general measurement procedure.

### Full citation to methods

[Pereira, L, PRL Bittencourt, RS Oliveira, MBM Junior, FV Barros, RV Ribeiro, and P Mazzafera. 2016. Plant pneumatics: stem air flow is related to embolism – new perspectives on methods in plant hydraulics. New Phytologist. doi: 110.111/nph.13905](https://nph.onlinelibrary.wiley.com/doi/full/10.1111/nph.13905)

### Template

[Pneumatic Method Manual Datalog](https://docs.google.com/spreadsheets/d/1KXQ5IoYeEURCN-4k8t9gBN5yb6eKQsCu/edit?usp=sharing&ouid=117278050553426340443&rtpof=true&sd=true)

### Contents

##### Apparatus set-up and tests

1. Datalogger and transducer  

2. System volume  

3. Sealing connections  

4. Leak tests

##### Appendices

1. Pressure transducer voltage to pressure conversion  

2. Equations for calculating pressure, moles discharged, air discharged, percent air discharged  

3. Apparatus photos  

4. Campbell datalogger programming  

5. Concerns about the method

### Apparatus set-up and tests

##### Datalogger and transducer

1. Pressure transducer: the [Omega PX141-015V5V](https://drive.google.com/file/d/1_ybB1SnXFQ1c9aApZV3L332BRG0Jr9eg/view?usp=sharing)
    1. This reads only negative, or vacuum pressures, and should not be positively pressurized (beyond atmospheric) because the internal pressure plates can become deformed
    2. Wiring
        1. Voltage input should be 8V, deviation from this input can affect voltage out and this accuracy of conversion to a pressure unit
            1. Use a step down voltage regulator ([like this one sold on Amazon](https://drive.google.com/file/d/1X0DIMTM8Fni0Y4MAsWRFd85s_paWi7Mc/view?usp=sharing)) to convert higher DC voltage from a 12V input into 8V to the transducer
        2. Use a 3 prong connector (Omega CX136-3, push-on wire connector) to connect a positive wire into the connector and positive out. A single split grounding wire can be both the grounding in and out ([see p 4/5 of product documentation for wiring diagram](https://drive.google.com/file/d/1_ybB1SnXFQ1c9aApZV3L332BRG0Jr9eg/view?usp=sharing))
            1. These connectors are possibly crimpable for a connection with input/output wires, but I found that they needed to be soldered in place (to wire, not transducer) for a consistent connection
      
2. Campbell datalogger or other equivalent (currently using 850x)
    1. Datalogger is necessary for more accurate readings and timing of tests: 
        1. If you want three minutes, or x seconds, of pressure change for each individual measurement, the most exact method will be using a datalogger (paired with manual logs of approximate start and stop time) to find initial and final voltage (=pressure)
        2. The datalogger can log voltage out every second for a high resolution of change
    2. Software interface
        1. [PC200W datalogger software](https://www.campbellsci.com/pc200w) from Campbell Scientific
            1. Allows connection with any Campbell datalogger, writing and retrieving programs, monitoring and collecting data
    3. Collect air temperature and voltage out from the pressure transducer
        1. Use a simple copper-constantin thermocouple to monitor air T
        2. Use simple voltage connection ([see the program, Pneumatic_SEVolt_1seclog, for example](https://drive.google.com/drive/folders/1pjFq8a9TgTJv2Q2EqzRnib6gr15jHM8g?usp=sharing))
        3. Monitor and sample every second, be sure to collect data daily from logger because the logs are extensive and time consuming to download
      
3. Initial set up
    1. Install all wiring to the pressure transducer and connect to the datalogger
    2. Connect a computer to the datalogger using the PC200W software
        1. Use a Serial to USB connection and specify the connection port when connecting
    3. Make sure to Set the Clocks (right side of first PC200W tab “Clock/Program”) so that the computer and datalogger are synced
    4. Under the Collect data tab, select the first table of the program (should have set for 1 sec sample output of air temperature and voltage) and choose an output location. Unless otherwise desired, ensure the radio button to append new data (rather than overwrite) is selected
        1. I made a new output file each day to reduce file size
    5. Under the Monitor Data tab, select Add and Table 1 to see the time, temperature and voltage output
    6. In an unpressurized system, the voltage output should be the atmospheric pressure: the gage should read kPaatm/100=Vout.  

##### System volume

1. Measuring
    1. The effective reservoir for measurement is from the stem base to the pressure transducer, excluding the arm of the stopcock that is an outlet to the larger vacuum system. This is primarily the volume of the single piece of tubing (EW-30600-62 Cole Parmer, ID = 0.065” = 1.651mm, L = 24” = 609.6mm), but should include the volumes of all other components. 
    2. See the spreadsheet, “[Pneumatic_method_manual_datalog](https://docs.google.com/spreadsheets/d/1KXQ5IoYeEURCN-4k8t9gBN5yb6eKQsCu/edit?usp=sharing&ouid=117278050553426340443&rtpof=true&sd=true)” sheet “V_calc” for an example. Volume should be given in L (air discharged, AD, is calculated in uL).

1. Error in measures
    1. As the test reservoir increases in size, the ability to detect small changes in air discharge decreases (error rate of pressure gage is ±0.5% of span = .005 * 5V = 0.025V), see sheet in “[Pneumatic_method_manual_datalog](https://docs.google.com/spreadsheets/d/1KXQ5IoYeEURCN-4k8t9gBN5yb6eKQsCu/edit?usp=sharing&ouid=117278050553426340443&rtpof=true&sd=true)” “Reservoir error calc” to see impact of initial test reservoir size (
    2. Recommend keeping the size to 1 reservoir. Can detect a loss of 800uL of air from a stem and a minimum loss of 7uL
    3. If stem quickly loses more than the maximum capacity, can refill the vacuum and continue to extract—however large losses (in small stems) are as likely to be leaks as real air within the stem

##### Sealing connections

1. Multiple iterations of leak tests (see section 4, below) and sealing connections should be done in system preparation

2. Water can build up in the tubing (should be checked for water droplets in between measurements) and should be checked during measurements, so having permanent seals between reservoir tubing and transducer is not recommended. 

3. Teflon tape within and around all connections reduces most leakage

4. Closing the stopcock to the vacuum pump after initial depressurization reduces air entry within the larger system

##### Leak tests

1. Leak tests are best performed, and closest to general measurement set up, when using a sealed stem (gel superglue over cuts) clamped into silicone tubing and connect to the vacuum reservoir

2. Perform a leak test at the start of and end of testing (or multiple times throughout testing for more accuracy) for the same amount of time as stems are tested

3. It seems that small amounts of leakage are unavoidable, but can be limited to < 5uL air/3min. Care should be taken when taping connections and setting up the system to ensure that leakage is low
      
4. Using a simple cap and FtoF luer for initial system tests can show how much leakage there is without a stem in the system

### Measurements

1. Measure plants (height.bsd) before harvest

2. Stem harvest:20- 40cm of stem with at least 6 healthy leaves
    1. Mark stem with tape to ID
    2. Cut under water and place in floral tube with dH2O
    3. cover 1-2 leaves with saran wrap (to reduce transpiration) and then foil
    4. Cover with thick black plastic bag and let equilibrate for 1 hour.

3. Record for each sample
    1. include length and bsd of each test stem

4. Measure air pressure in lab
    1. with Barometer app (phone reads 97.5 when LiCor 6400 reads 97.25kPa)
        1. record at start and stop

5. Start transducer 
    1. Switch Campbell sci logger to on. 
    2. plug in transducer and make sure voltage out is at 8V (on display)
        1. Any swing away from an input voltage of 8V will affect voltage output 

6. Datalogger set 
    1. Append all existing data to datafile
    2. Resync datalogger to system clock (correct sec error) 
    3. Resend program (this must be done or mismatch in time will cause problems)

7. Transducer check
    1. With stem inlet stopcock open to all three flows (whole system at atmosphere), make sure that the voltage out is similar to current atmospheric pressure, ex.97V=97kPa

8. System vacuum and Measure system error:
    1. check all connections; add parafilm/Teflon tape to any adjusted connections
    2. With stem inlet stopcock all the way open (whole system at atmospheric pressure)
    3. Close stopcock to stem inlet and open 3-way stopcock at vacuum pump
    4. Depressurize to -4.2 -  -4kPa and close stopcock to vacuum pump, let stabilize
    5. System leakage
    6. measure 1-2 times/day as noted in Equipment section

9. Stem connections
    1. Keep stem in large black bag with damp paper towels in between all measure/dehydration steps
    2. Before removing from water, immediately remove a foil covered leaf and bag for water potential tests
        1. Glue cut
    3. Prep
        1. measure stem length and bsd
        2. Dry stem gently to remove excess water and make new clean cut with razor
        3. Insert into tight fit silicone tubing (using an ID 2-3mm smaller than stem diameter) and insert M to F luer  on opposite end of tube to almost stem end (to keep reservoir size uniform)
        4. Clamp tubing around stem (with a hose clamp or hand tightened zip tie)
        5. Glue stem, with latex glue, at silicone tubing 
        6. Teflon tape over female end of luer and hose clamp over connection
        7. Hook quickly to system

10. Measure
    1. Close stopcock to larger vacuum reservoir, so that it is open only between transducer and stem
    2. Record initial voltage as pressure after immediate drop (initial drop is due to air in the stem connection tube, since that isn’t under vacuum
    3. If using a datalogger
        1. Also record start time for analyses, with seconds
    4. Measure for 3-5 minutes
        1. I want three minutes, which on tests of Q. virginiana captured large losses, and after which losses were small, until they increased again likely due to dehydration during measurement
    5. Record final voltage and time
    6. Record room temperature near reservoir (or record this measurement once or twice a day if room temp is stable)
    7. Close stopcock to stem outlet and remove stem, let bench dry

11. Leaf water potential
    1. Leaves should be removed right before each stem measure (should have been foil covered) 
    2. Cut should be covered with latex glue
    3. leaves should be sealed in humid whirlpak bags
    4. measured water potential within a few minutes (before next stem measure)

12. Drying plants
    1. Record time dried on spreadsheet
        1. Some plants need only a few minutes to an hour to drop 1MPa in stem water potential
        2. Plants may need to dry overnight to reduce water potential
        3. Ideally, the AD~max~ is measured on a stem that has only a small amount of water escaping from the xylem (is almost fully dehydrated) but is measured before reaching the limits of the pressure chamber (-8MPa in my case)
    2. At start of drying, when stem exposed, wrap and foil cover another new leaf 
        1. Oaks seemed to perform better and more consistently in terms of increasing embolism with declining stem water potential when drying stem ends were loosely wrapped (not completely sealed) with parafilm. I have some concerns about formation of tyloses and perhaps a slightly more humid environment prevents that.
    b. After set drying time, place stem in humidified dark bag and let equilibrate for at least 30 minutes

### Appendix A: Pressure transducer voltage conversion

![alt text](images/pneumatic_1.png)

**Figure 1** the Omega vacuum gage pressure transducer PX141-015V5V does
not come with individual calibrations, but, when voltage in is 8V, the
conversion from voltage to pressure (absolute not vacuum) is 0psi at 1V
and -15psi at 6V. This conversion in kPa is as above. At atmospheric
pressure, the gauge should read <sub>kPa</sub>atm<sub>/100=V</sub>out~.

### Appendix B: Equations

The pneumatic method uses the amount air in the stem (removed by vacuum)
as a proxy for embolism. Drying down of the stem between measurements,
combined with measures of stem-equilibrated leaves, produces a Ψ by PAD
(percent air discharged) vulnerability curve.

##### Equations

1. Stem segment conductance, following (Tyree and Ewers 1991), where K equals the sum of individual conductance of each non-embolized vessel (Ki)

$$K = \sum K_i = (n-e)K_i=(n-e)\alpha D^4L^{-1}$$

<table>
<thead>
<tr class="header">
<th>Variable</th>
<th>Variable definition</th>
<th>Units</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><em>K</em></td>
<td>segment conductance</td>
<td>kg MPa<sup>-1</sup> s<sup>-1</sup></td>
</tr>
<tr class="even">
<td><em>n</em></td>
<td>number of vessels</td>
<td></td>
</tr>
<tr class="odd">
<td><em>L</em></td>
<td>vessel length (assumed to be equal)</td>
<td>m</td>
</tr>
<tr class="even">
<td><em>D</em></td>
<td>diameter of vessels</td>
<td>m</td>
</tr>
<tr class="odd">
<td><em>e</em></td>
<td>number of embolized vessels</td>
<td></td>
</tr>
<tr class="even">
<td><em>α</em></td>
<td>constant following Poiseuille’s law</td>
<td>kg s m<sup>-3</sup> MPa<sup>-1</sup></td>
</tr>
</tbody>
</table>

2. If non-vessel air is negligible, then the volume of air in the same segment will be the volume of the sum of all the embolized vessels. 

$$V= \sum V_i = eV_i = e\pi (0.5D)^2L$$

<table>
<thead>
<tr class="header">
<th>Variable</th>
<th>Variable definition</th>
<th>Units</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><em>V</em></td>
<td>air volume of vessel</td>
<td>l</td>
</tr>
<tr class="even">
<td><em>L</em></td>
<td>vessel length (assumed to be equal)</td>
<td>m</td>
</tr>
<tr class="odd">
<td><em>D</em></td>
<td>diameter of vessels</td>
<td>m</td>
</tr>
<tr class="even">
<td><em>e</em></td>
<td>number of embolized vessels</td>
<td></td>
</tr>
</tbody>
</table>

3. Increase in moles of air, under vacuum, in the vacuum reservoir, as expected under ideal gas law (which should apply to O2, N2, CO2 and any atmospheric air under low pressure and room temperature)

$$\Delta n = n_f-n_i = {P_i V_r \over RT}-{P_f V_r \over RT}$$

<table>
<thead>
<tr class="header">
<th>Variable</th>
<th>Variable definition</th>
<th>Units</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><em>V<sub>r</sub></em></td>
<td>Volume of the vacuum reservoir</td>
<td>l</td>
</tr>
<tr class="even">
<td><em>P</em></td>
<td>initial and final pressure within reservoir</td>
<td>kPa</td>
</tr>
<tr class="odd">
<td><em>n</em></td>
<td>number of moles (initial and final)</td>
<td>mol</td>
</tr>
<tr class="even">
<td><em>R</em></td>
<td>gas constant: 8.314</td>
<td>kPa L mol<sup>-1</sup> K<sup>-1</sup></td>
</tr>
<tr class="odd">
<td><em>T</em></td>
<td>room temperature</td>
<td>Kelvin</td>
</tr>
</tbody>
</table>

4. Total volume of air discharged in to the vacuum reservoir

$$AD = {\Delta nRT \over P_{atm}}*10^6$$

<table>
<thead>
<tr class="header">
<th>Variable</th>
<th>Variable definition</th>
<th>Units</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><em>AD</em></td>
<td>Volume of air discharged</td>
<td>μL</td>
</tr>
<tr class="even">
<td><em>P<sub>atm</sub></em></td>
<td>atmospheric pressure (98kPa at 700m)</td>
<td>kPa</td>
</tr>
<tr class="odd">
<td><em>n</em></td>
<td>change in number of moles, see eqn 3</td>
<td>mol</td>
</tr>
<tr class="even">
<td><em>R</em></td>
<td>gas constant: 8.314</td>
<td>kPa L mol<sup>-1</sup> K<sup>-1</sup></td>
</tr>
<tr class="odd">
<td><em>T</em></td>
<td>room temperature</td>
<td>Kelvin</td>
</tr>
</tbody>
</table>

5. Normalizing the AD values, as a percentage of the total change between hydrated and dehydrated stems

$$PAD = 100 * {AD-AD_{min} \over AD_{max}-AD_{min}}$$

<table>
<thead>
<tr class="header">
<th>Variable</th>
<th>Variable definition</th>
<th>Units</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><em>AD</em></td>
<td>Volume of air discharged</td>
<td>μL</td>
</tr>
<tr class="even">
<td><em>PAD</em></td>
<td>atmospheric pressure (98kPa at 700m)</td>
<td>kPa</td>
</tr>
</tbody>
</table>

### Appendix C: Apparatus Photos

![alt text](images/pneumatic_2.png)

**Figure 2.** a) Test reservoir, connected to pressure transducer and
included 3-way stopcock. Stem would be connected to outlet. During
measurements the stopcock will be closed to the larger vacuum reservoir
on the left (non-orange outlet). b) Vacuum reservoir. Stopcock is
currently closed to vacuum pump, when left open, air leaks in when the
pump is not running. c) Datalogger and pressure transducer. Large blue
wire is copper/constantin thermocouple. d) Pressure transducer and
step-down voltage regulator. The voltage in is a 12V DC wall outlet (top
of voltage regulator), the voltage out to the pressure transducer is set
at 8V. Wires into the pressure run from the step-down regulator to the
white connector. The ground wire into and out of the connector are
spliced into 1 wire.

### Appendix D: Campbell Datalogger program recommendation

The program needs to log temperature and voltage, preferably every
second for high resolution recording of changes.

![alt text](images/pneumatic_3.png)  
**Figure 3.** Here’s an example of the measurements selected in the
ShortCut or PCW200 Campbell Scientific Software datalogger interface.  
——————————————————————————————-

![alt text](images/pneumatic_4.png)  
**Figure 4.** Wiring diagram for the program.  
——————————————————————————————-

![alt text](images/pneumatic_5.png)  
**Figure 5.** Sample table in the example program. Sampling is every 1
second.

### Appendix E: Concerns about the method

-   The vacuum strength at measurement could have a large effect on air
    out so it should be kept fairly standardized at least within
    measurements of any one individual stem—I’m trying to keep vacuum
    reservoir near 4.2, which drops to 4V at measure which is 62kPa at
    measure (when using 8V supply)
    -     Additionally, the argument that there is an exponential drop in air loss in  Pereira et al. (2016) would seem confounded with the fact that vacuum strength drops as air is added  
-   The AD~max~ measure may be subjective. It is essentially the highest
    measure that can be made for that plant, but that is just defined by
    equipment. I can measure -8MPa, so the AD of a measure near that
    will be AD~max~. It wouldn’t seem that the method would be very robust
    without most plants reaching that measure.
    -   I have settled on trying to reach max capacity of chamber or stopping when very little sap emerges from xylem—this is apparent when only small bubbles emerge from tiny sections of the petiole xylem indicating that very little water remains in the stem.   
-   Re: my branches, they found that vessel length wasn’t significantly
    correlated with PAD. But the authors also took the precaution of
    using smaller aerial shoots hoping that would include vessel ends.
    Some of the shoots I’ve used have been multi-branched (so that they
    contain enough leaves). Perhaps I should collect more small shoots
    with at least 4-6 leaves and aim for just 3-4 measurements per—these
    may also dehydrate more quickly
