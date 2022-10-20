---
hide: footer
---

# HPLC - Run Samples Protocol
### Author
Anna Schweiger and Cathleen Lapadat

### Updated
September 2022

### Quick Guide

1. Turn on all power buttons on machine
    1. Open ChemStation
    2. Turn on DAD lamp
    3. Turn on pump
    4. Turn on column thermostat
    5. Turn on sample thermostat

2. Process leaves/needles for pigment extraction 

3. Choose method and add sample ID into sequence
    1. Add samples into auto sampler tray
        1. Isopropanol in position 21
        2. Acetone blank in position 1
        3. Samples in position 2-xx
        4. Last in extraction is leaf standard

4. Start sequence run

5. Check first sample and every few samples to ensure machine is running properly

### Detailed Procedure
##### Setup instrument
1. Make sure you have an enclosed waste container collecting liquid from the waste lines.
    - Note: We are currently using a nalgene bottle that has a hole drilled into the cap with the waste line attached through the hole.
    
2. Start instrument: click all power buttons on HPLC.

3. Open ChemStation program: “Instrument 1 online” from icon on Desktop.

4. At least 20 min before running a sequence (ideally start before extraction):
    1. If you are unable to turn any of these below, please restart the system. Make sure all parts are turned on properly prior to starting up Chemstation.
        1. Turn on DAD/lamp to allow lamps to warm up, click small symbol on bottom right of DAD symbol
        2. Turn on column thermostat
        3. Turn on sample thermostat (machine will still run if this is not turned on so it is important to confirm that this is on as it keeps samples cool during run)
        4. Turn on pump to establish steady pressure: click small symbol below the pump control, make sure instrument is running solvent A (2ml/min)
        5. Instrument is ready when both the blue (pump pressure) and the red line (signal) in the graph have reached equilibrium: 80-90 bar for pres-sure for solvent A (depends on solvent), solid line for signal

5. Mix solvents in bottles: shake carefully by hand). 

6. Ensure you have enough solvent in the bottles you are using and the correct volumes are entered in solvent bottle icons: click on bottles below pump control and change solvent bottle filling if not correct. 

7. Make sure “turn pump off if running out of solvent” is checked.

8. Check that solvents are correctly labelled: load method, click pump control icon - set up pump, the names of the solvents have to correspond to the bottles on the tray.

##### Setup and Start Sequence
1. Have all your samples for one run (max. 20) prepared and stored on ice.
    1. Place samples into the auto sampler. 
        1. Isopropanol in position 21
        2. Acetone blank in position 1
        3. Samples in position 2-xx
        4. Last in extraction is leaf standard

2. Load Method: DOB_2016

3. Assign path: 
    1. Method and Run Control: Sequence tab - Sequence parameters: enter your name
    2. Path C:\Chem 32\1\DATA\ cannot be changed: assign a new subdirectory for your samples: e.g. name and date. Save original data in this folder and don’t ever change. For analysis make a copy of the folder and move to Lab-cavender shared drive.
    3. Make sure Shutdown - Post sequence command “STANDBY” is loaded and checked
    4. Move the new folder to the project folder after the sequence was completed

4. Load or create sequence: 
    1. Sequence tab - load sequence template or new sequence
    2. New sequence: click on the template below start button - sequence table
    3. Method for sample vials and blanks: DOB_2016.M 

5. Number the vials starting from 1, give each sample a unique name, insert/append lines as needed 

6. Make sure your vial # and location of the sample in the auto sampler match, select method to be used for each sample (usually the same), select the number of injections per sample (usually 1).

7. Set up Injector: click on syringe icon: define position of wash vial (position 21), injector volume should be 20 µl

8. Start sequence: click start or run sequence from sequence table.

9. When finished: switch pump, thermostats and lamps off (off button below GLP), close program, switch power of all units off. 

##### Sample Sequence
1. Blank – Acetone
    1. Change between each run

2. Leaf samples (Limit to no more than 20 per extraction; dependent on the number of samples you can extract within 2 hours.)

3. Leaf standard
    1. Purpose of leaf standard is to make sure it always falls in the [expected range]().
    2. Collect a leaf and take several hole punches. Wrap in aluminum foil, label and put in -80 C freezer.
    3. Consistently keep it around the same position for each run e.g. the 15th sample in each run if extracting 15 samples.

##### Wash
1. Isopropanol wash in between each blank/sample/leaf standard

2. Change between each run

### Weekly maintenance: 
1. Rinse out bottles with distilled water each week
    1. Dry completely prior to use
2. Change out solvents if it was not used up within 7 days

### Maintenance and tips 
1. Sample IDs in sequence table can be added or changed during a run as long as it the specific line is not currently running

2. All chemicals always have to be HPLC grade

3. Method parameters: DOB2016
    +	2 ml/min
    +	Stop: 25 min
        -	1: 12 min 0% C
        -	2: 16 min 100% C
        -	3: 18 min 100% C
        -	4: 19 min 0% C
    +	A: Acet/MeOH/Tris
    +	C: MeOH/Ethyl Acetate

4. Every ½ year: change purge valve frit (small filter in pump).

5. After changing seals: use solvent running at 350 bar to tighten

6. Sonicator can be used clean solvent filters if they get dirty or clogged. 

7. Check lamp:
    1. Diagnostics – DAD calibration, Holmium, Internal tests
    2. Run HPLC water, take flow cell out, bypass column
    3. Compare counts
    4. Results are wvl dependent, if lamp fails in wvl not relevant for pigment spectra, failure doesn’t matter much

8. Use the Help Tab in ChemStation: Tutorial for analyzing samples and data. 

9. Agilent helpline: 800 277 9770

### Problems
1. Leak error
    1. Instrument will turn of automatically (or stop pump, stop sequence), switch off power, repair leak (reassemble and tighten again), make sure areas around leak and leak sensors are dry. Each compartment has its own leak sensor (u-shaped wire): instrument will not run until the sensor is dry even if the leak has been resolved.
    2. Often after changing the column or cleaning out pump there will be a leak.

2. High pressure error 
    1. Often when switching between solvents (column cleaning, new methods)
    2. New solvent combinations: turn down pump rate, run gradient
    3. Check the lines: make sure you are not forcing air into the system
    4. Check solvent bottles: if the plastic filter on the end of the solvent line in the solvent bottle is clogged, try to clean it in strong acid or replace. You can check if this is the problem by temporarily removing the filter and see if that improved pressure.
    5. Check the inner pump filter: unscrew and remove the pump behind the black control knob, remove the filter end in the inner cylinder and clean with isopropyl alcohol, occasionally the filter will need to be replaced (1x year), carefully reassemble pump (often may initially leak).