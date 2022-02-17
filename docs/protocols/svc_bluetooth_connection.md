###### Author: Beth Fallon

### Goals

Connect to bluetooth on SVC.

### Bluetooth connection and troubleshooting connections

    1.  Establishing a Bluetooth connection
      a.    In a Windows PC (~Windows 8/10), use Search bar (or right click Windows icon and “Search”)
      b.    Select “Bluetooth and other devices”
      c.    Turn Bluetooth On
      d.    If the HR1024i device is not shown as paired and connected, choose “Add Bluetooth or other device”
        i.  Select “Bluetooth” device
        ii. When prompted enter the Bluetooth pin/passcode: “hr1024i”
    2.  Finding the correct COM port
      a.    Via Bluetooth settings (most direct):
        i.  Follow steps 1a-b to get to Bluetooth settings
        ii. On the right side menu, choose “More Bluetooth options”
        iii.    Click on the “COM ports” tab
        iv. Use the listed Outgoing HR1024i COM for SVC connections
      b.    Search for the “Device Manager” in the Control Panel
        i.  Select “Ports”
        ii. All Serial over Bluetooth connection ports are possible connections
    3.  Can’t establish a connection
      a.    Follow steps 2.a.i – 2.a.iii above
      b.    Delete any existing HR1024i connections by highlighting each and choosing “Remove”
      c.    Click “Add”
      d.    Select “Outgoing” [PC initiates], then choose the HR1024i device from the dropdown
