---
hide: footer
---

###### Author
Hilary Major

###### Updated
22 February 2022 by Cathleen Lapadat

### Goal

This protocol details the steps to process images of leaf skeletons and tracing for VLA analysis.

### Supplies/Equipment Needed

- ImageJ software

### ImageJ

###### Crop Images

1. Crop the individual leaf images from the leaf scans. 

2. Save as .tif file.

###### Create a VLA square

1. Open leaf tif file with ImageJ.

2. Choose the area you like for cropping.
    1. Squares are 236 pixels squared (236 pixels = 1 cm)
    2. It should be an average section of the leaf--representative of the vein density away from the first order of veins. 
    3. Do not include the midrib vein unless the leaf is so small that it's necessary.
    4. Scroll in at least 600x magnification to ensure the contrast between the vein and leaf tissue has clear resolution that you can visually detect.
        1. '+' and '-' are also useful for zooming in and out, respectively.

3. Set scale
    1. Click Analyze, "set scale".
    2. Write 
        1. Distance in pixels: 1 
        2. Known distance: 1
        3. Pixel aspect ratio: 1.0
        4. Unit of length: pixel
        5. Click "Global".
        6. OK

    3. Use the rectangle button and choose a square. 
        1. Hold onto ctrl+shift to create a square and move your cursor to the desired selection.
        2. The selection size appears in the status bar. Always keep at exactly 236 pixels/1 cm per side. You may need to zoom in until you can get it precisely to 236 pixels.

    4. Use Image -> Crop (ctrl+shift+x) to crop the square.

    5. Save cropped image as .tif file. 

### Trace

1. Open leaf square in ImageJ.

2. Right click on the "*Straight*, segmented or freehand lines, or arrows" tool button.
    1. Choose "segmented line".

3. Left click on the image to start tracing the veins. Left click to create a new segment and angle of the line. Double click to complete the line.

4. Click "t"  to add line to ROI Manager
    1. Alternatively, click on: 
        1. Analyze 
        2. Tools
        3. ROI Manager
        4. Add [t]
            
5. On the ROI manager window, click on "Show All" and "Labels".
    1. View all numbered lines.

6. Save regularly to not lose work.
       
7. Repeat steps 4 and 6 until tracing of image is complete.

### Calculate VLA

1. Go to the ROI Manager 
    1. Click ‘Measure -> Edit, 
    2. Select all and copy
    3. Paste the values in an excel file to calculate the length sum, which is set in pixels.
      
2. The formula for VLA in $mm/mm^2$ is ${sum\;vein\;length \over (square\;side\;length)^2} = {B1 \over C1^2}$
    1. Convert pixel vein length to mm.
    2. Square side length is 10 mm.
        1. For example
            - $6500 = sum\;pixel\;vein\;length$  
            - ${6500\;pixels \over 23.6\;pixels/mm} = 275.423729$  
            - ${275.423729mm \over (10mm)^2} = 2.75423729 mm/mm^2$

### Notes/Tips

#####Image J

1. For any adjustments:
    1. Choose the line of interest.
    2. Click "Update". Click "Delete", if removal is preferred.
    3. Adjust as needed. Points are movable to shorten and lengthen line or adjust angle of lines.

2. When resuming work after shutdown:
    1. Open file.
    2. Go to:
        1.    Image
        2.   Overlay
        3.  To ROI Manager (this will add your already created lines into the ROI manager.)

3. Adjust the contrasts to better see if you are looking at a 4th order vein or a blobby artifact from scanning. 
    1. Image
    2. Adjust
    3. Brightness/Contrast

4. Shows negative image with the edges of veins in green against black.
    1. Process
    2. Find Edges
        
5. Enhance images and contrast
    1. Process
    2. Sharpen
        1. If you make any marks or lines while it is in contrast, cannot save the changes and revert (Ctrl+shift+R) back to the original image.

### Reference

[Lawren Sack, Marissa Caringella, Christine Scoffoni, Chase Mason, Michael Rawls, Lars Markesteijn, Lourens Poorter. 2014. Leaf Vein Length per Unit Area Is Not Intrinsically Dependent on Image Magnification: Avoiding Measurement Artifacts for Accuracy and Precision, Plant Physiology, Volume 166, Issue 2, October 2014, Pages 829–838, https://doi.org/10.1104/pp.114.237503](http://www.plantphysiol.org/content/plantphysiol/166/2/829.full.pdf)
