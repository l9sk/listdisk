# listdisk
## List and Query Physical Disk Properties on Microsoft Windows based systes.

Displays vendor, product, bus type, serial number, disk GUIDs used by Microsoft Failover Cluster, BTL, trim support, etc. The utility will work even if VDS is hung or inoperable. 

Developer example of how to list physical disks in Windows NT systems by querying NT Namespace for PhysicalDrive objects and query physical disk for properties via IOCTL.

Example output:

```
PhysicalDrive0:
  Vendor   : HP
  Product  : LOGICAL VOLUME
  Serial   :
  Removable: False
  BusType  : RAID
  Status   : Online
  Size     : 111.8 GB
  Layout   : GPT
  DiskID   : {8FAFB531-7334-4334-A64F-D61C90BF5060}
  HBTL     : 0:0:4:0

PhysicalDrive1:
  Vendor   : ATA
  Product  : SAMSUNG MZ7KM960
  Serial   : S2NFNX0H400050B
  Removable: False
  BusType  : SAS
  Status   : Online
  Size     : 894.3 GB
  Layout   : GPT
  DiskID   : {1A539AB6-76F8-470C-995F-105B314AF1B5}
  Trim     : Supported
  HBTL     : 1:2:1:1

PhysicalDrive2:
  Vendor   : NVMe
  Product  : Samsung SSD 950
  Serial   : 0000_0000_0000_0000.
  Removable: False
  BusType  : NVME
  Status   : Online
  Size     : 476.9 GB
  Layout   : GPT
  DiskID   : {D0C45AEA-586A-4DF2-A657-6C8E3C0A487A}
  Trim     : Supported
  HBTL     : 2:0:0:0

PhysicalDrive3:
  Vendor   : (n/a)
  Product  : SATADOM-SL 3ME
  Serial   : TW02PTHF482935730153
  Removable: False
  BusType  : SATA
  Status   : Online
  Size     : 59.6 GB
  Layout   : GPT
  DiskID:  : {8EF1BEE1-83F1-40DB-B049-6DD7126FE619}
  Trim     : Not Supported
  HBTL     : 0:5:0:0

PhysicalDrive4:
  Vendor   : ATA
  Product  : INTEL SSDSC2BB80
  Serial   :   PHWL5273045K800RGN
  Removable: False
  BusType  : SAS
  Status   : Online
  Size     : 745.2 GB
  Layout   : GPT
  DiskID:  : {042A9DF8-2992-4C4E-B99D-A3F1755D84AF}
  Trim     : Supported
  HBTL     : 1:0:3:0
```