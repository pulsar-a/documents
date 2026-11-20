---
permalink: /brinebook/privacy/
---

# Brinebook: Privacy Policy

**Last updated: November 20, 2026**

Brinebook is a journal for your ferments, for Windows, macOS and Linux, made by Dinar Garipov ("I", "me"). This policy
explains what happens to your information when you use Brinebook.

> **The short version: I don't collect any data from Brinebook.**
>
> - **Your journal stays on your computer.** Your ferments, jars, recipes, pantry, readings and photos are kept in one
>   folder on your computer, and Brinebook's settings and logs too.
> - **Nothing about you or your journal is sent to me.** Brinebook has no account, no analytics, no ads, no crash
>   reporting and no tracking.
> - **Brinebook goes online for one thing only:** to check for a new version, in the editions you download from GitHub.
>   You can turn that off.
> - **Photos from your phone** travel over your own home network, straight to your computer, only while you have it
>   switched on. Nothing goes through the internet.

## Your journal stays on your computer

Everything you write in Brinebook (your ferments and batches, your jars, recipes and pantry, the journal's notes, pH
and temperature readings, ratings and photos) is kept as plain files in one folder on your computer. Brinebook never
copies or uploads it anywhere. Settings ▸ Your journal shows where it is (*Show in folder*).

When you add a photo, Brinebook keeps its own copy in the journal. It turns it upright and leaves out what the camera
wrote into it, such as the place it was taken (EXIF, XMP and IPTC data), so your journal doesn't hold your location.

If you put your journal in a cloud folder such as iCloud Drive, Dropbox or OneDrive, or copy it to another computer,
that service or copy works under its own terms. That is your own choice: Brinebook only reads and writes the files on
your computer, and I receive nothing from it.

## What Brinebook keeps on your computer

| Edition | Folder |
|---|---|
| Windows | `%LOCALAPPDATA%\Brinebook` (in the Microsoft Store edition, Windows keeps it inside the app's own package folder) |
| macOS | `~/Library/Application Support/Brinebook` (in the Mac App Store edition, inside the app's container, `~/Library/Containers/app.brinebook.journal`) |
| Linux | `~/.config/brinebook` (or `$XDG_CONFIG_HOME/brinebook`) |

In that folder:

- **Your journal** (`journal`), with two safety nets: a copy of each file as it was before its first change of the
  day (`backups`), and what you delete (`trash`), so Undo can bring it back. Both are kept for 30 days, then deleted.
  A file Brinebook can't read is moved aside to `unreadable` and kept, untouched.
- **Settings**: your language, units and temperature scale, theme, font, accent color, background and the other look
  choices, text size and motion, the questions you asked not to be asked again, how codes on jars are made, the salt
  you used last, and whether to check for updates. If you choose your own picture as the background, a copy of it is
  kept beside the settings.
- **Logs**, written only when something goes wrong: warnings and errors with their technical details. They never
  contain what you wrote in your journal; a file error is logged by its kind and code, not by your file's name. Logs
  are deleted after 14 days.
- **Small copies of your photos** (`thumbnails`), so lists show quickly. They can be deleted at any time; Brinebook
  makes them again.
- **Updates** you download in the editions that update themselves, in an `updates` folder until they are installed.
- **Unsaved changes**, only in the rare case that your journal's folder couldn't be written to when you closed
  Brinebook and you chose to close anyway (`unsaved`); Brinebook tells you where they are.

None of this leaves your computer. Uninstalling Brinebook doesn't remove this folder, so your journal is never lost by
accident: to remove everything, delete the folder yourself.

## Photos from your phone

Brinebook can take photos straight from your phone (the **Phone** button, or Ctrl+P). This is **off until you press
*Connect your phone***, and works like this:

- Brinebook starts a small web server on your computer, on your home network only, and shows a QR code. The address in
  it carries a long random code (a token of 128 random bits): Brinebook answers only requests that carry it.
- Your phone opens that address in its browser. No app, no account, and no internet: your phone and your computer talk
  to each other directly over your Wi-Fi.
- The page on your phone shows the names (and small pictures) of your ferments, jar types, jars and recipes, so you can
  choose where each photo goes. Your phone sends the photos you choose to your computer, where they go into your journal.
- The session ends when you press *Stop*, when you quit Brinebook, or after half an hour without use. A new session has
  a new code.

The connection uses plain HTTP inside your home network, not encryption. Someone else on the same network who could
read its traffic could see the photos you send and the names on that page while a session is on, and anyone who had
the address could use it until the session ends. Use it on a network you trust, such as your home Wi-Fi, and press
*Stop* when you're done. Nothing of this ever reaches me.

## When Brinebook connects to the internet

### Update checks

The editions you download from Brinebook's releases on GitHub check for a new version:

- **When Brinebook starts**, while *Check for updates when Brinebook starts* is on in Settings ▸ Updates. It is **on by
  default**; turn it off there and Brinebook won't go online by itself.
- **When you press *Check now*** in Settings ▸ Updates.

To check, Brinebook asks GitHub, where its releases are published, what the latest version is. If there is a newer one
and you choose to update, Brinebook downloads it from GitHub, checks that it is exactly the published file, and
installs it when you quit. Like any connection to a website, this reveals your IP address to GitHub, and the request
names Brinebook and its version (GitHub requires that). It contains nothing about you or your journal, and I receive
nothing from it.

The Microsoft Store and Mac App Store editions don't check: their store updates them.

Brinebook makes no other connection to the internet.

## No analytics, no ads, no tracking

Brinebook contains no analytics, no advertising, no crash reporting, no telemetry, no usage statistics and no tracking
of any kind.

Because nothing is collected, there is nothing to sell, share, transfer, request access to or delete on my side.

## App stores and installers

If you get Brinebook from the Microsoft Store or the Mac App Store, the store handles its download and updates under
its own privacy policy. If you have chosen in your system's settings to share diagnostics with app developers, the
store may give me crash reports and overall statistics (such as the number of downloads and crashes). These don't tell
me who you are, and Brinebook itself sends nothing.

## Children

Brinebook doesn't collect information from anyone, including children.

## Your rights

Data protection laws such as the GDPR give you rights over personal data that is processed about you. Since I process
no personal data from Brinebook, I hold nothing about you to access, correct, export or erase. Your journal and
Brinebook's settings and logs are on your computer, under your control, and you can view, change, copy or delete them
at any time. If you check for updates, GitHub handles those requests under the
[GitHub General Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement).

If you write to me (for example for support), I receive your email address and what you write, use them only to
answer you, and delete them when they are no longer needed. You can ask me to delete them at any time.

## Changes

If Brinebook ever starts collecting personal data (for example optional crash reports, or syncing), this policy will be
updated before that version is released, and the date at the top will change.

## Contact

Questions about privacy: [garipov.dinar@gmail.com](mailto:garipov.dinar@gmail.com)
