---
hide: footer
---

# PSR Leaf Measurements Protocol

#### Author
Isaiah Clark

### Goal

Step-by-step assembly and operation of Spectral Evolution PSR+ spectrometer for both fiber optic cable/leaf clip and FOV lens.

### Information

The Spectral Evolution PSR+ 3500 is a portable spectroradiometer for high resolution remote sensing applications in the field. The principal components of the PSR are: the main unit, the power cable, the lens (for making distance measurements) and the lamp module, fiber optic cable, and leaf clip (for leaf-level measurements). The Getac handheld device connects to the unit via bluetooth and displays/stores collected spectra.

For more info, refer to the PSR and DARWin software manuals (teal binder labeled Spec Evo, on lab bench shelf).

### Fiber optic cable and leaf clip (direct measurements):

##### Assembly

1. Insert a fully-charged battery into the rectangular slot to the left of the control panel until you hear a click. 

2. Loosen the silver thumbscrew to remove the protective cap from the fiber adapter. On the split end of the fiber optic cable, insert the keyed terminal into the fiber adapter and re-secure with the thumbscrew. 

3. Insert the single terminal end of the fiber optic cable into the leaf clip and secure it with plastic screws. 

4. Attach the lamp module to the main unit by sliding it onto the unit track and securing with the small screw on the side of the module. 

5. Insert the other terminal on the split end of the fiber optic cable (smaller and threaded) into the bottom of the lamp module and tighten. 

6. Just like the fiber optic cable, the power cable also has a split end and a single terminal end. Connect the two ends of the split side of the power cable with the main unit (next to fiber adapter) and the lamp module (on top, next to the red switch)
    1. Insert the single end of the power cable into the leaf clip. At all three cable connections, make sure to line up the red marks on the cable with the corresponding marks on the plug.

##### Operation

1. Turn the main unit on (switch next to the main unit control panel). 

2. Turn the Getac PS336 device on by holding the power button (bottom right) for a few seconds. 

3. Open Darwin software (Windows menu &gt; DARWin Compact 1.2) 

4. In the Device tab, set the drop-down menu at the top of the window to COM8 and tap Connect; it takes a few moments. 

5. Edit filename to your first measurement name (ex. 0001). 

6. Make sure Auto-Integration is checked and Optic is set to the first “Unverified” destination listed. 

7. Then go to the Scan tab. Turn the lamp on (red switch on lamp module). 

8. The leaf clip has two faces: one with a PTFE reference (white) and one with anodized black. These faces can be switched by pulling the plate away from the hinge of the clip and rotating. 
    1. With the white reference facing the fiber (i.e. on the inside of the clip) and the clip closed, take a reference measurement by tapping “Ref” on the Getac. 
    2. Flip the leaf clip plate back over so that the black side faces the fiber. 

9. You can now take measurements by clipping your leaf with the adaxial side facing the fiber and tapping “Tgt” on the Getac. 
    1. Take a new white reference every ~10 samples (especially if you are measuring outside, to account for changes in solar altitude). 

10. After all measurements have been taken, first disconnect the Getac and then turn off the main unit. If you need to replace the battery at any time during measuring, follow this order as well. 

11. Export all data from Getac to PC via USB.

### FOV lens (distant measurements):

##### Assembly

1. Insert a fully-charged battery into the rectangular slot to the left of the control panel until you hear a click. 

2. Loosen the silver thumbscrew to remove the protective cap from the fiber adapter. 

3. Remove the fiber adapter and screw in the FOV lens until tight.

##### Operation

1. Turn the main unit on (switch next to the main unit control panel). 

2. Turn the Getac PS336 device on by holding the power button (bottom right) for a few seconds. 

3. Open Darwin software (Windows menu &gt; DARWin Compact 1.2) 

4. In the Device tab, set the drop-down menu at the top of the window to COM8 and tap Connect; it takes a few moments. 

5. Edit filename to your first measurement name (ex. 0001). 

6. Make sure Auto-Integration is checked and Optic is set to "LENS:4 {Radiance}" destination listed. 

7. Then go to the Scan tab. Turn the lamp on (red switch on lamp module). 

8. For distant measurements, the spectralon panel is used as a white reference. 
    1. Take a reference measurement by holding the unit as level and perpendicular as possible above the panel and hitting “Ref” (you can hold down the silver laser scan switch on the front of the main unit before taking your measurements to show where the lens is pointing.) 

9. You can now take distant measurements by elevating the unit as before, directing the lens over the sample, and tapping “Tgt” on the Getac. 
    1. For all distant measurements, make sure to avoid casting any shadows into the field of view and wear dark clothing to minimize interference with the signal. 
    2. Take a new white reference every ~10 samples (especially if you are measuring outside, to account for changes in solar altitude.) 
    
10. After all measurements have been taken, disconnect the Getac and then turn off the main unit. If you need to replace the battery at any time during measuring, follow this order as well. 

11. Export all data from Getac to PC via USB.