---
hide: footer
---
###### Author: Beth Fallon, updated by: Cathleen Lapadat and Lucy Schroedert

### Goals

How to use Hansatech FMS2, data collection procedures, and downloading data

### Notes

This protocol details steps for the alternative method to measure dark adapted fluorescence without working in the dark. Please refer to "(Pre-dawn)Dark/Light Adapted Leaf Measurements" for the original method (working in the dark only). 

### Supplies/Equipment Needed

- FMS2 with fiber optic cable
- Leaf clips or aluminum foil
- Dark adapter cover
- Charged batteries with battery charger
- Leaves!
- RS232 to USB
- Parview

##### Preparation

1. In the evening before, cover leaf with foil or clips around sunset
    
2. Confirm that batteries are charged


##### Start up

1. Connect the fiber optic cable. The leaf clip with PAR sensor isn’t needed for pre-dawn measurements
    
2. Make sure that fiber optic cable is firmly seated in the hood 
    
3. Turn on machine, select program to run -> EXP, then Next -> Choose your program

##### Collecting data

###### Dark-adapted

1. If used foil to cover leaves, slide leaf clip on leaf under foil
    1. Make sure window of clip is enclosed to ensure dark acclimation
    2. Have leaf clip handle roughly perpendicular to mid vein
    
2. If did not use foil to cover leaves, skip to step d
    
3. Remove foil from leaf
    
4. Insert fiber optic/black hood assembly to leaf clip
    
5. Slide open the window of the clip
    1. Orient fiber optic cable and leaf hood so that cable is aligned over the leaf clip handle
    
6. Press Run for measurement
    
7. Record file number to data sheet and click Yes to save data
    1. Check that value is reasonable (not error-slide still closed) 
        
8. If also measuring light adapted fluorescense, with a sharpie, trace around the edges of the leaf.
    1. Remove the clip from the leaf and ensure leaf is marked for light measurements

###### Light-adapted
    
1. Locate tree/leaf and find the outline of the leaf clip from the dark-adapted measurements
    
2. Attach leaf clip in the same position as the dark-adapted measurements
    1. Check that window of clip is open
    
3. Go to your light-adapted settings
    
4. Attach fiber optic/black hood assembly to leaf clip
    1. Orient fiber optic cable and leaf hood so that cable is aligned over the leaf clip handle
    
5. Press Run
    
6. Record file number to data sheet and click Yes to save data
    1. Check that value is reasonable (not error-slide still closed) 
##### Downloading data

1. Connection with computer (RS232 to USB): 
    1. Needs to be COM1 at 38400 Baud rate. 
        1. Find the correct port on your computer for COM1.
        2. To confirm COM and baud rate on computer, go to Device Manager in control panel.
            1.  Port -> right click on COM1 -> select Properties. Go to Port settings and select your FMS baud rate.
        3. To confirm baud rate on the FMS, hold the bottom button on the display panel and switch the FMS on.
    2.   Turn off UART functioning in advanced port settings (should be default)
    3.  Restart the computer interface and/or fluorometer if changing the COM port settings
    
2. Using Parview
    1. Check machine status
        1. Hardware -> Status
            1. shows protocol numbers, number of files
            2. Hardware -> Set date/time
                1. !! Caution date must be in DD/MM/YY: can use PC date and time, but must adjust manually
                2.    Time in HH:MM:SS (also adjust manually)
    2. View data
        1. File -> Upload params
            1. Choose protocol number (#1 = Fv/Fm)
        2. See actual data:
            1. Column headings -> AutoSet, OK
            2. Should see all the data then
    3. Download data
        1. File -> Convert to ASCII
            1. Save as Oakwilt_fluor_YYYYMMDD.ASC
            2. Open that file externally with notepad and make sure that all data is present
    4. Clear data: ! Only after making sure have all data you need, Clears all data!
        1. Hardware -> Clear memory
            
###### Tips

* Same instrument should be used for dark adapted and light adapted measurements on the same leaf
* If leaf is damp in morning, have paper towels to dry off leaf before marking with sharpie

