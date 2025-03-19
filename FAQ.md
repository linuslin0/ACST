# Frequently Asked Questions

## Failed to load save file

This tool only supports standard format saves generated from legitimate game copies.

If you enconter this error during the save conversion, consider using alternative tools or manually hex editing the saves by restoring the correct save header - usually the first 0x228 bytes as observed in a standard format save.

If you still need help, please refer to [this issue](https://github.com/linuslin0/ACST/issues/96)

## 7z SFX error during launch

The packed executable might be flagged by some antivirus software as a false positive.
Try these steps to run the actual executable instead:
1. Rename the packed executable file extension from `.exe` to `.7z`.
2. Extract it using 7-Zip or another extraction tool.
3. Run the main executable inside the extracted `ACST` folder.

## How to use this tool from the command line?

First, extract the actual executable by following the steps mentioned above 👆.

Then, launch the main executable from a terminal window using the `--no-gui` along with other necessary parameters.

Example:
``` powershell
.\ACSaveTool.exe --no-gui -d="foo" -e="bar" <path_to_save>
```

To check all available parameters, use the `-h` option.

Tip: You can find the game title index on the GUI by selecting a game and hovering the cursor over the game title.

## Where is the Preferences dialog?

`CTRL + P`

## Converted saves not working?

Ensure that the original saves are not corrupted, as this tool does not alter the actual save data.

If you are not using the auto-detection feature, verify that the Encryption/Decryption ID is correct. This tool has basic format checking and decryption validation enabled by default to help prevent incorrect IDs from being used.

Additionally, for certain games, you may not be able to load a save generated from a higher version of the game.

## How does the save "encryption" work?

AC game save only performs an XOR in ECB mode:

1. Compute the MD5 hash of your account ID.
2. Create the encryption key from the 16-byte MD5 hash: take the first and last bytes, followed by the remaining 14 bytes in reverse order.
3. Determine the rotation offset based on the save data size: `size % 16`, then perform a right rotation on the key.
4. XOR the key with the save data.

Note: Other games may use different encryption methods for their saves, which are not supported by this tool.
