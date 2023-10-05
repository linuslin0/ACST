ACST
====
Public releases for ACSaveTool  
For downloads, please refer to [Release](https://github.com/linzhouyu/ACST/releases) page.

#### Features:
- Convert saves between different encryption IDs.
- Support various game saves.
- Multiple file processing.
- Auto-detect game titles, decryption/encryption key for certain saves.
- Auto save path lookup for supported titles.

#### Usage:
1. Open save files by clicking `Open` button, or drag and drop to the app window.
2. Choose the matching game title, or leave as `[Auto Detect]` (only works for certain game saves).
3. Enter `Decryption ID` for loaded saves, or use the `Detect` checkbox.
4. Enter `Encryption ID` for new saves. Or click the button on the right to open a test save for encryption key detection.
5. Click `Convert` button, original saves will be backed up in `acst_backup` folder.
6. Copy the converted saves to the corresponding game save location. You might need to temporarily disable cloud save sync before starting the game.

Supported game saves and their decryption/encryption ID type:
```
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

#### Requirements:
Windows 10 or later, x64 edition.

#### Disclaimer:
This software is provided "AS IS" and for research purposes only. Commercial use prohibited.
The author is not responsible for any data corruption that may be caused by using this software.

#### Bug report:
Please open issues [here](https://github.com/linuslin0/ACST/issues).

#### Credits:
- [Ubisoft](https://www.ubisoft.com/) for all the fun.
- [Linus L.](https://github.com/linuslin0) for writing this tool.
- machine4578 for testing and feedback.
