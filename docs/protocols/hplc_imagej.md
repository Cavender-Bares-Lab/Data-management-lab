---
hide: footer
---

# HPLC - ImageJ Protocol
##### Author
Anna Schweiger
###### Updated
31 January 2022 by Cathleen Lapadat

### Goal

This protocol details the steps to process images of leaf samples measured for HPLC analysis and applicable for SLA.

### Supplies/Equipment Needed

- ImageJ software

### ImageJ

1. Open image: file - open

2. Set scale:
    1. Click line:
        1.  Draw line from one side of the image to the other
    2. Analyze - set scale: 
        1.  For inner line of boat 0.0028m, set to global, okay

3. Identify leaf
    1. Image - adjust - color threshold 
        1.  Unselect black background
        2. play with hue, saturation, brightness: leaf should be red
    2. close color threshold

4. Calculate area of leaf
    1. Analyze - analyze particles:
        1.    Set lower size limit - Infinity
        2.   Show: outlines
        3.  Display results
        4.   Exclude on edges
        5.    Include holes
        6.   Summarize
5. Add area to excel
    1.  Make sure outlines are of leaf/needle.
