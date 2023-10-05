# Frequently Asked Questions

## Failed to load save file

This tool only supports standard format saves generated from legit game copies.

For other saves those can't be loaded, either use other alternative tools, or manually hex editing the saves by restoring the save header: the first 0x228 bytes as we can see by looking at a standard format save.

If you still need help, please refer to [this issue](https://github.com/linuslin0/ACST/issues/96)

## 7z SFX error during launch

Extract the packed executable using 7-Zip or other extractor and run the main executable  inside. The packed executable could also be flagged by some antivirus software as false-positive.

## Converted saves not show up/show as corrupted in the game

Please make sure the original saves are not corrupted. This tool does not modify the actual save data.

If you are not using the auto detection feature, ensure that the Encryption/Decryption ID is correct. This tool has basic format checking and decryption validation enabled by default, to help prevent wrong IDs from being used.

Also, for certain games, you won't be able to load a save generated from a higher version of the game.

## How does the save "encryption" work?

AC game saves only do a XOR in ECB mode:
1. Calculate the MD5 hash of your account ID.
2. Generate the encryption key using the 16-byte MD5 hash: take the first and last bytes and followed by the rest 14 bytes in reverse order.
3. Get the rotation offset based on the save data size: `size % 16` and do a right rotation on the key.
4. XOR the key with the save data.

Other games might use different encryption for their save data and are not supported by this tool.
