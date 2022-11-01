---
hide:
  - footer
---

# Sartorius Balance COM Port Settings

### Goal
To detail steps to connect Sartorius Balance with Computer to measure hydraulic conductivity.

### Notes
+ Balance, computer and software all must match
    + Balance is hardest to change, so use defaults unless necessary
+ You need a serial-port-to-USB cable.
+ Download [conduct.verX.xls](https://docs.google.com/spreadsheets/d/19Gr1bHsw4f4eCfuZ9XkLv3EeIw5RaviX/edit?usp=sharing&ouid=117278050553426340443&rtpof=true&sd=true) file 
    + Open it in excel, enabling the macros.
+ Software: [StrokeReader ActiveX](https://strokescribe.com/en/serial-port-download.html)

### Settings
+ Baud rate (bits per second): 1200
+ Data bits: 7
+ Parity: odd
+ Stop bits: 1
+ Flow control: Hardware (may also be called hardware handshake CTS)

#### Computer Settings
1. Open "Device Manager"

2. Expand "Ports (COM & LPT)"

3. Find your port (should be USB converter)

4. Note port number (varies by device)

5. On "Port settings" tab, change settings to match above.

#### Software Settings
###### Option A
1. Make sure "Developer" ribbon is enabled in excel.

2. Click "View Code"

3. Under the submodule "connect()", change settings
    1. Will likely only need to change "Sartorius Connection Port"

###### Option B
1. Make sure "Developer" ribbon is enabled in excel.

2. Click "Design Mode" - little box that says "COM" should appear

3. Select little box & open "Properties" (on ribbon or right-click menu). Make changes and close.

4. Turn off "Design mode" to use tool.