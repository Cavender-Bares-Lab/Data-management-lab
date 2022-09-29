---
hide: footer
---

### HPLC Summary

Please see below for the following protocols for HPLC use

* [Pigment Calibration](https://cavender-bares-lab.github.io/Data-management-lab/protocols/pigment_calibration/)
    * Steps to determine pigment concentration from pigments Chl a and b, beta-carotene, and lutein. This step is necessary when DAD lamp is changed and pigment values don't come in the same ranges as previous calibration. **Please note:** this is not a systemic calibration, this calibration will change the fitted lines for pigment concentration. 
    * Current pigment equations (Last update - 9.29.2022):
        + Neoxanthin -> $Area = 98.2872684x + 0$
        + Violaxanthin -> $Area = 107.0247492x + 0$
        + Antheraxanthin -> $Area = 118.748979x + 0$
        + Lutein -> $Area = 122.088997x +0$
        + Zeaxanthin -> $Area = 128.514202x + 0$
        + Chlorophyll b -> $Area = 36.0649618x +0$
        + Chlorophyll a -> $Area = 19.6773059x + 0$
        + Beta-carotene -> $Area = 121.044949x + 0$

* [Pigment Extraction](https://cavender-bares-lab.github.io/Data-management-lab/protocols/pigment_extraction)
    * Detailed steps to process leaf samples for pigment extraction
    * [Extraction Template](https://docs.google.com/spreadsheets/d/1QPHQzdJdP6NZR6k2inDp37g0YwTTxf9h/edit?usp=sharing&ouid=117278050553426340443&rtpof=true&sd=true)
      
* [Run Samples](https://cavender-bares-lab.github.io/Data-management-lab/protocols/hplc_run_samples)
    * Protocol to run samples on the HPLC (High Performance Liquid Chromatography) machine.
    * [File Template]
      
* [ImageJ](https://cavender-bares-lab.github.io/Data-management-lab/protocols/hplc_imagej)
    * Determine leaf area of needles and leaves (for leaves that cannot be hole punched).
    * [Leaf Area Template]()

* [Export & Process Data](https://cavender-bares-lab.github.io/Data-management-lab/protocols/hplc_export_data)
    * Steps to export pigment area and concentration. Use an R script to compile csv files to include pigment concentration values and metadata.
    * [File Template]()