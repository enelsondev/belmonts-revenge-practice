# Applying alpha17

## 1. Check your input ROM

Use an **unmodified US Castlevania II: Belmont's Revenge**, revision0, exactly
**131,072 bytes (128 KiB)**. Filenames alone do not identify a ROM.
Do not use a Japanese ROM, another hack, an older practice ROM, or a patched output.

| Check | Required value |
|---|---|
| SHA-256 | `17570ceec1b22153604622c4412d048dd8f7ccb4626daf9ddea96de8a062dbf2` |
| SHA-1 | `696b9ad1e9cfb7112977c9a7c05cf64fe8423d8a` |
| CRC32 | `8875C8FE` |

On Windows PowerShell, check SHA-256 with:

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath 'C:\Games\YourOriginalGame.gb'
```

The IPS format does not enforce an input-ROM checksum. Verify the hash first;
a patcher completing successfully does not prove you used the correct ROM.
Keep your original ROM unchanged. Obtain/dump your own copy; this project provides none.

## 2. Apply the patch

A browser option is [Rom Patcher JS](https://www.marcrobledo.com/RomPatcher.js/),
whose [upstream project](https://github.com/marcrobledo/RomPatcher.js) supports IPS.

1. Download and extract the alpha17 release ZIP.
2. Open the patcher and select your matching **original US ROM** as the ROM file.
3. Select `patches/belmont-practice-alpha17.ips` as the patch file.
4. Apply the patch and save the result as a **new** file, such as
   `BelmontsRevengePractice-alpha17.gb`.
5. Check the resulting file against the values below.

Apply just this one patch directly to the clean source. Do not stack practice
releases or apply it a second time. No Japanese ROM is needed to use Cross.

## 3. Verify and play

Expected patched size: **262,144 bytes (256 KiB)**.
Expected patched SHA-256:

`fff7bd58fdae8ee270d72d92cb008037b8e2305f4f1d55d19247142275828449`

Cold-boot this output in BGB or your Game Boy emulator. Do not load an older
build's save state. Start pauses; Up+Select opens Practice. See [CONTROLS.md](CONTROLS.md).

## Troubleshooting

- Wrong source hash: use the specified unmodified US revision; renaming a ROM won't fix it.
- Wrong output hash/size: check the source and patch versions, then patch the clean source again.
- Game boots but menu is wrong: cold-boot the patched `.gb`, without an old save state
  or emulator auto-patching another IPS over it.
- Emulator reports unsupported cartridge: the output uses MBC1, 256 KiB ROM, no cartridge RAM.
- Still stuck: report the emulator/core and release version, without uploading your ROM or state.
