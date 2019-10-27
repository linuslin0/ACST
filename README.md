ACST
====
Public releases for ACSaveTool  
For downloads, please refer to [Release](https://github.com/linzhouyu/ACST/releases) page.

#### Feature:
- Convert saves between different encryption IDs.
- Support various game saves.
- Multiple files processing at once.
- Auto detect game title, decryption/encryption ID for certain saves.

#### Usage:
1. Open save files by clicking `Open` button, or drag and drop to app window.
2. Choose the matching game title, or leave as `[Auto Detect]`.
3. Enter `Decryption ID` for the loaded saves, or select `Detect` checkbox.
4. Enter `Encryption ID` needs to be converted to, or use that weird button, open a test save to detect encryption ID.
5. Click `Convert` button, original saves will be backed up in `acst_backup` folder.
6. Copy converted files (*.save) to save location, you may need to temporarily disable cloud save sync before starting the game.

Note: Detection features only support certain saves.

Supported game saves and their decryption/encryption ID type:
```
Assassin's Creed Odyssey           // Account GUID
Assassin's Creed Origins           // Account GUID
Steep                              // Account GUID
Assassin's Creed Syndicate         // Account GUID
Assassin's Creed Rogue             // Game key
Assassin's Creed Unity             // Account GUID
Assassin's Creed Liberation HD     // Game key
Assassin's Creed IV Black Flag     // Game key
Assassin's Creed III [Remastered]  // Game key [Account GUID]
Assassin's Creed Revelations       // Legacy username in lower case
```

#### Requirements:
Windows 7 and later, x64 edition.

#### Disclaimer:
This software is provided "AS IS" and for research purpose only. Commercial use prohibited.
Author is not responsible for any data corruption may be caused by using this software.

#### Bug report:
Please open issues [here](https://github.com/linzhouyu/ACST/issues).

#### Credits:
- [Ubisoft](https://www.ubisoft.com/) for all the fun.
- [Linus L.](https://github.com/linzhouyu) for writing this tool.
- machine4578 for earlier version testing and feedback.
