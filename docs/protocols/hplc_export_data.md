---
hide: footer
---

# HPLC - Export Data Protocol
### Introduction
The protocol outlines the steps to integrate, export, and process HPLC pigment data.

### Quick Guide
1. Integration
    1. Add lines to pigment peaks.
        1. Save
    2. Identify each peak with correct pigment.
    3. Export Report
    
2. Compile CSV files into one folder

3. Run HPLCimport R script to output calculations
    1. Need SampData csv file

### Details Steps

##### Integration
1. Open ChemStation (offline) software.

2. On the left hand side, click on "Data Analysis".

3. Click on "Integrate".

4. Navigate to your folder on the left hand side. Click on your first sample in the sequence list.

5. Click on the "" icon to remove automated integrations. Lines under the pigment peaks will be removed.

6. Zoom in to your first 3 peaks (Neoxanthin, Violaxanthin, and Antheraxanthin, if present) by clicking and dragging to view your desired peaks.
    1. Look at your first peak and decide where the peak begins to increase (start point) and when it decreases and plateaus (end point). This is where you draw your line. Choose the "integrate" icon and carefully click on the start point and click again at the end point. Repeat with the remaining to peaks.

7. Zoom out and then zoom in to the remaining peaks (Lutein, Zeaxanthin, if present, Chl b, Chl a, and Beta-carotene).
    1. Draw your lines from the start and end point for each peak.
    2. For overlapping pigments, which is normal for Lutein and zeaxanthin, draw the line from the start and end point of both pigments. Click on the "splitting icon". Split at the center of the plateau between peaks.

8. Click save icon.

9. Click on "Calibration".
    1. Ensure the [current equations]() match the equations listed in each pigment graph.
    2. You will need to change the retention times of each pigment to identify the peaks.
        1. Look at your first peak, Neoxanthin. Click on the Neoxanthin retention time and enter the time of the peak. You should see Neoxanthin labeled above your peak. Continue entering the retention times for each peak and confirm that each peak is labeled with the correct pigment.
            1. It is important to label the peaks. If skipped, the pigment values will not be exported.

##### Export
1. Click on Report. Then click on Specify Report.

2. Choose the following: 
    1. Destination: File
    2. File Settings:
        1. Add check to "Unique pdf file name"
        2. Enter file name as sample's Unique ID
        3. Add checks to pdf, csv, and txt. Press Okay.

3. Click on Report. Then click Export Report.

4. Repeat Integration and Export steps for each sample until complete.
        
##### Compile CSV Files
1. Create and name folder for the CSV files.

2. For each sample folder, move the CSV file to the newly created folder.
    1. Example of the exported CSV files.
    
##### Run R Script
1. Script is stored in the shared drive
    1. Path: LAB-cavender\1-Important Lab Information\R Scripts\HPLCimport.R
    2. The script compiles the csv files, adds the metadata, and calculates concentration values of each pigment.

2. Edit the path of your files in the script.

3. You will need a csv file with your metadata. This file is named "Sampdata.csv" in the script.
    1. [csv file template](https://drive.google.com/file/d/1rqFtI-C_uq54s5Or6KkV3JUGJjqRK10f/view?usp=sharing){:target="\_blank"}
        1. [README](https://drive.google.com/file/d/1t0TWe5EMjUYtfu1-10WNYmPmvX951Z8G/view?usp=sharing){:target="\_blank"} file for column names and calculations.

##### Data information
1. There are multiple ways to report the pigment values. The script outputs several different values:
    1. ng.mg.Wet = ng of pigment/mg of wet sample weight
    2. ng.mg.Dry = ng of pigment/mg of dry sample weight
    3. ug = pigment amount in ug in leaf hole punch
    4. umol = pigment amount in umol in leaf hole punch
    5. umol.m2 = pigment amount (umol)/leaf area