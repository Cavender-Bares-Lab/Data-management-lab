---
hide:
  - footer
---

###### Author: William C. Eddy; Updated: 6 November 2019 by Allison Gill

Dissolved Organic Carbon (DOC) measured as non-purgeable organic carbon (NPOC) and Total Nitrogen. Often used in our lab to measure microbial biomass on non-fumigated and fumigated soil samples.

### Instrument

- Shimadzu TOC-VCSN
- Shimadzu TN unit
- Shimadzu autosampler (ASI)
- Shimadzu TOC-V software controller  
    *Owned by Jacques Finlay.*

### Samples

- Water (no dilution, and Salt Extracts (3x dilution)

### Supplies

- Aluminum Foil
- Standard Stock Solution (Finlay lab fridge next to instrument)
- 2 M HCl
- 0.05 M HCl
- Nanopure water
- Volumetric pipets
- Volumetric flasks
- 23 mL glass Vials (number of samples plus 14 standards)~
- Ultra High Purity air (Ustores p/n cx77020)~

**Note: Supplies with ~ and other Shimdzu supplies (TOC catalyst, combustion tubes, O rings, etc, are supplied by Jacques Finlay as part of the per sample cost.)**

### Procedure

##### Sample Preparation

*The Shimadzu carousel can accommodate 93 total vials. Each run will require 14 vial spaces for standards (2 curves with seven points each). Vials are stored in the Hobbie Lab and should be acid washed and ashed between uses.*

1. For HIGH SALT SAMPLES (0.5M K2SO4) **Please dilute your samples at least 4:1** to a total volume of 22 mL. This will make the catalyst and detectors last longer. This should be done manually.

2. Put 22 mL of sample in TOC vial. Add 100 uL 2 M HCl to each vial. Cover with aluminum foil and press down over top with thumb.

3. Store acidified samples in the refrigerator until you are ready to start your run (ideally that day).

##### STANDARD PREPARATION

*Prepare standards using the stock solutions located in the Finlay Lab fridge near the Shimadzu. Make sure to use appropriate standard containers (most often for total N and DOC rather than DIC).*

1. Dilute standard stock solutions to build curve containing seven concentrations, with target concentrations matching those listed in the DOC-TDN Standard Dilution Template.

2. Place TOC vial on a balance and zero mass. Add DOC stock solution to target mass according to the DOC-TDN Standard Dilution Template (Column G). Record mass in column I. Add TDN standard (goal amount in column H) and record mass of both standards in column J (do not zero balance between standard addition). Add nanopore water to a total mass of ~22 g and record in column J. Calculate the exact standard concentration as: (Mass stock\*Stock Concentration)/Total Solution Mass. (Solution density =1g/mL, which allows the solutions to be prepared by mass rather than volume).

3. Prepare two replicate curves, recording exact masses and calculating concentrations for each.

4. Each standard vial can be analyzed twice. I usually place standards in positions 1-14 in the carousel and assign one set to be read at the start and after 1/3 of samples and the other to be read after 2/3 of samples and at the end. If you not running the full rack of samples, it may be fine to make one set of standards and run it at the beginning and end of the run.

##### SAMPLE ANALYSES

Machine Start-up:

1. Start air flow to TOC by opening main valve on gas tank. Check that 500 psi air remains in tank to complete a run. Do not run the analyzer below 500psi!

2. Power on TOC-L (button on front of machine). Ozone generator should turn on automatically.

3. Turn on Computer

4. Open TOC control to warm instrument
    1. Connect by clicking the lightning bolt, always using “settings on PC”
    2. Warm up should take 45min (TOC-L).

5. Pre-run checks:
    1. Open front panel on TOC machine
    2. Check Humidifier level- it should be within ¼” of  high mark. Fill with nanopure water if level is low.
    3. Acid (0.05M HCl) column inside machine should be full and bubbling
    4. Acid at the side of the machine (2M HCl)
        1. Volume above ¼, tube at the bottom of bottle
    5. NOTE: backpressure sometimes prevents acid addition. ENSURE THAT ACID ADDITION IS FUNCTIONING BY OBSERVING MOVEMENT OF ACID INTO THE MULTIPORT VALVE DURING SAMPLE.
    6. Dilution (square bottle next to machine) and rinse reservoir
        1. Fill with fresh nanopure
        2. NOTE: backpressure sometimes prevents dilution. ENSURE THAT DILUTION IS FUNCTIONING BY OBSERVING MOVEMENT OF WATER INTO THE MULTIPORT VALVE DURING SAMPLE INTRODUCTION.
    7. Halogen scrubber – if there is more than a cm or so of discoloration, it is time to replace the scrubber. (if any doubt, replace the scrubber. It is relatively cheap, the detector is not)

6. Warm up check list
    1. Pressure Gauge inside instrument should be 200kpa; Mass flow for TC should be 125-130. Set the flow rate to ~210kpa for the TOC-L using the regulator on the gas tank. The meter is in the “monitor” tab.
    2. Check back internal water reservoir for bubbling (there shouldn’t be).   Bubbling indicates overpressure of TN unit or too little water in back reservoir (add until it overflows into tube using a squirt bottle).
    3. TOC-L – TNM-1, O3 generator, and autosampler turn on with main button (onfront of machine)
    4. TN flow should be 0.4 – 0.5 for TN

7. Sample setup (one option)
    1. Create new sample run: “File”, “New”, “Sample Run”
    2. Connect to the analyzer, always using “settings on PC”
    3. Go to “Insert” and select “Sample” to set up sample table
        1. Select previously stored  method that will reference the specific calibration files you would like to use (use one with most recent date)
        2. Insert samples or autogenerate samples
        3. Insert standards at beginning, middle, and end of the run (each standard can be read 2 times, so read the same set for the beginning and middle, then a different set for the end)
            1. Insert standard concentrations from the same protocol: “insert” > “sample” then hit “next” until through the menu.
        4. Run a rinse before low standard and after high standard each time (So you will be inserting 7 samples and 2 rinses). Rinses should be noted as vial position zero.
        5. Assign vial positions to each sample
        6. Important: Run at least 4 blanks at the end of the run to flush the sample syringe. These may be draw from the Erlenmeyer flask (i.e. vial position zero) to save room on the autosampler rack. To do this, “Insert” > “Multiple Samples”. Check the rinse reservoir each day and refill with nanopore as needed.
    4. Save file with unique name in the appropriate “Data” folder
    5. Load samples in carousel in appropriate vial positions

8. Wait for top right corner of the DOC program to say “ready”
      
9. Run Samples
    1. Click on stoplight (connect if the stoplight isn’t highlighted)
    2. Make sure vial positions are correct, edit if necessary

10. Save file then export as ASCII (detailed version)

11. Shutdown
    1. Automatic shutdown: 
        1. select “shut down instrument” button on standby in sample setup
        2. shut off gases once the unit turns itself off, or as soon as possible thereafter
        3. NOTE: the automatic shutdown does not always work!! 
    2. Manual shutdown: (i.e. “ keep running“ selected in sample setup)
        1. Click on standby icon to begin shutdown Let gas run for 20min
        2. Machine will completely power down in 30min. Turn off gas at main valve

12. Files
    1. Your data
        1. It is possible to reanalyze sample runs at a later date if the appropriate files are saved
        2. If there are data, method, or calibration files (i.e. all files associated with your run) that you wish to keep after you are through running your samples, please keep a copy either on a disk or in the “Shimadzu user files” folder
    2. Your responsibilities
        1. Please update the log sheet as to the specifics of your run such as the number of samples run, budget numbers, analysis performed, et cetera. 

### CALIBRATION AND METHODS FILES

1. Calibration
    1. Standard curves are stored in fridge #1 and may be used in multiple runs:
        1. Standards should bracket samples across no more than 1order of magnitude i.e. use various curves according to the expected sample concentration. 
        2. Always add standards to your own run as a check of calibration – best to run a set at the beginning, middle and end to adjust for any drift.

2. Method file – use one of the preset methods listed below for the TOC-L or most recent for the TOC-Vcsh.
    1. Water 160pp C 20ppm N
    2. Water 500ppm C 20ppm N
    3. Water 100ppm DIC
    4. Salt 160ppm C 20ppm N ***This is probably what you want to use

### ROUTINE MAINTENENCE

1. Change CO2 absorber and halogen scrubber 12 months, or as soon as discoloration begins.

2. Catalyst: 
    1. Regenerate catalyst when repeatability declines using “Regenerate catalyst  “ command under “Maintenance”
    2. If performance does not improve, replace catalyst.  After installing new catalyst, condition it using 10 DI samples (5inj/sample, 150L/injection; use method “New column breakin.met”).

3. Change membrane filter, o-rings, and manganese dioxide (TN) once per year.

4. Check screw on bottom of injection syringe (with lockwasher between syringe and screw).  Screw should be tight – if it’s loose, tighten it up & watch it to ensure it does not fall off during the run.

5. If syringe adjusted, use “syringe zero point detect” to reset syringe.

### NOTES and TROUBLESHOOTING:

1. For manual injection, use vial zero

2. Peak shape usually not of concern. However, could indicate problems:
    1. Combustion tube
    2. Sample injection

3. No baseline return = contamination

4. Keep instrument door closed

5. Concentrated Stock standards should be remade every 6 months

6. Detection limits
    1. Regular sensitivity catalyst
        1. DOC = at least 0.5mg/l
        2. TN = at least 0.1mg/l
    2. High sensitivity catalyst (a new machine system is necessary)
        1. DOC = 0.05mg/l ?
        2. TN measurements CANNOT be made with this catalyst

### HIGH SALT SAMPLES (i.e. 0.5 M K2SO4 extracts)

1. Please dilute your samples at least 4:1 ! This will make the catalyst and detectors last longer. This should be done manually. 

2. At the end of every overnight run:
    1. rinse sample line and valve lines (automatic)
    2. rinse injection port and syringe
    3. run 3 DI samples, using 5 injections per sample, 150 µL per injection

3. Catalyst/columns lasts about 700 samples, but has to be washed after 500-600 samples due to salt build-up, so it’s best just to change out catalyst when salt build-up gets too great (after 500-600 samples). If samples are diluted, salt build up may not be an issue before catalyst change is necessary.

4. Acid wash combustion tube when changing catalyst—it’s good to have an extra tube on hand so that you don’t have to wait to pack a new column.

5. Sometimes after salt build-up is high, pressure builds up and unseats the combustion tube, forcing it out of the O-ring seal.  When this happens, the TOC reading is 0.000 due to leakage. 

### CONSUMABLES

Please inform Finlay if any other supplies (e.g. combustion catalyst) are running low.

### METHODS OPTIONS:

- IC – sparge to the detector

- TC – everything to the detector

- TOC – by difference

- NPOC – Sample is acidified, sparge gas is vented, liquid is injected to detector. Risk is loss of volatile organics.
