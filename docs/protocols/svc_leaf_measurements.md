---
hide: footer
---

# SVC Leaf Measurements Protocol
###### Author
Beth Fallon

###### Associated project
Grand Challenges - Oak Wilt

### Goals

How to prepare and use SVC, including data collection using either computer or built-in screen

### Important Note

This protocol was originally written for an oak wilt potted seedling experiment. Some steps are very specific in file naming and measurements. If you need a more specific protocol tailored to your project, create another protocol while using this as a template and store in protocols with your project in “Associated Project”. The SVC settings are the same throughout projects.

### Quick Measure Guide

1.  Check that white reference disc, black background, and glass lens are clean

2.  Secure leaf clip to tripod stand, attach battery, turn on light (10 minutes to warm up)

3.  New battery in spectroradiometer body, attach fiber optic cable, turn fan on Spec body

4.  Connect to SVC via Bluetooth and set integration time to 2 sec

5.  Create a new Windows file folder for data collection: YYYYMMDD, leave window open

6.  At each plant: 
    1.    Adjust height of leaf clip to measure full sun leaf:
    2.    Open a new file in SVC software (Alt+F+N)
        1.    Named plant id = “####”
    3.    Take a white reference with empty leaf clip, white disc facing in (Alt+R)
    4.    Take a white target measurement (Alt+T), if line is flat at 100%, then change suffix of data file collected to “####_000WR”
    5.    Take a target measurement with leaf inside, black background behind
        1.    Change Suffix to indicate leaf type (no suffix for green, non-symptomatic, SYM for symptomatic, S-T or S-G)
    6.    Measure 3 healthy leaves/plant; 3 symptomatic leaves when present (up to 3 measures/symptomatic leaf)
    7.    Note log # (number after plant ID) for each measure on datasheet

7.  Take a new white reference when adjusting leaf clip height

8.  Copy data folder to CBS Shared drive
<br>
### Detailed Steps of Measurements

##### Start Up

1. Insert new battery in SVC console (main body of machine)
      
2. Extend legs at base of SVC body
      
3. Remove forelens and insert fiber optic cable and screw hand tight
      
4. Leaf clip preparation:
    1. Check that black disc has ridges running parallel to the left and right sides of the reversible plate
    2. If white disc is dirty/not hydrophobic: lightly sand white disc with v. fine grit sand paper under diH2O until surface of disc is uniformly hydrophobic. Let air dry.
    3. Clean glass of leaf clip (in/out) if necessary
      
5. Check that prominent screw on side of leaf clip is loose and Insert fiber optic cable into leaf clip (look in window that cable end is at edge of fiber optic cable housing). Use screw to secure into place.
      
6. Plug in lamp power pack to leaf clip base and screw to secure
      
7. Turn switch at top of leaf clip to Low
      
8. Turn on lamp (press green button at back of clip) and let warm up in greenhouse environment for 10-15 minutes
<br>
##### SVC-HR1024i software for Data Collection

Recommended or go through Setup menu on machine to get Optic and Scan
timing same as below.

1. Choose Control->Setup Instrument (Alt+C+S on Windows)
    1. Find your connection: List all possible ports
        1. Bluetooth: find Bluetooth port (~COM5, see Appendix A for notes on troubleshooting connection difficulties)
        2. OR can use the USB to D-type connection (connects to base of body of spec) and find the serial port #
    2. Settings:
        1.    Optic = Fiber1
        2.    Scan Timing = 2 s (leave Coadds as default)
        3.    Integration = Auto integration
    3.    Check and correct date/time
    4. Integration scales RAW DN data = Check box 
      
2.    Choose Control->Overlap/Matching (Alt+C+O)
    1.  Preserve Overlapped Detector data (keeps whole, uncorrected file)
    2. Matching type = None
<br>
##### Leaf locations measured

Note: protocol was originally written for Oak Wilt potted seedling
experiment. If not measuring for oak wilt, follow steps to measure
healthy leaves only.

1. The widest part, between midvein and leaf margin, of the adaxial (upper surface) of a fully-sun exposed leaf
    1. When there are no symptoms on a Control, Oak Wilt, or Drought plants:
        1. Measure three (3) healthy appearing, green leaf
    2. When there are symptoms:
        1. In addition to the healthy green measurement: Select up to 3 (if available) typical symptomatic leaves and collect up to 3 additional measurements on each leaf
            1. Measure the green appearing portion of that leaf (if any)
            2. Measure the most symptomatic portion
            3. Measure the transition zone between
<br>
##### Best practices for all measurements

1. Leave lamp on whole time (or let warm up again)
        
2. White reference (Ref, then Target) each time move leaf clip (between plants and between leaves)
        
3. Avoid adjusting the angle of the leaf clip between plants (adjust the height)
        
4. Always measure adaxial (top) of leaf
        
5. NIR peak reflectance (~740nm) should be at least 35%, if isn’t make sure enough leaf (covering at least 1/3-1/2) in clip
        
6. Label white reference files with suffix WR and any bad scans with BAD
        
7. Clean leaf clip with KimWipes and EtOH between leaves to avoid spreading pathogens
        
8. If not using computer interface, can check the output in the same way as below, but need to record file log numbers
<br>
##### Data collection

1. Choose File->New (Alt+F+N)
    1. Navigate to OakWilt_local/OakWilt_data/OakWilt_spec
    2. Create a file folder for day YYYYMMDD
    3. Create basename for each new individual plant:
        1. ex: “4000” , Open
     
2. White reference 
    1. Move leaf clip near to leaf being measured
    2. Flip leaf clip to white side and close
    3. Click Reference (Alt+R)
        1. Reference radiance is total lamp output. Should be a relatively smooth, normalish curve with peak in the visible spectrum
        2. This doesn’t create a scan file (.sig), can wait and re-ref if looks weird
    4. Click Target (Alt+T)
        1. Target scan should be a relatively straight line at 100% reflectance. There will be a lot of noise at low edge of PAR (at UV), then a small blip at ~900, ~1800 where the sensors overlap
            1. any significant dips along slope after NIR peak are bad (740-900nm)
        2. ZOOM IN/OUT: draw a box or double click to zoom in, right click on plot to zoom out
    5. If looks normal, rename file (“4000_000”) as “4000_000WR” in an open file window
      
3. Leaf scan
    1. Flip lower part of leaf clip so black side is facing the window
    2. Place leaf in window (top of leaf facing lamp) and gently let clamp close on leaf
    3. Hold handheld leaf clip steady while scanning
        1. Check that reflectance meets standards
            1. If bad, label file “4000_01BAD” and find a new leaf, WR, and scan again
        2. Check that file name is correct
            1. If measuring a symptomatic leaf, use SYM code after name “4000_002SYM” (for fully symptomatic)
                1. code S-T: “4000_002S-T” (for transition zone between symptomatic and green portions of the leaf
                2. code S-G “4000_002S-G” for green portion of a symptomatic leaf
                3. Find new leaf location, WR, and scan again
                4. Open new between individuals or leaves
<br>
###### White Reference Graphs

![alt text here](images/WR%20Good.png)  
*Figure 1:* Target and reference of white reference disk in leaf clip.
Good quality.  
<br> ![alt text here](images/WR%20BAD.png) ![alt text
here](images/WR%20BAD%202.png)  
*Figures 2 & 3:* Target and reference of white reference disk in leaf
clip. Both bad quality.
<br>
###### Leaf Scan Graphs

![alt text here](images/Leaf%20Spectra%20Good.png)  
*Figure 4:* Leaf spectra of fresh leaves. Good quality.  
<br> ![alt text here](images/Dried%20Leaf%20Spectra%20Good.png)  
*Figure 5:* Leaf spectra of dried leaves. Good quality.  
<br> ![alt text here](images/Leaf%20Spectra%20Bad%20Dip.png)  
*Figure 6:* Bad quality leaf spectra. The dip at ~740-900nm is likely
due to an SVC error due to overheating.  
<br> ![alt text here](images/Leaf%20Spectra%20bad%20low.png)  
*Figure 7:* Low reflectance of leaf spectra. Explanations for this
include, but not excluded to, not enough leaf/needles/grass blades in
view of leaf clip or white, hairs or powdery mildew on leaf.
<br>
##### Data download

1. Connect to SVC-HR1024i software.
      
2. Control-> Read memory (ALT+C+R)
    1. Choose data file numbers to download
    2. Apply current/overlap matching settings (if settings = preserve and matching = none, otherwise Do NOT apply)
    3. Change output directory to wherever permanent data storage location is
    4. Output file format = YYYYMMDD_HHMM_RxxTxx
    5. Download now
      
3. Confirm download of all files before erasing
<br>
##### Post measure

1. Turn off lamp, turn off spec
      
2. Remove and charge spec and leaf clip lamp batteries
      
3. Carefully remove and put away fiber optic cable in loose loops in pelican case (unless in safe location)
    1. Then place leaf clip on side (black disc out), check that screw securing fiber optic cable is in place and leaf clip/cable can’t slide off area
<br>
### Appendix A

Bluetooth connection and troubleshooting connections

1. Establishing a Bluetooth connection
    1. In a Windows PC (~Windows 8/10), use Search bar (or right click Windows icon and “Search”)
    2. Select “Bluetooth and other devices”
    3. Turn Bluetooth On
    4. If the HR1024i device is not shown as paired and connected, choose “Add Bluetooth or other device”
        1. Select “Bluetooth” device
        2. When prompted enter the Bluetooth pin/passcode: “hr1024i”

2. Finding the correct COM port
    1. Via Bluetooth settings (most direct):
        1. Follow step 1 to get to Bluetooth settings
        2. On the right side menu, choose “More Bluetooth options”
        3. Click on the “COM ports” tab
        4. Use the listed Outgoing HR1024i COM for SVC connections
    2. Search for the “Device Manager” in the Control Panel
        1. Select “Ports”
        2. All Serial over Bluetooth connection ports are possible connections

3. Can’t establish a connection
    1. Follow step 2 above
    2. Delete any existing HR1024i connections by highlighting each and choosing “Remove”
    3. Click “Add”
    4. Select “Outgoing” [PC initiates], then choose the HR1024i device from the dropdown
