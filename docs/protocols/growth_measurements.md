---
hide:
  - footer
---

### Background
This protocol details fall growth measurements for FAB 1 and FAB 2 through Fulcrum App.

### Notes
- **ATTENTION TO SUPERVISOR**: Confirm that the requirements are reinstated if it was removed previously for the reproduction survey.

### Preparation

1. Download Fulcrum App on your mobile device

2. Use the log in details provided

### Detailed Steps

1. Open Fulcrum App on your phone  
    1.  Apps: FAB1 Growth and Reproduction and FAB2 Growth and Reproduction
    2.  Go to Settings: 
        1. Sort by: Date/Time Created
        2. Ascending: Turn On
    3.  When viewing **All Records**, the order of the lines are Listing number, Plot, Row, Column, Individual ID  
        1. e.g. 1, 1, 1, 1, QUAL-2016-1  

2. Select **Filter**    
    1. **+ Add Rule**   
        1. Choose **Survey**
            1. Operator: **Equals** or **Contains**; Value: **Yes**
                1. Values are case sensitive
                2. For proper filtering, confirm that you have 31500 (FAB2) or 8960 (FAB1) records showing
        2. Choose **Plot**
            1. Operator: **Equals**; Value: Chosen plot to survey
                1. For proper filtering, confirm that you have 100 (FAB2) or 64 (FAB1) records

3. Locate tree
    1. When located, choose the correct line in fulcrum app, and scroll down. Click **Growth**  

4. Measurements
    1. At the bottom, choose **+ Record**
        1. **User initials**
            1. Enter your initials
        2. **Measurement Date**
            1. defaults to current date
        3. **Dead/Missing**
            1. **Yes**: The tree is dead
                1. If Yes, **SAVE**
                2. On main page, respond to the following accordingly:
                    1. Reproduction complete: Yes
                    2. Needs Reproduction Count: No
            2. **No**: The tree is alive
        4. **Height**: cm
            1. From the ground to the highest living bud
        5. **Diameter**: mm
            1. Basal diameter is measured at 5cm
        6. **DBH**: mm
            1. Measured at 137 cm in height
        7. **Above/Below**
            1. If there is an abnormality at 5cm or 137cm, measure diameter/dbh above or below
        8. **Notes**
            1. not required but recommended if you notice anything of significance that may have impacted the individual's growth measurements
                1. e.g. leading stem is dead, parts of tree is yellowing, etc
        9. **Photos**
            1. Not required
    2. **Save**
        1. fulcrum app was created with several requirement rules, you must fill in the requirements in order to save properly. 

5. Reproduction
    1. On main page of the individual, if responses for the two below are empty, continue to **Reproduction** field
        1. Reproduction complete 
        2. Needs Reproduction Count 
    2. **Reproduction** field:
        1. Survey date
            1. defaults to current date
        2. Reproducing
            1. If **Yes**, continue to **Sub_RC**
            2. If **No**, choose No and SAVE
                1. Fill in the following on the main page:
                    1. Reproduction complete: Yes
                    2. Needs Reproduction Count: No 
        3. Sub_RC
            1. Choose N/A
        4. Reproduction Count
            1. Skip; reproduction count will be done after growth measurements are completed
        5. Reproduction Type
            1. Choose flower, fruit, or cone
        6. SAVE
            1. On main page, fill in the following:
                1. Reproduction complete: No 
                2. Needs Reproduction Count: Yes 
            
6. At the end of the day, **sync** the app
    1. Choose the sync button at the right hand corner
        1. sync button looks like a refresh button
            
### Brief Summary of Fulcrum App Steps
```
1. Add filters for Survey and Species Code

2. Choose individual

3. Go to Reproduction

4. + Record

5. Growth requirements
    a. User initials
    b. Measurement Date
    c. Dead/Missing
    d. Height (cm)
    e. Diameter (mm)
    f. DBH (mm)
    g. Above/Below
    h. Notes
    i. Photos
    j. SAVE

6. Reproduction   
    a. Survey date
    b. Reproducing
    c. Sub_RC
    d. Reproduction Count: SKIP
    e. Reproduction Type
    f. SAVE

7. Main page requirements
    a. Reproduction complete
    b. Needs Reproduction Count
    c. SAVE
    
8. Repeat steps 2-7

9. Sync
```
