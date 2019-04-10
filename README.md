# etHANol
v3 HAN Tools: A Collection of Tools Targetting 3000/4000 Series Slim/Superslim To Allow OFW Package Manager and More


PS3Xploit Tools v3.0.1


** 20190321 - ADDED SUPPORT FOR 4.83/4.84 HFW (Hybrid Firmware) thanks joonie/habib! **

** 20190407 - ADDED SUPPORT FOR Batch Install All Packages for HAN Enabler & Debug PKG Enabler thanks joonie/habib! **

** 20190409 - Renamed old support files to han_supportfiles-482.zip **


Overview
---------

1. HAN style packages allowed (Patched external modules ecdsa)
2. PSX/PSP Free license type allowed (Patched sceNpdrmHeader check)
3. Resigned ACT.DAT & RIF allowed
4. Cinavia protection removed on HDD content
5. OFW Package Manager
6. Debug pkg file support added (optional)
7. reactPSN alternative solution for OFW users


===========================
Instructions for each tool
===========================


PS3 HAN ACT/IDPS Dumper
-----------------------
This will dump your activation file (act.dat) and your IDPS.

- Load Exploit Page

- Select Dump Path From Dropdown Box (default /dev_usb000/)

- Click "Initialize ACT/IDPS Dumper" button

- When init ready, click "Dump ACT.DAT & IDPS" button

- The browser will close automatically by default



PS3 HAN ACT/RIF Copier
----------------------
This will write back a modified act.dat and *.rif file

** It is recommended to resign all the pkgs that require Han enabler **
** Packages which are converts and packages which needs rif activation **

- Use habib's resigner tool to resign rif and create new signed_act.dat
  Place act.dat in resigner directory and drag matching rap file onto exe
  Resigner Tool Repo: https://github.com/PS3Xploit/PS3xploit-resigner

- Rename your new "signed_act.dat" to "act.dat" and place on USB drive
  ** keep original act.dat in a safe place **

- Place new rif file on USB drive as well

- Load Exploit Page

- Change RIF File Name to match your target 
  example PS2 Placeholder: 2P0001-PS2U10000_00-0000111122223333

- Select Root Path where act.dat/*.rif is located (default /dev_usb000/)

- Click "Initialize ACT/RIF Copier" button

- When init ready, click "Copy Files" button to transfer to HDD



PS3 HAN Installer
-----------------
This will copy files from USB to Flash Memory for OFW Package Manager

- Extract all files from "han_supportfiles.zip" on target USB drive root

- Load Exploit Page

- Select Root Path where these files are (default /dev_usb000/)

- Click "Initialize HAN Installer" button

- When init ready, click "Launch HAN Installation" button to copy files to flash and reboot

- Once rebooted, you can now use the HAN Enabler and Debug Package Enabler



PS3 HAN Enabler
---------------
This will initialize HAN using previously copied files to allow OFW Package Manager and other patches

- Load Exploit Page

- Click "Initialize HAN Enabler" button

- When init ready, click "Enable HAN" button to activate patches

- Once browser closes (default option) you can install HAN packages from XMB



PS3 HAN Debug PKG Enabler
-------------------------
This will allow Debug Package types to be installed

- Load Exploit Page

- Click "Initialize HAN Debug PKG Enabler" button

- When init ready, click "Enable Debug PKG" button to activate patches.

- Once browser closes (default option) you can install Debug packages from XMB.

- Reboot console before installing updates or retail/fake retail error will occur





Team PS3Xploit 2019
ps3xploit.com