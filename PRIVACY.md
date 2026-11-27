# KeyScope privacy policy

*Last updated: 2026-11-26*

KeyScope reads Windows licensing and system information **on your PC** and shows it to you. It does not send your product key, information about your PC, or usage data anywhere. It has no telemetry, no analytics, no advertising and no automatic update check.

## What KeyScope reads

- The Windows product key stored in the PC's firmware (the ACPI MSDM table) and in the registry.
- The Windows edition, version, build and licensing channel, and basic system details such as the computer name.

KeyScope only reads this information. It never changes the registry, firmware or Windows activation.

## What stays on your PC

- **Preferences** (theme, language, whether the key is shown) are stored in `%LOCALAPPDATA%\KeyScope`, or in the `Data` folder next to the program when it runs in portable mode. They never include the product key.
- **Reports** are only written when you choose *Save report*, to the file you pick. The full product key is only included if you answer *Yes* when asked; otherwise a report shows only its last five characters.
- **Copying** the key places it on the clipboard but keeps it out of Windows clipboard history and cloud clipboard sync.

## The one time KeyScope uses the internet

KeyScope connects to the internet only when you **activate, check or deactivate an optional Technician License**. While a license is active, KeyScope also checks it again now and then, no more than once every 14 days. These requests go to Polar (`api.polar.sh`), which sells the Technician License, and contain only:

- the license key you entered,
- KeyScope's seller ID, and
- a random installation label (or the activation ID Polar returned for it).

They contain no product key, computer name, user name or other information about your PC. Polar, like any web server, sees the IP address the request comes from. If you never enter a license key, KeyScope never connects to the internet.

The license is stored on your PC: encrypted with Windows' data protection for installed copies, or as a plain file in the `Data` folder for portable copies so that it moves with them.

## Buying a Technician License

Purchases are handled by [Polar](https://polar.sh), the merchant of record, which processes your payment and billing details under its own privacy policy, published on its website. Unpossible Apps receives the order details Polar shares with sellers, such as your name, email address and license key. Card details stay with Polar and its payment processor.

## Downloads

KeyScope's downloads are hosted on GitHub, and the winget listing points to them. GitHub's [privacy statement](https://docs.github.com/site-policy/privacy-policies/github-general-privacy-statement) applies to those downloads.

## Changes and contact

Changes to this policy are published in this repository. Questions can be asked on the [Issues page](../../issues).
