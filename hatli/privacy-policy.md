---
permalink: /hatli/privacy/
---

# Hatli: Privacy Policy

**Last updated: November 25, 2026**

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
>   open their mail. Fonts from the web stay off unless you turn them on.
> - **If you connect an AI agent to Hatli**, that agent can read your mail through Hatli, as far as you allow. What the
>   agent does with it is between you and the agent's provider.

## Your mail and your mail providers

When you add an account, Hatli connects to that account's mail servers: IMAP to read your mail, SMTP to send it. Your
mail, your folders, the messages you send and the drafts you write (kept in your account's Drafts folder, so they are
there on your other devices; not the drafts AI agents write) go between your computer and your provider, encrypted
(TLS), under your provider's own privacy policy. Hatli never falls back to an unencrypted connection, and sends your password only once
the connection is encrypted. It doesn't copy, upload or index your mail anywhere else.

### Signing in with Google or Microsoft

For a Google or Microsoft account, you can sign in with your provider instead of a password. Hatli opens your
provider's own sign-in page in your web browser; you sign in there, never in Hatli. Your provider then gives Hatli a
sign-in token for your mail, which Hatli keeps in your system's keychain and uses only to connect to that account's
mail servers. Your address is taken from the sign-in: from Google, only when Google says it is verified; from
Microsoft, as the name of the Microsoft account you signed in with.

With a Google account, Hatli asks for access to your Gmail (the `https://mail.google.com/` scope, which IMAP and SMTP
need) and your email address. It uses them only to show you your mail, keep it in step with Gmail, and send the mail
you write, all on your computer. Hatli's use and transfer to any other app of information received from Google APIs
will adhere to the
[Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy), including
the Limited Use requirements. In particular, none of it reaches me, it is never sold, never used for advertising, and
never read by people. It reaches another app only if you connect an AI agent to Hatli yourself (see *AI agents*).

With a Microsoft account (Outlook.com, Hotmail, Live, Microsoft 365), Hatli asks for access to your mail over IMAP
and SMTP (`IMAP.AccessAsUser.All`, `SMTP.Send`), to stay signed in, and for your email address, and uses them only in
the same way. If you turn on *Sync contacts* or *Sync calendar* for it, Hatli also asks to read your contacts
(`Contacts.Read`) or your calendars (`Calendars.Read`) through Microsoft Graph, and only reads them, unless you also
turn on *Edit calendar*: then it asks to change your calendars too (`Calendars.ReadWrite`), and uses that only to send
the events you add, change or delete in Hatli.

You can end Hatli's access at any time by removing the account in Hatli, and also in your provider's account settings
(for Google, [myaccount.google.com/permissions](https://myaccount.google.com/permissions); for a personal
Microsoft account, [account.live.com/consent/Manage](https://account.live.com/consent/Manage); for a work or school
account, [myapplications.microsoft.com](https://myapplications.microsoft.com/)).

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
  `%USERPROFILE%\.hatli`, where Hatli and its agent server both reach them). **Each draft is encrypted**
  (AES-GCM), with a random key kept in your system's keychain.
- **Your accounts and account groups**: their names, addresses, servers, colors, icons and signatures. A picture you
  choose for an account or a group, or for a signature (a company's logo, `signatures`), is saved as Hatli's own small
  copy, without anything else the file held. A signature's pictures go inside the messages it is under.
- **Settings**: your appearance, accessibility, mail, privacy and AI agent choices, the senders whose pictures you
  allowed, and the window's layout. Your two custom themes are files of their own.
- **Company logos**, if you turn them on (see *Company logos*): the icons of the websites Hatli asked, as Hatli's
  own small copies (`logos`), each kept for 30 days.
- **Logs**, only when something goes wrong: warnings and errors with their technical details, which can include the
  names of Hatli's own files. Hatli doesn't write your mail's text, subjects, addresses or passwords into them. Logs
  are deleted after 14 days.
- **Notifications.** When new mail comes to an inbox while Hatli is open, Hatli asks your system to show a
  notification with the sender and the subject (Settings ▸ Notifications can make it say only that new mail came,
  turn notifications off, or mute them every day between two times; a muted group stays quiet). Your system keeps its notifications in its own
  notification center and may show them on the lock screen. On Windows, outside the Microsoft Store edition, the
  name they are shown under is written in your user's registry (`Software\Classes\AppUserModelId\Hatli.Mail`).
  Nothing about them is sent over the internet.
- **Your default email app**, only if you choose it: Settings ▸ General ▸ *Make Default* asks your system to open email
  links in Hatli (on Windows, in Windows' own settings; on macOS, your Mac asks you first). On Windows, a copy of Hatli
  that wasn't installed first lists itself among your email apps, in your user's registry (`Software\Hatli`,
  `Software\Classes\Hatli.Url.mailto`).
- **The web engine's folder** (`engine`), used by the system's web engine that shows HTML mail. It runs in private
  mode and keeps no mail there.

**Passwords and sign-in tokens are never in these files.** They are kept in your system's own keychain: Windows
Credential Manager, or the macOS Keychain (on this Mac only, never synced to iCloud). On Linux, until Hatli supports
the Secret Service, your password is kept only in memory while Hatli runs, and an encrypted account's mail and your
drafts aren't kept on disk at all.

None of this leaves your computer. **Removing an account** removes its mail, its key and its password from your
computer (the mail stays on your provider's servers). Uninstalling Hatli doesn't always remove its folders: to remove
everything, also delete them.

Contacts: if you turn on *Sync contacts* for an account (Add account asks; the account's settings change it), Hatli
copies that account's address book from your own provider into Contacts: from its contacts server (CardDAV) for
iCloud, Fastmail, Yahoo or your own domain, from Google's contacts (the People API) for Gmail, or from Microsoft
Graph for Outlook (read only), for which Google or Microsoft asks you first to let Hatli see your contacts. Hatli only reads them, unless you also turn on *Edit contacts* for the
account (it is off until you do): then a contact you add, change or delete in Hatli in that account's address book is
sent to that same provider, and only that (Google asks you first to let Hatli change your contacts). Hatli deletes a
contact at your provider only when you delete it in Hatli, a few seconds later (so you can undo it), and never writes
over, or deletes, a contact changed there meanwhile. A change waiting to be sent is kept with the copy.
**The copy is encrypted** (ChaCha20-Poly1305) with its own random key in your system's keychain, whatever you chose for the mail;
where there is no keychain (Linux, for now) it is kept only in memory while Hatli runs. Turning the switch off, or
removing the account, removes the copy and its key from your computer.

Calendars: if you turn on *Sync calendar* for an account (Add account asks; the account's settings change it), Hatli
copies that account's calendars from your own provider: from its calendar server (CalDAV) for iCloud, Fastmail, Yahoo
or your own domain, signing in as it does for the mail, from Google Calendar (the Calendar API) for Gmail, for which
Google asks you first to let Hatli see your calendars (the `calendar.readonly` scope, used under the same Limited Use
terms as your mail), or from Microsoft Graph for Outlook, for which Microsoft asks you first. Hatli only reads them, unless you also turn on *Edit calendar* for the account (it is off until you
do): then an event you add, change or delete in Hatli in one of its calendars is sent to that same provider, and only
that change (when you open a guest's answer to an invitation you sent, that guest's answer in the event counts as one) (Google asks you first to let Hatli change your calendar events, the `calendar.events` scope; Microsoft,
the `Calendars.ReadWrite` scope). Hatli never writes over a change made there meanwhile (at Outlook, it looks for one
just before it writes), and never lets your provider send its guests anything, except Outlook, which itself emails an
event's guests its invitation, changes and cancellation when you add, change or delete an event that has guests. A change waiting to
be sent is kept with the copy. Without *Edit calendar*, events you add in Hatli to a synced calendar, and your answers
to invitations, are kept with the copy on your computer and aren't sent to the server (an answer goes to the organizer
as a message, as described above). **The copy is encrypted** the same way, with its own random key; where
there is no keychain it is kept only in memory. Turning the switch off, or removing the account, removes the copy, the
events you added to it and its key from your computer. Events you write in a calendar that isn't synced are kept on
your computer only.

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

### Fonts from the web

Some messages are designed with fonts that live on a website: the sender's, or a font service's (such as Google Fonts).
Fetching one tells that website your IP address, the time and that the message was opened, as a picture does. By
default (Settings ▸ Privacy ▸ *Fonts from the web*: off), **Hatli doesn't fetch them**, and messages show in fonts on
your computer. If you turn it on, Hatli fetches a message's fonts itself, the same way it fetches pictures, and only
for a message whose pictures from the web you loaded. I receive nothing.

### Company logos

If you turn on *Company logos* in Settings ▸ Privacy (**off by default**), Hatli shows a company's logo beside its
mail instead of its initials. For that it first looks up the logo the company publishes for its mail (BIMI) in the
DNS, through the DNS servers your computer uses, and if there is one, fetches it from where the company's record says
it is. Otherwise it asks the company's own website (the end of the sender's address, such as `amazon.de`) for the icon
it publishes for itself: `apple-touch-icon.png`, else the icon its home page names (which can be on a server the
website keeps its files on), or else `favicon.ico`. It asks only over an encrypted connection, without cookies, and
never from your own computer or local network. It never asks about personal addresses at mail services (such as Gmail
or Outlook). The website (and the server it keeps its icon or logo on) learns your IP address and the time, but not
which message you got, or that you opened it. Hatli keeps each icon on your computer for 30 days, and asks a website
that has none again only after 7 days. I receive nothing.

### Update checks

The editions downloaded from Hatli's website can check for updates: when you click *Check for updates…*, or, if you
turn it on in Settings ▸ General (**off by default**), when Hatli starts, at most once a day. Hatli asks GitHub, where its releases
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
If you load pictures from the web, turn on fonts from the web, or turn on company logos, the websites asked handle
those requests under their own policies. If you
connect an AI agent, its provider handles what the agent sends under its own policy.

If you write to me (for example for support), I receive your email address and what you write, use them only to
answer you, and delete them when they are no longer needed. You can ask me to delete them at any time.

## Changes

If Hatli ever starts collecting personal data (for example optional crash reports), this policy will be updated before
that version is released, and the date at the top will change.

## Contact

Questions about privacy: [garipov.dinar@gmail.com](mailto:garipov.dinar@gmail.com)
