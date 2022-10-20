---
hide: footer
---

# HPLC Summary

Please see below for the following protocols for HPLC use

* [Pigment Calibration](https://cavender-bares-lab.github.io/Data-management-lab/protocols/pigment_calibration/){:target="\_blank"}
    * Steps to determine pigment concentration from pigments Chl a and b, beta-carotene, and lutein. This step is necessary when DAD lamp is changed and pigment values don't come in the same ranges as previous calibration. **Please note:** this is not a systemic calibration, this calibration will change the fitted lines for pigment concentration. 
    * Current pigment equations (Last update - 10.18.2022):
        + Neoxanthin -> $Area = 97.757x + 0$
        + Violaxanthin -> $Area = 106.41x + 0$
        + Antheraxanthin -> $Area = 118.11x + 0$
        + Lutein -> $Area = 121.43x +0$
        + Zeaxanthin -> $Area = 127.79x + 0$
        + Chlorophyll b -> $Area = 37.353x +0$
        + Chlorophyll a -> $Area = 20.297x + 0$
        + Beta-carotene -> $Area = 129.05x + 0$

* [Pigment Extraction](https://cavender-bares-lab.github.io/Data-management-lab/protocols/pigment_extraction){:target="\_blank"}
    * Detailed steps to process leaf samples for pigment extraction
    * [Extraction Template](https://docs.google.com/spreadsheets/d/1QPHQzdJdP6NZR6k2inDp37g0YwTTxf9h/edit?usp=sharing&ouid=117278050553426340443&rtpof=true&sd=true){:target="\_blank"}
      
* [Run Samples](https://cavender-bares-lab.github.io/Data-management-lab/protocols/hplc_run_samples){:target="\_blank"}
    * Protocol to run samples on the HPLC (High Performance Liquid Chromatography) machine.
    * [File Template](){:target="\_blank"}
      
* [ImageJ](https://cavender-bares-lab.github.io/Data-management-lab/protocols/hplc_imagej){:target="\_blank"}
    * Determine leaf area of needles and leaves (for leaves that cannot be hole punched).
    * [Leaf Area Template](){:target="\_blank"}

* [Export & Process Data](https://cavender-bares-lab.github.io/Data-management-lab/protocols/hplc_export_data){:target="\_blank"}
    * Steps to export pigment area and concentration. Use an R script to compile csv files to include pigment concentration values and metadata.
    * Path to script: LAB-cavender\1-Important Lab Information\R Scripts\HPLCimport.R
    * [SampData Template](){:target="\_blank"}