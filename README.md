ACST
====
Public releases for ACSaveTool  
For downloads, please go to the [Release](https://github.com/linuslin0/ACST/releases) page.

## Features
- Convert saves between different encryption IDs.
- Support for various game saves.
- Process multiple files simultaneously.
- Auto-detect game titles and decryption/encryption keys for certain saves.
- Automatically lookup save paths for supported titles.

## Usage
1. Open save files by clicking the `Open` button or drag and drop saves into the app window.
2. Select the appropriate game title, or leave it as `[Auto Detect]` (only works for certain game saves).
3. Input the `Decryption ID` for the loaded saves, or check the `Detect` box.
4. Input the `Encryption ID` for the new saves, or click the button on the right to open a test save for encryption key detection.
5. Click the `Convert` button. The original saves will be backed up in the `acst_backup` folder.
6. Copy the converted saves to the corresponding game save location. You may need to temporarily disable cloud save sync before launching the game.

Refer to [FAQ](FAQ.md) for common issues and tips.

## Supported Games
Supported game saves and their decryption/encryption ID type:
```
Assassin's Creed Shadows           // Account ID
Assassin's Creed Mirage            // Account ID
Assassin's Creed Valhalla          // Account ID
Assassin's Creed Odyssey           // Account ID
Assassin's Creed Origins           // Account ID
Assassin's Creed Syndicate         // Account ID
Assassin's Creed Rogue             // Game key
Assassin's Creed Unity             // Account ID
Assassin's Creed Liberation HD     // Game key
Assassin's Creed IV Black Flag     // Game key
Assassin's Creed III Remastered    // Account ID
Assassin's Creed III               // Game key
Assassin's Creed Revelations       // Account (legacy) username
Immortals Fenyx Rising             // Account ID
```
Note: Use `Account ID` and `Account (legacy) username` in lowercase; `Game key` in uppercase.

## Requirements
Windows 10 or later (64-bit).

## Disclaimer
This software is provided "AS IS" for research purposes only. Commercial use is prohibited. The author is not liable for any save data corruption or loss that may occur from using this software.

## Credits
- [Ubisoft](https://www.ubisoft.com/) for all the fun.
- [Linus L.](https://github.com/linuslin0) for writing this tool.
- machine4578 for testing and feedback.
