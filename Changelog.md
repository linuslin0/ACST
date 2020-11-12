ACST Changelog
==============

#### v2.4.0
- Added support for ACValhalla
- Added input validation for Encryption/Decryption ID fields
- Minor GUI tweaks

#### v2.3.1
- Added support to convert ACLHD save to ACLRM (choose ACLHD & double click `Encryption ID` label)
- Show output file name if different from the original file
- Adjusted release package structure

#### v2.3.0
- Added support for loading certain non-standard saves (*.sav)
- Moved backup save location to separate `acst_backup` folder
- Fixed test save file processing logic
- Performance optimization
- Miscellaneous GUI issue fixup

#### v2.2.0
- Disable detection feature if user choose game title as ACR
- Added support for Steep saves
- Changed default file open path to user profile directory
- Reduced release package size
- Some cleanup and minor GUI issue fixes

#### v2.1.1
- Additional checking for the test save path to prevent folder or file with same name been used as test save
- Relaxed filtering for decryption/encryption ID input to allow underscores (_) and dots (.)

#### v2.1.0
- Added support for detect decryption key from test save file
- Fixed issue on GUI stopping processing saves when decryption and encryption key are both given
- Added showing execution time on GUI
- Added extra checking for valid save detection

#### v2.0.0
- First public release

