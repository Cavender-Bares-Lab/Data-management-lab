---
hide: footer
---

###### Author
Beth Fallon

### Goals

Connect to bluetooth on SVC.

### Bluetooth connection and troubleshooting connections

1. Establishing a Bluetooth connection
    1. In a Windows PC (~Windows 8/10), use Search bar (or right click Windows icon and “Search”)
    2. Select “Bluetooth and other devices”
    3. Turn Bluetooth On
    4. If the HR1024i device is not shown as paired and connected, choose “Add Bluetooth or other device”
        1. Select “Bluetooth” device
        2. When prompted enter the Bluetooth pin/passcode: “hr1024i”
2. Finding the correct COM port
    1. Via Bluetooth settings (most direct):
        1. Follow steps 1 to get to Bluetooth settings
        2. On the right side menu, choose “More Bluetooth options”
        3. Click on the “COM ports” tab
        4. Use the listed Outgoing HR1024i COM for SVC connections
    2. Search for the “Device Manager” in the Control Panel
        1. Select “Ports”
        2. All Serial over Bluetooth connection ports are possible connections
3.  Can’t establish a connection
    1. Follow step 2 above
    2. Delete any existing HR1024i connections by highlighting each and choosing “Remove”
    3. Click “Add”
    4. Select “Outgoing” [PC initiates], then choose the HR1024i device from the dropdown
