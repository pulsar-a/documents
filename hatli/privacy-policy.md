---
permalink: /hatli/privacy/
---

# Hatli: Privacy Policy

**Last updated: November 18, 2026**

Hatli is an email app for Windows, macOS and Linux made by Dinar Garipov ("I", "me"). This policy explains what
happens to your information when you use Hatli.

> **The short version: I don't collect any data from Hatli.**
>
> - **Your mail goes between your computer and your mail providers only.** Hatli connects straight to the mail
>   servers of the accounts you add (Gmail, Outlook, iCloud, your own…). There is no Hatli server in between and no
>   Hatli account.
> - **Your mail is kept on your computer, encrypted**, and your passwords and sign-ins in your system's keychain.
> - **Nothing about you or your mail is sent to me.** Hatli has no analytics, no ads, no crash reporting of its own and
>   no tracking. I never see your mail, your contacts or your passwords, and I have no way to.
> - **Pictures from the web in messages are blocked** until you choose to load them, so senders can't tell when you
>   open their mail.
> - **If you connect an AI agent to Hatli**, that agent can read your mail through Hatli, as far as you allow. What the
>   agent does with it is between you and the agent's provider.

## Your mail and your mail providers

When you add an account, Hatli connects to that account's mail servers: IMAP to read your mail, SMTP to send it. Your
mail, your folders and the messages you send go between your computer and your provider, encrypted (TLS), under your
provider's own privacy policy. Hatli never falls back to an unencrypted connection, and sends your password only once
the connection is encrypted. It doesn't copy, upload or index your mail anywhere else.

### Signing in with Google or Microsoft

For a Google or Microsoft account, you can sign in with your provider instead of a password. Hatli opens your
provider's own sign-in page in your web browser; you sign in there, never in Hatli. Your provider then gives Hatli a
sign-in token for your mail, which Hatli keeps in your system's keychain and uses only to connect to that account's
mail servers. Your address is taken from the sign-in only when your provider says it is verified.

With a Google account, Hatli asks for access to your Gmail (the `https://mail.google.com/` scope, which IMAP and SMTP
need) and your email address. It uses them only to show you your mail, keep it in step with Gmail, and send the mail
you write, all on your computer. Hatli's use and transfer to any other app of information received from Google APIs
will adhere to the
[Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy), including
the Limited Use requirements. In particular, none of it reaches me, it is never sold, never used for advertising, and
never read by people. It reaches another app only if you connect an AI agent to Hatli yourself (see *AI agents*).

You can end Hatli's access at any time by removing the account in Hatli, and also in your provider's account settings
(for Google, [myaccount.google.com/permissions](https://myaccount.google.com/permissions)).

## What Hatli keeps on your computer

| System | Folders |
|---|---|
| Windows | `%LOCALAPPDATA%\Hatli` (in the Microsoft Store edition, Windows keeps it inside the app's own package folder) and `%USERPROFILE%\.hatli` |
| macOS | `~/Library/Application Support/Hatli` (in the Mac App Store edition, inside the app's container, `~/Library/Containers/app.hatli.mail`) |
| Linux | `~/.config/hatli` (or `$XDG_CONFIG_HOME/hatli`) |

Settings ▸ Storage shows how much space each part takes and opens the folder.

- **Your mail.** A copy of each account's mail is kept on your computer, so Hatli opens fast, searches quickly and
  works offline. Settings ▸ Storage chooses how much mail, and whether attachments, are kept. **Each account's mail is
  encrypted** (ChaCha20-Poly1305), with its own random key kept in your system's keychain. You can turn encryption
  off for an account in its settings; Hatli says plainly what that means.
- **Drafts**, including the drafts AI agents write for you (on Windows, the mail and drafts are in
  `%USERPROFILE%\.hatli`, where Hatli and its agent server both reach them).
- **Your accounts and account groups**: their names, addresses, servers, colors, icons and signatures. A picture you
  choose for an account or a group is saved as Hatli's own small copy, without anything else the file held.
- **Settings**: your appearance, accessibility, mail, privacy and AI agent choices, the senders whose pictures you
  allowed, and the window's layout. Your two custom themes are files of their own.
- **Logs**, only when something goes wrong: warnings and errors with their technical details, which can include the
  names of Hatli's own files. Hatli doesn't write your mail's text, subjects, addresses or passwords into them. Logs
  are deleted after 14 days.
- **The web engine's folder** (`engine`), used by the system's web engine that shows HTML mail. It runs in private
  mode and keeps no mail there.

**Passwords and sign-in tokens are never in these files.** They are kept in your system's own keychain: Windows
Credential Manager, or the macOS Keychain (on this Mac only, never synced to iCloud). On Linux, until Hatli supports
the Secret Service, your password is kept only in memory while Hatli runs, and an encrypted account's mail isn't kept
on disk at all.

None of this leaves your computer. **Removing an account** removes its mail, its key and its password from your
computer (the mail stays on your provider's servers). Uninstalling Hatli doesn't always remove its folders: to remove
everything, also delete them.

Contacts and calendars: Hatli doesn't read your address books or calendars from your providers yet. Contacts and
events you write in Hatli are kept on your computer. When Hatli syncs them, it will be with your own providers only,
and this policy will say so first.

## When Hatli connects to the internet

Besides your mail providers and their sign-in, Hatli goes online only for the things below, and only when you choose
to. Links you click open in your browser or a new message (see *Links*).

### Pictures from the web

Many messages load pictures from websites, and senders use them, especially tiny hidden "tracking pictures", to see
when and where you opened a message. By default (Settings ▸ Privacy ▸ *Pictures from the web*: *Ask*), **Hatli blocks
them**: it shows the message without them, says how many were blocked and whose tracking pictures they are, and loads
them only when you choose, for one message or always for a sender you trust. Tracking pictures have their own setting
there too.

Messages in HTML are shown by your system's own web engine (WebView2 on Windows, WebKit on macOS and Linux), which
Hatli keeps off the network: it can't fetch anything by itself, and scripts, forms and embedded objects in a message
are removed before it is shown. When you load a message's pictures, Hatli fetches them itself, only over an encrypted
connection, without cookies or the page they are in, and never from your own computer or local network. The websites
hosting them learn your IP address, the time and that the message was opened. What they do with that is up to them; I
receive nothing.

### Update checks

The editions downloaded from Hatli's website can check for updates: when you click *Check for updates…*, or, if you
turn it on in Settings ▸ General (**off by default**), each time Hatli starts. Hatli asks GitHub, where its releases
are published (`api.github.com`), for the latest release. Like any connection to a website, this reveals your IP
address to GitHub, and the request names Hatli and its version. It contains nothing about you or your mail, and I
receive nothing from it.

The Microsoft Store and Mac App Store editions are updated by their store.

## AI agents

Hatli can work with AI agents such as Claude, Codex and Cursor through the Model Context Protocol (MCP). Nothing
happens until **you add Hatli to an agent** yourself: Settings ▸ AI agents shows what to paste into your agent's
settings. Hatli doesn't change any agent's settings itself.

**What the agent can do.** Once connected, the agent starts Hatli's MCP server on your computer and talks to it
directly, not over the internet. The server reads the mail kept on your computer (never changing it) and lets the agent
list your accounts and folders, search your mail, read messages and conversations, and write drafts. Settings ▸ AI
agents lets you choose what it may do: *Allow reading message text* (when off, an agent sees only the sender, date and
subject), *Allow writing drafts*, or nothing at all (*Let AI agents use Hatli*). Your choices apply at once.

**What an agent can't do.** It can't send, delete or move mail, or reach the internet through Hatli. A draft it writes
waits in your Drafts, marked as written by an agent, until you review and send it yourself, and it never carries an
attachment.

**Where your mail goes from there.** Whatever an agent reads through Hatli becomes part of its conversation. Most
agents send their conversations to their provider's servers (for example Anthropic or OpenAI) to work, under that
provider's terms and privacy policy. Hatli doesn't control that and I receive none of it. Connect only agents you trust
with your mail.

## No analytics, no ads, no tracking

Hatli contains no analytics, no advertising, no crash reporting of its own, no telemetry, no usage statistics and no
tracking of any kind. Smart categories and search work on your computer. Hatli connects to the internet only as
described above.

Because nothing is collected, there is nothing to sell, share, transfer, request access to or delete on my side.

## App stores and installers

If you get Hatli from the Microsoft Store or the Mac App Store, the store handles its download and updates under its
own privacy policy. If you have chosen in your system's settings to share diagnostics with app developers, the store
may give me crash reports and overall statistics (such as the number of downloads and crashes). These don't tell me
who you are, and Hatli itself sends nothing.

## Links

Links in a message open when you click them, never by themselves, and Hatli shows where a link really goes before you
open it: `https:` links in your browser, `mailto:` links as a new message in Hatli; an `http:` link asks you first.
What happens on those websites is up to them.

## Children

Hatli doesn't collect information from anyone, including children.

## Your rights

Data protection laws such as the GDPR give you rights over personal data that is processed about you. Since I process
no personal data from Hatli, I hold nothing about you to access, correct, export or erase. Your mail is with your mail
providers and on your computer, under your control, and you can view, change or delete it at any time. Your mail
providers handle your mail under their own policies. If you check for updates, GitHub handles those requests under the
[GitHub General Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement).
If you load pictures from the web, the websites hosting them handle those requests under their own policies. If you
connect an AI agent, its provider handles what the agent sends under its own policy.

If you write to me (for example for support), I receive your email address and what you write, use them only to
answer you, and delete them when they are no longer needed. You can ask me to delete them at any time.

## Changes

If Hatli ever starts collecting personal data (for example optional crash reports), this policy will be updated before
that version is released, and the date at the top will change.

## Contact

Questions about privacy: [garipov.dinar@gmail.com](mailto:garipov.dinar@gmail.com)
