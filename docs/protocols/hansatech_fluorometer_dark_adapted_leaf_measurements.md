###### Author: Beth Fallon

###### Associated project: Grand Challenges - Oak Wilt

### Goals

How to use Hansatech, data collection procedures, and downloading data

### Steps

1.Start up

-   1.  Connect the fiber optic cable (silver). The leaf clip with PAR
        sensor isn’t needed for pre-dawn measurements.

-   1.  Make sure that fiber optic cable is firmly seated in the hood.

-   1.  Turn on machine, select program to run -> EXP, then Next ->
        Program #1 Fv/Fm

2.Collecting data

-   1.  Best practices:

    -   1.  Measurements should be completed before any measurable light
            is on (need to check with other greenhouse users about lamp
            time on), this is generally at nautical twilight ++ ii. Use
            a green headlamp and avoid casting light on leaves as much
            as possible

-   1.  Measuring dark adapted fluorescence ++ i. Use a leaf clip over
        the measurement area, keep slide closed until measuring. Have
        leaf clip handle roughly perpendicular to mid vein ++ ii. Attach
        fiber optic cable/leaf hood over the leaf clip securely to
        occlude all light ++ iii. Orient fiber optic cable and leaf hood
        so that cable is aligned over the leaf clip handle ++ iv. Open
        slide and press RUN ++ v. Check that value is reasonable (not
        error—slide still closed) -> Save Yes ++ vi. Note the File
        number

3.Downloading data

    a.  Connection with computer (RS232 to USB): 
      i.    Needs to be COM1—(currently on Panasonic this left most port) at 38400 Baud rate. 
      ii.   Turn off UART functioning in advanced port settings (should be default)
      iii.  Restart the computer interface and/or fluorometer if changing the COM port settings
    b.  Using Parview
      i.    Check machine status
        1.  Hardware -> Status
          a.    shows protocol numbers, number of files
        2.  Hardware -> Set date/time
          a.    !! Caution date must be in DD/MM/YY: can use PC date and time, but must adjust manually
          b.    Time in HH:MM:SS (also adjust manually)
      ii.   View data
        1.  File -> Upload params
          a.    Choose protocol number (#1 = Fv/Fm)
        2.  See actual data:
          a.    Column headings -> AutoSet, OK
          b.    Should see all the data then
      iii.  Download data
        1.  File -> Convert to ASCII
          a.    Save as Oakwilt_fluor_YYYYMMDD.ASC
          b.    Open that file externally with notepad and make sure that all data is present
      iv.   Clear data: ! Only after making sure have all data you need, Clears all data!
        1.  Hardware -> Clear memory
