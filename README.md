# PS4_db_rebuilder_6.72_7.02_7.55
If you rebuild your PS4 database, all your installed FPKGs can disappear.
This script will build a new database, and your FPKGs will reappear.
Downsides: Custom folders in your home menu will be gone, and all recovered FPKGs will now have the same install date.

## Requirements
- Python (preferably 3.0+)

## How to use:
1) Firmware 5.05: recursively clone the original repo or download a [Release](https://github.com/Zer0xFF/PS4_db_rebuilder/releases)  
Firmwares 6.72, 7.02, and 7.55: recursively clone this repo or download a [Release](https://github.com/hippie68/PS4_db_rebuilder/releases)
2) Start an FTP server on the PS4 and open a command line on your computer.
3) If you use the FTP payload: `python3 fix_db.py PS4_IP`  
   If you use GoldHEN: `python3 fix_db_goldhen.py PS4_IP`  
   If you use the PS4 Xplorer app: `python3 fix_db_ps4xplorer.py PS4_IP`
4) Wait for the script to finish, then logout of the PS4 user without closing the browser.
5) Log back in and all your games should be there again.
