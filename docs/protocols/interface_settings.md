---
hide: footer
---

### Goals
Documents multiple examples of settings for Hansatech fluorometer. Settings are dependent on your goals.

#### Mid-day (oleiodes project)

    1. Actinic light, equivalent to ambient light: 
        a.  Set value between 0 and 50 (steps from 0 to 3000 micromoles m-2s-1)🡪probably keep at 50, check readout
        b.  Need 10 sec of actinic light for measurement
    2. Pulse: saturating light to leaf:
        a.  Check peak fluorescence by pulse from 0 to 100
        b.  Choose the saturating pulse, without torturing plant with high light (at beginning of plateau value)
    3. Width of pulse: length of pulse
        a. .7 is what Jose uses, check that additional pulse exposure doesn’t change fluorescence adjust to maximize

#### Yield (oleoides)

In general,there is an initial high yield light exposure, then 10 sec of actinic light, then another saturating pulse
    
    1. Gain: 50 (check glossary)
    2. Mod: 2 (modulation, check manual if need to adjust)
    3. Log: 1 (1= log data, 0=no logging)
    4. FVFM: ##,##,##
        a. 2.5 duration of element
        b. 60 intensity of saturating pulse (adjust as needed)
        c. .7 width
    5. ACT: 43 actinic
    6. WAIT: 10 (seconds of waiting)
    7. ePS2: 
        a. 2.5 duration of element
        b. 60 pulse
        c. .7 width
    8. Beep 1=yes beep
    
#### Dark-adapted (ACE)

    1. Gain: 50 (check glossary)
    2. Mod: 2 (modulation, check manual if need to adjust)
    3. Log: 1 (1= log data, 0=no logging)
    4. FVFM: ##,##,##
        a. 2.5 duration of element
        b. 60 intensity of saturating pulse (adjust as needed)
        c. .7 width
    8. Beep: 0.5
    
#### Light-adapted (ACE)

    1. Gain: 50 (check glossary)
    2. Mod: 2 (modulation, check manual if need to adjust)
    3. Log: 1 (1= log data, 0=no logging)
    4. ACT: 43 actinic
    5. WAIT: 10 (seconds of waiting)
    7. ePS2: 
        a. 2.5 duration of element
        b. 50 pulse
        c. .7 width
    8. Beep: 0.5