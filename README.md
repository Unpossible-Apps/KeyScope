# KeyScope

**Windows License & System Insights.** KeyScope shows the Windows product key stored on your PC, where it came from, and the licensing and system details that go with it. It only reads and never changes anything.

- Finds the OEM key stored in the PC's firmware (the ACPI MSDM table) and the key stored in the registry.
- Shows the Windows edition, version and build, and the licensing channel (Retail, OEM or Volume).
- Keeps the key masked until you reveal it. Copies leave it out of clipboard history and cloud clipboard sync.
- Saves a report as text, CSV or JSON, one file per PC. The full key is only included if you say so.
- Works offline. KeyScope sends nothing about your PC anywhere ([privacy](PRIVACY.md)).

This repository holds KeyScope's downloads, license terms and privacy policy. The source code is not public.

## Download

Get the latest version from the [Releases page](../../releases/latest).

| Edition | For | Download |
| --- | --- | --- |
| **KeyScope** | Windows 10 version 1809 or later, and Windows 11 (x64 and ARM64) | `KeyScope-<version>-setup-<arch>.exe` (installer), or `KeyScope-<version>-portable-<arch>.zip` |
| **KeyScope Classic** | Windows 7 SP1, 8.1, 10 and 11 (needs .NET Framework 4.8) | `KeyScopeClassic-<version>.exe`, a single program file, or `KeyScopeClassic-<version>-portable.zip` |

Both editions show the same information. KeyScope Classic exists for older Windows versions. It has been tested on Windows 11 only, not yet on Windows 7 or 8.1.

### With winget

```powershell
winget install UnpossibleApps.KeyScope
```

This installs KeyScope for the current user. Add `--scope machine` to install it for all users. `winget upgrade UnpossibleApps.KeyScope` updates it. New versions usually reach winget a few days after they appear on the Releases page.

### Portable use

The portable zips run without installation, for example from a USB stick. Preferences and the Technician License are kept in a `Data` folder next to the program. Deleting the `KeyScope.portable` file makes a copy behave like an installed one.

### Checking a download

The files are not code-signed yet, so Windows SmartScreen may warn the first time you run one. Each release includes `SHA256SUMS.txt`. To check a file, compare its hash with the one listed there:

```powershell
Get-FileHash .\KeyScope-1.0.0-setup-x64.exe
```

## License

KeyScope is **free for personal, non-commercial use**. Using it in the course of paid work, such as PC repair, IT support or business administration, requires a **Technician License**: a one-time purchase that can be activated on up to three copies of KeyScope and does not expire. The license unlocks no extra features; the free version is complete.

[Buy a Technician License](https://buy.polar.sh/polar_cl_J5zj0IcIkBdpN3H8Kp7cZXU26mGMN1ogXb2VG4Kj7WB) · [License terms](EULA.md)

## Support

Report problems on the [Issues page](../../issues). Please never post your product key. If you attach a report, save it without the full key.
