---
hide: footer
---

# Measuring Leaf Area Protocol
###### Author
Cavender-Bares Lab

###### Updated
21 October 2022

### Goal

The goal of this protocol is to standardize the measurements of leaf area using scanned leaves and Image J.

### Requirements

- Scanner
- Image J software

### Steps

##### Scanning Leaves

1. Place leaf and label face down on scanner. The goal is to have leaf and label visible in photo. If scanning multiple leaves in a single photo, ensure no overlaps. Include a clear ruler on the scanner that can be seen in each image.

2. Enter EPSON Scan application. 
    1. Set file name prefix and destination by clicking the folder on the bottom of the right window. 

3. Click Scan. Once scanned the photo should appear in its folder; open the photo and look to see if it was scanned appropriately. Return each leaf to its appropriate envelope. Once all leaves are scanned, place them in the drying oven for a minimum of three days before dry-weighing.

##### Image J

1. Open program Image J application. 
    1. Select File open > Import > Image Sequence
    2. Open the folder with your leaf scans. ImageJ can stack up to 60 images at a time.

2. Select the Line tool. 
    1. Draw a segment on the ruler of a certain length (ex. 8 cm). 
    2. Select Analyze > Set Scale. 
    3. Enter the certain length under Known distance, cm for Unit of length, and check Global. Click Ok.

3. Select Analyze > Set measurements. 
    1. Make sure Area, Perimeter, and Feret’s diameter are checked. Choose Ok.

4. Select Image > Adjust > Color Threshold. 
    1. Tweak the color and brightness thresholds so that only the leaves are cleanly selected, using a red background on the scanner makes this easier. 
    2. Once your threshold is established click Stack. This will apply your threshold to every image in the sequence.

5. Click on the Wand tool and select one of the leaves. It should highlight the perimeter of the leaf in yellow. If a leaf is touching another it will trace around everything. You will need to use the draw tool to manually trace each leaf.

6. Once the leaf is highlighted select Analyze > Measure (Ctrl-M). A new window will appear with the measurements. If a leaf is damaged or heterogeneous it may require multiple selections that will need to be added together. 

7. Copy your measurements into an excel spreadsheet with appropriate labels and save.

###### Notes/Tips
It is ideal to stack with similar types of leaves. Different types of leaves/needles will require different thresholds so should not be stacked together.