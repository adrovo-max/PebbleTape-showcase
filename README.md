# PebbleTape by HandyPebble

**A mirror for your digital day.**

See where your computer day actually went. PebbleTape records foreground
application time on your Windows PC, keeps an encrypted local history, and lets
you review your day without productivity scores or judgments.

**Everything stays on your PC. No account. No cloud. No tracking server.**

- [Official product page and setup guide](https://handypebble.com/pebbletape/)
- [Download PebbleTape 0.2.0 for Windows x64](https://handypebble.com/pebbletape/downloads/PebbleTape-0.2.0-Setup-x64-win10-compat.exe)
- [Developer's note: memory, awareness, better choices](https://handypebble.com/pebbletape/developer/)
- [HandyPebble](https://handypebble.com/)

![PebbleTape settings shown with isolated test data](screenshots/recording-settings.png)

## What you can do

- Record application intervals and review previous days.
- Search and filter entries, see application totals, and save encrypted notes.
- Set a password once. By default, recording starts when you open PebbleTape;
  viewing history still requires your password.
- Require a password before recording starts instead, if you prefer.
- Lock the timeline or hide to the tray while recording continues.
- Pause recording or choose private time without saving application details.
- Follow the Windows display language automatically or choose a language in
  Settings. Navigation supports 12 languages. New recording and security text
  currently supports English and Simplified Chinese, with English fallback for
  other languages.

Window titles are off by default. This version does not capture screenshots,
keystroke contents, or clipboard contents. Recording and history work offline.
Export, automatic history cleanup, and automatic launch at Windows sign-in are
not included yet. Application time describes the foreground window, not effort
or accomplishment.

## Install or update

For Windows 10 or Windows 11, x64. The approximately 52 MB installer includes
the runtime and database components; no separate .NET or database-server setup
is needed. Exit PebbleTape from its tray menu before updating. The installer
preserves your local data outside the program folder.

The current compatibility installer has been confirmed to start on a Windows
10 21H2 x64 PC where the original package would not open. It leaves
hardware-enforced stack protection off for the PebbleTape process, without
changing Windows security settings, database encryption, or password protection.
That does not establish compatibility with every Windows installation.

The installer is unsigned. Windows or workplace policy may warn about or block
it. Do not disable Windows security; ask your administrator before installing
on a work or school PC. First setup requires recording consent and a password
of at least 12 characters. There is no password-recovery service.

SHA-256 for `PebbleTape-0.2.0-Setup-x64-win10-compat.exe`:

```text
5F36CA05D0D99B14420BF683DC0ED39650F4A551699E37584C42ADF53E2CEC27
```

## Privacy boundaries

Activity and notes are encrypted locally. Automatic recording additionally
uses a Windows-protected recording key for your Windows account. Software
running as the same Windows user may recover that key. App password protection
is not a defense against malware, administrators, or someone controlling an
unlocked Windows account. Use separate Windows accounts on shared PCs and lock
Windows when stepping away. This is not an independently audited security
product.

## About this repository

This is the official **public product showcase**, not a source-code repository.
It contains only product information, release notes, and a screenshot made with
isolated test data. Installers are hosted on HandyPebble, not in this repository.

**Source code is not publicly available. Proprietary software. All rights reserved.**

See [release notes](CHANGELOG.md), [security reporting](SECURITY.md), and the
[rights notice](LICENSE-NOTICE.md).
