---
hide: footer
---

# Pre-dawn Dark/Light Adapted Leaf Measurements Protocol
###### Author
Beth Fallon

###### Updated
Summer 2022 by Cathleen Lapadat

###### Associated project
Grand Challenges - Oak Wilt

### Goals

How to use Hansatech, data collection procedures, and downloading data

### Notes

This protocol details steps to measure pre-dawn dark-adapted fluorescence.

### Supplies/Equipment Needed

-   FMS2 with fiber optic cable
-   Leaf clips or aluminum foil
-   Dark adapter cover
-   Charged batteries with battery charger
-   Leaves!
-   RS232 to USB
-   Parview

##### Start up

1.  Connect the fiber optic cable (silver). The leaf clip with PAR sensor isn’t needed for pre-dawn measurements.
    
2.  Make sure that fiber optic cable is firmly seated  in the hood. 
    
3  Turn on machine, select program to run -> EXP, then Next -> Program #1 Fv/Fm

##### Collecting data

1.  Best practices:
    1. Measurements should be completed before any measurable light is on, this is generally at nautical twilight
    2. Use a green/amber headlamp and avoid casting light on leaves as much as possible
    
2.  Measuring dark adapted fluorescence
    1. Use a leaf clip over the measurement area, keep slide closed until measuring. Have leaf clip handle roughly perpendicular to mid vein
    2. Attach fiber optic cable/leaf hood over the leaf clip securely to occlude all light
    3. Orient fiber optic cable and leaf hood so that cable is aligned over the leaf clip handle
    4. Open slide and press RUN
    5. Check that value is reasonable (not error—slide still closed) -> Save Yes
    6. Note the File number

##### Downloading data

a. Connection with computer (RS232 to USB): 
    1. Needs to be COM1 at 38400 Baud rate. 
        1. Find the correct port on your computer for COM1.
        2. To confirm COM and baud rate on computer, go to Device Manager in control panel.
            1. Port -> right click on COM1 -> select Properties. Go to Port settings and select your FMS baud rate.
        3. To confirm baud rate on the FMS, hold the bottom button on the display panel and switch the FMS on.
    2. Turn off UART functioning in advanced port settings (should be default)
    3. Restart the computer interface and/or fluorometer if changing the COM port settings
    
b.  Using Parview
    1.Check machine status
        1. Hardware -> Status
            1. shows protocol numbers, number of files
        2. Hardware -> Set date/time
            1. !! Caution date must be in DD/MM/YY: can use PC date and time, but must adjust manually
            2. Time in HH:MM:SS (also adjust manually)
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
