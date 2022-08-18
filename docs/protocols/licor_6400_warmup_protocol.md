---
hide:
 - footer
---

###### Author: Licor, Inc.; Manual: Chapter 4 -> Please refer to the manual for the fundamental of good measurements in Chapter 4: Making Measurements.

### Goal

Checklist of things that should be done prior to making measurements with Licor 6400/6400xt. Takes about 5 minutes.

### Supplies Needed

- Licor 6400/6400XT with leaf chamber
- Charged batteries
- CO<sup>2</sup> canisters
- Soda Lime
- Drierite
- Plants!!!

### Checklist Summary

1. During Warm up
    1. Air Supply: Prepare CO2 Mixer or Buffer Volume
    2. Temperatures: Values OK? Tleaf responding?
    3. Light Source, Sensors: Responding? Values OK?
    4. Pressure Sensor: Value OK? Stable?
    5. Leaf Fan: Running?
    6. Flow Control: Max flow OK? Chemical tube restrictions?
      
2. After Warm-up
    1. Check the flow zero
    2. Adjust latch, close chamber
    3. Check CO2 zero
    4. Check H2O zero
    5. Mixer Calibration (optional)
    6. Lamp Calibration (optional)
    7. Check Tleaf zero
    8. Set Reference CO2 and H2O
    9. Test for leaks
    10. Match the IRGAs. Valve working?
      
3. Measuring the First Leaf
    1. Set Light
    2. Set Flow to 400 μmol s-1
    3. Set Reference CO2
    4. Temperature?
    5. Clamp onto leaf
    6. Set Area and Stomatal Ratio
    7. Set constant humidity?

### Detailed Steps During Warm Up

Once OPEN is loaded, and while the gas analyzers are warming up, you should do these steps.

1. Air Supply - Cartridge or Buffer Volume? 
    If you are going to be using the 6400-01 CO2 mixer, install a cartridge now, so the system can begin pressurizing. Otherwise, prepare a buffer volume (see Air Supply Considerations on page 4-50).

2. Check the Temperatures
    The three measured temperatures (block, air, and leaf) are together in display group h. Check to see that they read reasonable values, and are within a few degrees of each other.
    Position the thermocouple properly, either just above the gasket (Figure 19-23 on page 19-25) for leaf measurement (normal), or pulled down for air temperature measurement (energy balance).

3. Check the Light Source and Sensors
    Check to make sure that the instrument is configured for the light source that you are using. See Specifying the Source and Sensor on page 8-3.
    The light sensors (ParIn_μm and ParOut_μm) are both in default display group g. See that they respond as expected when the light sensors are illuminated and darkened.
    If you get negative ParIn_μm values, there is probably a mismatch between the real light source, and the one OPEN thinks it has. A trip to <open> <light> <source> in Config Menu | View/edit (page 8-4) will fix that.

4. Check the Pressure Sensor
    The pressure measurement (Prss_kPa) is shown in display group g. See that it shows reasonable, stable values. (Typical values: 100 kPa near sea level, 97 kPa at 1000 ft., 83 kPa at 5000 ft., etc., but this varies with the weather.)

5. Check the Leaf Fan
    Turn the leaf fan off and on (f3 level 3), and listen for sound changes in the sensor head as the fan motor stops and starts. If you do not hear a sound when the fan should be on, it could mean a blown fuse (fan or flow board), a fan jammed with debris, or other problems (see Chapter 20). Leave the fan on when you are done.

6. Is Flow Control OK?
    Use the flow control key (f2 level 2) to fix the flow at 1000 μmol s-1. Watch the Flow_μms (display group b) to determine the actual maximum flow. The value is typically in the 700’s if a CO2 mixer is installed, or higher if not.
    Now test the chemical tubes for flow restrictions by changing each from full bypass to full scrub, and watching the effect on flow rate. Normally, scrubbing
    will drop the maximum flow by 5 or 10 μmol s-1 per tube. Larger drops may indicate that the air mufflers in the chemical tubes are getting clogged, or that a flow diversion tube is pinched shut. See Pump/Flow Problems on page 20-13 for more details.
    Finally, set the flow to 500 μmol s-1.

### Detailed Steps After Warm Up

After the IRGAs have been on for about 10 minutes, continue with the following steps:

1. Check the Flow zero
    In New Measurements mode, monitor Flow_μms (display line b) and turn the pump off (2 f2 N) and the chamber fan off (3 f3 O for off)2. The flow should drop to within 1 or 2 μmol s-1 of zero. If it doesn’t, re-zero the flow meter (Zeroing the Flow meter on page 18-23). Turn the fan back on when done.

2. Adjust the latch, and close the chamber
    1. Adjust the latch so that the chamber lips are slightly apart when the chamber is closed. 
    2. With the chamber closed, close the adjustment knob until it starts to become snug. 
    3. Open the chamber, and turn the knob one or two more half turns. Now the chamber is adjusted properly for sealing when empty, or with thin leaves. Close the chamber for the next two steps.


3. Check the CO2 IRGA zero
    In New Measurements mode, with the mixer off (2 f3 N), and the flow set to 500 μmol s-1 (f2 F 500 enter), monitor CO2 reference and sample (display line a). Turn the soda lime on full scrub, and the desiccant on full bypass. The reference should quickly approach zero, while the sample will approach zero a bit more slowly. If they are within 5 μmol mol-1 of zero, it will be adequate.

4. Check the H2O IRGA zero
    Turn the desiccant to full scrub, and watch sample and reference H2O. The reference will again approach zero faster than the sample does. It will zero more slowly than the CO2 IRGA did, however, because of water sorption. Rather than wait the 10 or 20 minutes to get a really good zero, use your judgement. If after a minute or so, the reference is down to 0.2 or 0.3 mmol mol-1 and falling slowly, that’s good enough. The sample will be higher than that. Clearly, if it’s negative and falling after only 1 minute, it will be going too low, and re-zeroing may be in order.
    If the CO2 or H2O IRGAs need zeroing, refer to Setting the CO2 and H2O Zero on page 18-11. The important thing is that the reference IRGAs are reasonably well zeroed (let’s say ±5 μmol mol-1 CO2, ±0.5 mmol mol-1 H2O). The first time you match (Step 10, coming up), the sample IRGAs will be taken care of, as they are adjusted to match the reference IRGAs.
    **Important Note about CO2 and H2O Zeros:** If your chemicals are not fresh, then you will do more harm than good by setting the zeros with them.
    The IRGA zeros are quite stable, especially in the absence of big temperature changes. Therefore, the exercise of checking zeros each day is really a diagnostic. If the indicated concentration doesn’t change when it should (that is, if it doesn’t drop when you start scrubbing), then something is wrong, and it’s good to find that out early.

5. Mixer Calibration
    If you are using the 6400-01 CO2 Mixer, run the routine found in Calib Menu | CO2 Mixer | Calibrate, described in 6400-01 CO2 Mixer on page 18-25. The chamber can be open for this. Make sure that the soda lime is on full scrub.

6. Lamp Calibration
    If you are using the 6400-02 or -02B LED Source, or the 6400-40 LCF, run its calibration (Calib Menu|LED Source|Calibrate described on page 18-30 , or Calib Menu | LCF Source | Calibrate described on page 27-75). You will do the best calibration by having the chamber closed onto a representative (with respect to its reflectance) leaf. This isn’t critical however, but the chamber should at least be closed.

7. Check Tleaf zero
    Unplug the leaf temperature thermocouple connector (it’s purple colored), and compare the leaf and block temperatures. If they differ by more than 0.1°, then adjust the leaf temperature zero (see Zeroing the Leaf Temperature Thermocouple on page 18-24).
    Finally, reconnect the thermocouple, open the chamber, and verify that “Tleaf_°C” responds when the thermocouple is warmed by touching it.

8. Set Desired Reference Values for CO2 and H2O
    If you are using the CO2 mixer, set it to control on reference concentration with a target of 400 μmol mol-1. Make sure that the soda lime is on full scrub.
    If you are not using the CO2 mixer, monitor the reference CO2 concentration. Is CO2R_uml sufficiently stable? (Over a 30 s period, it should change less than 2 μmol mol-1.) If not, use a larger buffer volume.
    For H2O, set the desiccant at mid-range (between scrub and bypass) for now.

9. Leaks?
    Set the flow rate to 200 μmol s-1. With the chamber closed and empty, exhale around the chamber gaskets, and look for any fluctuations in the sample cell CO2 concentration (CO2S_μml, display group a). If there are no leaks, the CO2S_μml value should not increase by more than 1 μmol mol-1.

10. Match the IRGAs
    Matching the IRGAs is easily accomplished whether the chamber is empty or not, but it’s a good policy to do this once right before starting a measurement. Refer to Matching the Analyzers on page 4-33 for how to do this. Verify that the match valve is in fact working. Figure 4-2 on page 4-34 shows what to look for. You are now ready to clamp onto a leaf and begin measurements.
