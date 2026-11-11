---
permalink: /uku/privacy/
---

# Uku: Privacy Policy

**Last updated: November 11, 2026**

Uku is a Markdown reader for Windows, macOS and Linux made by Dinar Garipov ("I", "me"). This policy explains what
happens to your information when you use Uku.

> **The short version: I don't collect any data from Uku.**
>
> - **Your documents stay on your computer.** Uku reads and edits the Markdown files and folders you open, where they
>   are. Its settings and logs are kept only on your computer too.
> - **Nothing about you or your documents is sent to me.** Uku has no account, no analytics, no ads, no crash
>   reporting of its own and no tracking.
> - **Uku goes online only when you ask it to:** to check for updates, or to load a picture from the web. Both are off
>   until you turn them on or click them.
> - **If you connect an AI agent to Uku** (optional, off until you set it up), that agent can read your Markdown
>   through Uku. What the agent does with it is between you and the agent's provider.

## Your documents stay on your computer

Uku opens the Markdown files and folders you choose, reads them where they are and, when you edit a document, saves it
back to the same file. It doesn't copy or upload your documents anywhere. Diagrams, math, syntax highlighting and
everything else on the page are drawn on your computer.

**Read aloud** uses the voices installed on your computer, through your system's own speech (on Windows, Windows'
speech voices; on a Mac, the Mac's own voices). Uku never sends the text to an online speech service.

Searching your files reads them on your computer when you search. Uku doesn't build or keep a search index on disk.

If your files are in a cloud folder such as iCloud Drive, Dropbox, OneDrive or on a network drive, that service syncs
them under its own privacy policy. That is your own choice and your own service: Uku only reads and writes the files on
your computer, and I receive nothing from it.

## What Uku keeps on your computer

Uku keeps a settings file and, only when something goes wrong, log files in its own folder. Settings ▸ Advanced shows
where they are and opens them.

| Edition | Folder |
|---|---|
| Windows | `%LOCALAPPDATA%\Uku` (in the Microsoft Store edition, Windows keeps it inside the app's own package folder) |
| macOS | `~/Library/Application Support/Uku` (in the Mac App Store edition, inside the app's container, `~/Library/Containers/app.uku.reader`) |
| Linux | `~/.config/uku` (or `$XDG_CONFIG_HOME/uku`) |

- **Settings** hold your appearance, reading, accessibility (such as text spacing, the reading ruler and the read
  aloud voice and speed) and language choices, your keyboard shortcuts, the window's size and
  position, the folders of your workspace and the documents you had open, your pinned files and folder colors, your
  list of recent files and folders (their paths on your computer), and your choices for updates, web pictures and AI
  agents. You can clear the recent list in the app (⋯ ▸ Recent ▸ *Clear list*).
- **Logs** hold warnings and errors with their technical details, which can include the paths of files and folders
  Uku couldn't read, watch or save. Uku writes them only when something goes wrong.
- **Updates** you download in the editions that update themselves are kept in an `updates` folder there until they are
  installed.
- **On a Mac App Store edition**, macOS lets Uku open only the folders you choose. To open them again next time, Uku
  keeps macOS's permission for each (a "bookmark") in its folder.

None of this leaves your computer. Uninstalling Uku doesn't always remove it: to remove everything, also delete its
folder (and, if you connected an AI agent, the sessions folder described below).

When you delete a file or folder in Uku's sidebar, it goes to your system's Trash or Recycle Bin, where you can restore
it. Where there is none (for example on some network drives), Windows asks you before deleting it for good, and on
macOS and Linux Uku doesn't delete it.

## When Uku connects to the internet

Uku goes online only for the two things below, and only when you choose to. Links you click open in your browser or
email app (see *Links*).

### Update checks

The editions downloaded from Uku's website can check for updates, in two cases only:

- **When you click *Check for updates…*** (or *Check now* in Settings ▸ General). Uku checks once, right then.
- **When you turn on *Check for updates when Uku starts*** in Settings ▸ General. It is **off by default**. Uku then
  checks once each time it starts, until you turn it off again.

To check, Uku asks GitHub, where its releases are published, what the latest version is. If there is a newer one and
you choose to update, Uku downloads it from GitHub, checks that it is exactly the published file, and installs it when
Uku quits. Like any connection to a website, this reveals your IP address to GitHub, and the request names Uku and its
version (GitHub requires that). It contains nothing about you or your documents, and I receive nothing from it.

The Microsoft Store and Mac App Store editions are updated by their store. Asking for updates there asks the Microsoft
Store, or opens Uku's page in the App Store.

### Pictures from the web

A document can show pictures from websites. By default (Settings ▸ Reading ▸ *Pictures from the web*: *Always ask*),
Uku doesn't download them: it shows a placeholder, and loads a picture only when you click it, or all of a document's
pictures when you click *Load pictures*. So opening a document never tells a website that you read it, unless you ask.

When a picture is loaded, by your click or because you chose *Allow* in Settings, the website hosting it can see your
IP address, the time, that Uku (and its version) requested it, and so that the document was opened. Uku sends no
cookies with these requests. You can go back to *Always ask* at any time.

## AI agents

Uku can work with AI coding agents such as Claude Code and Codex through the Model Context Protocol (MCP). This is
**optional and off until you set it up**, in Settings ▸ AI agents (or by adding Uku to an agent yourself).

**What setting it up does.** When you click *Add Uku* for an agent, Uku runs that agent's own command to add Uku, or
adds an entry for Uku to that agent's settings file. To show you which agents have Uku, Settings ▸ AI agents reads
those agents' settings files on your computer. *Remove* and *Disconnect* take Uku out again.

**What the agent can do.** Once connected, the agent starts Uku's MCP server on your computer and talks to it
directly, not over the internet. The agent can search your Markdown files, read their outlines and sections, check them
and open them in Uku. Whatever the agent reads this way becomes part of its conversation. Most agents send their
conversations to their provider's servers (for example Anthropic or OpenAI) to work, under that provider's terms and
privacy policy. Uku doesn't control that and I receive none of it. Connect only agents you trust with your documents.

**What you're reading.** An agent can also ask which document you have open in Uku, which section is on screen and
which text you selected, but only if you turn on *Let agents see what I'm reading* in Settings ▸ AI agents. It is
**off by default**.

**Sessions.** To list each agent session with the Markdown files it wrote in the sidebar's Sessions tab, Uku's server
watches the agent's project folder for Markdown files that change, and reads the agent's own session records on your
computer (Claude Code's in `~/.claude`, Codex's in `~/.codex`) to find the session's name and the Markdown files it
wrote. On a Mac App Store edition, it reads Claude Code's folder only after you allow it. From these, Uku keeps only
each session's title, the agent's name, the project folder, and the names of the files with when they changed, in a
`sessions` folder (`%USERPROFILE%\.uku` on Windows, Uku's own folder on macOS and Linux). Nothing else of your
conversations is kept. A session is kept for 30 days after it was last active; *Clear session data…* in Settings ▸ AI
agents deletes them all now.

## No analytics, no ads, no tracking

Uku contains no analytics, no advertising, no crash reporting of its own, no telemetry, no usage statistics and no
tracking of any kind. It connects to the internet only as described above.

Because nothing is collected, there is nothing to sell, share, transfer, request access to or delete on my side.

## App stores and installers

If you get Uku from the Microsoft Store or the Mac App Store, the store handles its download and updates under its own
privacy policy. If you have chosen in your system's settings to share diagnostics with app developers, the store may
give me crash reports and overall statistics (such as the number of downloads and crashes). These don't tell me who you
are, and Uku itself sends nothing. The same goes for installing with Homebrew or winget: those tools work under their
own policies.

## Links

Web and email links in a document open in your browser or email app when you click them; other files open in the app
your system uses for them, or in the app you pick from a link's menu (*Open with*). What happens on those websites and in those apps is up to them.

## Children

Uku doesn't collect information from anyone, including children.

## Your rights

Data protection laws such as the GDPR give you rights over personal data that is processed about you. Since I process
no personal data from Uku, I hold nothing about you to access, correct, export or erase. Your documents and Uku's
settings, logs and sessions are on your computer, under your control, and you can view, change or delete them at any
time. If you check for updates, GitHub handles those requests under the
[GitHub General Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement).
If you load pictures from the web, the websites hosting them handle those requests under their own policies. If you
connect an AI agent, its provider handles what the agent sends under its own policy.

If you write to me (for example for support), I receive your email address and what you write, use them only to
answer you, and delete them when they are no longer needed. You can ask me to delete them at any time.

## Changes

If Uku ever starts collecting personal data (for example optional crash reports), this policy will be updated before
that version is released, and the date at the top will change.

## Contact

Questions about privacy: [garipov.dinar@gmail.com](mailto:garipov.dinar@gmail.com)
