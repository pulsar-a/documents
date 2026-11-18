---
permalink: /yasa/privacy/
---

# Yasa: Privacy Policy

**Last updated: November 13, 2026**

Yasa is a to-do app for Windows, macOS and Linux made by Dinar Garipov ("I", "me"). This policy explains what happens
to your information when you use Yasa.

> **The short version: I don't collect any data from Yasa.**
>
> - **Your tasks stay on your computer.** Your lists and tasks are in `.yasa` files you choose. Yasa's settings,
>   backups and logs are kept only on your computer too.
> - **Nothing about you or your tasks is sent to me.** Yasa has no account, no analytics, no ads, no crash reporting of
>   its own and no tracking.
> - **Yasa goes online only when you ask it to:** to check for updates. Checking at every start is off until you turn
>   it on.
> - **If you connect an AI agent to Yasa** (optional, off until you set it up), that agent can read and change the tasks
>   of the documents you allow. What the agent does with them is between you and the agent's provider.

## Your tasks stay on your computer

Your lists and tasks are saved in `.yasa` files on your computer, in the folders you choose. Yasa has no account and no
server, and it does not send your tasks anywhere. There is no copy of your data anywhere except where you put it.

If you keep a file in a cloud folder such as iCloud Drive, Dropbox or OneDrive, that service syncs it under its own
privacy policy. That is your own choice and your own service: Yasa only reads and writes the file on your computer,
and I receive nothing from it.

## What Yasa keeps on your computer

Besides your `.yasa` files, Yasa keeps a folder of its own on your computer: `%LOCALAPPDATA%\Yasa` on Windows,
`~/Library/Application Support/Yasa` on macOS (inside the app's container for the Mac App Store edition) and
`~/.local/share/Yasa` on Linux. In it are:

- **your settings**, including the documents you opened recently;
- **backups** of your documents, the last versions of each, so you can go back to one;
- **copies used to merge changes** made to the same document on two computers, and changes waiting to be written when a
  document couldn't be saved at once;
- **log files**, written only when something goes wrong, with what went wrong. They contain no task titles or notes;
- **AI agents' settings**, when you connect one (see *AI agents*);
- **downloaded updates**, while they wait to be installed (see *Update checks*).

None of it leaves your computer. *About Yasa ▸ Diagnostic info* shows a report for a bug report, with nothing private in
it; it goes nowhere unless you copy it and send it yourself. Uninstalling Yasa and deleting this folder and your `.yasa`
files removes everything.

## When Yasa connects to the internet

Yasa goes online only to check for updates, and only when you choose to. Links you open go to your browser (see
*Links*).

### Update checks

The editions downloaded from Yasa's website can check for updates, in two cases only:

- **When you click *Check for updates…*** (in the menu, Settings ▸ General ▸ *Check now*, or *Update Yasa* for a
  document made by a newer Yasa). Yasa checks once, right then.
- **When you turn on *Check for updates when Yasa starts*** in Settings ▸ General. It is **off by default**. Yasa then
  checks once each time it starts, until you turn it off again.

To check, Yasa asks GitHub, where its releases are published, what the latest version is. If there is a newer one and
you choose to update, Yasa downloads it from GitHub, checks that it is exactly the published file, and installs it when
Yasa quits. Like any connection to a website, this reveals your IP address to GitHub, and the request names Yasa and its
version (GitHub requires that). It contains nothing about you or your tasks, and I receive nothing from it.

The Microsoft Store and Mac App Store editions are updated by their store. Asking for updates there asks the Microsoft
Store, or opens Yasa's page in the App Store.

## Passwords

If you protect a document with a password, Yasa encrypts it on your computer. Your password is never stored or sent
anywhere. If you choose "Remember on this device", a key derived from the password is kept in your operating system's
secure storage (the macOS Keychain, Windows DPAPI or your Linux keyring) and stays on that computer.

I can't see, reset or recover your password. If you forget it, nobody can open that document, including me.

## Purchases (Microsoft Store, Mac App Store)

The store editions offer an optional purchase, Yasa Pro: an in-app purchase in the Mac App Store, an add-on in the
Microsoft Store. Purchases are handled entirely by Apple or Microsoft. I don't receive your name, account, payment
details or any other personal information; Yasa only asks the store whether Pro is owned. The stores' handling of
purchases is described in their privacy policies. They may give developers aggregated, anonymous sales reports; these
contain nothing that identifies you. The editions from Yasa's website have no purchases: everything in them is
unlocked.

## AI agents (optional)

Yasa can act as a local MCP server, so that an AI tool you install and set up yourself can read and change your tasks.
It runs on your computer only when your AI tool starts it, does not listen on the network, and reaches only the
documents you allow agents to use. When you connect an agent in Settings ▸ AI agents, Yasa adds itself to that agent's
settings on your computer. Whatever the agent sends to its AI provider is governed by that tool's and provider's
privacy policies. Yasa itself sends nothing to anyone.

## No analytics, no ads, no tracking

Yasa contains no analytics, no advertising, no crash reporting of its own, no telemetry, no usage statistics and no
tracking of any kind.

Because nothing is collected, there is nothing to sell, share, transfer, request access to or delete on my side.

## App stores and installers

If you get Yasa from the Microsoft Store or the Mac App Store, the store handles its download and updates under its own
privacy policy. If you have chosen in your system's settings to share diagnostics with app developers, the store may
give me crash reports and overall statistics (such as the number of downloads and crashes). These don't tell me who you
are, and Yasa itself sends nothing. Downloading Yasa from GitHub, or installing it with a Linux package manager, works
under those services' own policies; Yasa's installers and packages send nothing.

## Links

Links you put into task descriptions open in your web browser only after you confirm. What happens on those websites
is up to them.

## Children

Yasa doesn't collect information from anyone, including children.

## Your rights

Data protection laws such as the GDPR give you rights over personal data that is processed about you. Since Yasa
processes no personal data on my side, I hold nothing about you to access, correct, export or erase. Your data is on
your computer, under your control, and you can view, change, export or delete it at any time.

## Changes

If Yasa ever starts processing personal data (for example optional crash reports), this policy will be updated before
that version is released, and the date at the top will change.

## Contact

Questions about privacy: [garipov.dinar@gmail.com](mailto:garipov.dinar@gmail.com)
