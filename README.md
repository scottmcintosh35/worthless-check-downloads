# Worthless Check — Windows downloads

Download the **1.0.0-rc66 Windows installer** from the [rc66 release](https://github.com/scottmcintosh35/worthless-check-downloads/releases/tag/v1.0.0-rc66).

## Requirements

Windows 11 x64 or Windows Server 2022 x64 with Desktop Experience. The installer is unsigned. rc66 is a release candidate.

## Getting started

1. Open the release above and download **Worthless-Check-Setup-rc66.exe** under **Assets**.
2. Run the installer and open **Worthless Check**.
3. Create your first Administrator account. Leave fictional sample cases unchecked to start with no cases or payments.
4. Open **Office Information** to enter your organization name, custom heading lines, address, and contact details.

Normal startup creates or reopens your personal workspace at `%LOCALAPPDATA%\WorthlessCheck\Data\wc.sqlite`. It does not require server-group membership. Each Windows user has a separate personal workspace. Reinstalling does not clear an existing workspace.

## Verify the download

The release includes `Worthless-Check-rc66-SHA256.txt`. Expected installer SHA256:

```text
C955FE2F3514D2208904FA65282ED87A209A9A25EC23B38A784C748C44E6F6D4
```

Check it with PowerShell from the folder containing the downloaded installer:

```powershell
Get-FileHash -LiteralPath '.\Worthless-Check-Setup-rc66.exe' -Algorithm SHA256
```

## Scope

This repository contains download instructions and installer releases. It contains no office databases or credentials. GitHub's automatically generated source archives contain this downloads repository's README, not the application source.

Custom organization headings are supported. Archived agency-specific legal forms remain disabled pending review of organization-specific templates. Back up your workspace before updates. Downloading this release does not deploy it to an operational server or change existing office records.
