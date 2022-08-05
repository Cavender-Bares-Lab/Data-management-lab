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
    *  Apps: FAB1 Growth and Reproduction and FAB2 Growth and Reproduction
    *  Go to Settings: 
        - Sort by: Date/Time Created
        - Ascending: Turn On
    *  When viewing **All Records**, the order of the lines are Listing number, Plot, Row, Column, Individual ID  
        - e.g. 1, 1, 1, 1, QUAL-2016-1  

2. Select **Filter**    
    * **+ Add Rule**   
        - Choose **Survey**
            * Operator: **Equals** or **Contains**; Value: **Yes**
                - Values are case sensitive
                - For proper filtering, confirm that you have 31500 (FAB2) or 8960 (FAB1) records showing
        - Choose **Plot**
            * Operator: **Equals**; Value: Chosen plot to survey
                - For proper filtering, confirm that you have 100 (FAB2) or 64 (FAB1) records

3. Locate tree
    * When located, choose the correct line in fulcrum app, and scroll down. Click **Growth**  

4. Measurements
    * At the bottom, choose **+ Record**
        - **User initials**
            * Enter your initials
        - **Measurement Date**
            * defaults to current date
        - **Dead/Missing**
            * **Yes**: The tree is dead
                + If Yes, **SAVE**
                + On main page, respond to the following accordingly:
                        * Reproduction complete: Yes
                        * Needs Reproduction Count: No
            * **No**: The tree is alive
        - **Height**: cm
            * From the ground to the highest living bud
        - **Diameter**: mm
            * Basal diameter is measured at 5cm
        - **DBH**: mm
            * Measured at 137 cm in height
        - **Above/Below**
            * If there is an abnormality at 5cm or 137cm, measure diameter/dbh above or below
        - **Notes**
            * not required but recommended if you notice anything of significance that may have impacted the individual's growth measurements
                - e.g. leading stem is dead, parts of tree is yellowing, etc
        - **Photos**
            * Not required
    * **Save**
        - fulcrum app was created with several requirement rules, you must fill in the requirements in order to save properly. 

5. Reproduction
    * On main page of the individual, if responses for the two below are empty, continue to **Reproduction** field
        * Reproduction complete 
        * Needs Reproduction Count 
    * **Reproduction** field:
        * Survey date
            - defaults to current date
        * Reproducing
            - If **Yes**, continue to **Sub_RC**
            - If **No**, choose No and SAVE
                - Fill in the following on the main page:
                    * Reproduction complete: Yes
                    * Needs Reproduction Count: No 
        * Sub_RC
            - Choose N/A
        * Reproduction Count
            - Skip; reproduction count will be done after growth measurements are completed
        * Reproduction Type
            - Choose flower, fruit, or cone
        * SAVE
            - On main page, fill in the following:
                * Reproduction complete: No 
                * Needs Reproduction Count: Yes 
            
6. At the end of the day, **sync** the app
    * Choose the sync button at the right hand corner
      - sync button looks like a refresh button
            
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
