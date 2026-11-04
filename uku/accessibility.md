---
permalink: /uku/accessibility/
---

# Uku: Accessibility

**Last updated: November 4, 2026**

Uku should work for everyone, whether you read with a mouse, only the keyboard, a screen reader, or need more contrast,
larger text or less motion. This page lists what Uku does for that on Windows, macOS and Linux, and where to find the
settings.

Shortcuts are written for Windows and Linux; on a Mac, use ⌘ for Ctrl and ⌥ for Alt, except where the table says
otherwise. These are the default shortcuts: you can change any of them in Settings ▸ Keyboard.

## See it the way you need

- **Themes.** The **Aa** button in the toolbar, or Settings ▸ Appearance: *System* (the default) follows your system's
  light or dark setting, or choose *Light*, *Sepia* (warm paper for long reading), *Sage*, *Dusk*, *Dark*, *Espresso*,
  *Night* (near black) or *High contrast*. You can also pick an accent color.
- **High contrast.** The *High contrast* theme, also a switch in Settings ▸ Accessibility: black surfaces, white text,
  a yellow accent and a cyan focus ring, with alerts and messages outlined instead of tinted. On *System*, Uku switches
  to it by itself when your system's high contrast is on.
- **Readable colors.** Text has a contrast of at least 4.5:1 with its background, and the keyboard focus ring at least
  3:1, in every theme, including code and its colors; every accent color is checked too. Uku's automated tests check
  this before every release.
- **Bigger text.** Ctrl+= and Ctrl+- make the document's text larger or smaller, from 70 % to 200 % (Ctrl+0 goes back to
  100 %); Ctrl and the mouse wheel, or pinching on a trackpad, do the same. The page reflows, nothing is cut off. Also in
  **Aa** ▸ *Text size* and Settings ▸ Reading. The rest of the window keeps its size.
- **Comfortable reading.** **Aa** ▸ *Font* (sans, serif or mono) and *Line width* (narrow, medium, wide or the full
  window). Focus mode (F11) leaves only the page.

## Not just color

Nothing in a document is told only by color:

- Alerts (*Note*, *Tip*, *Important*, *Warning*, *Caution*) have an icon and their name, not only a tint.
- Links are underlined as well as colored. A link to a file that doesn't exist is shown in red with a dashed
  underline, and clicking it also says *Can't find …*.
- Done tasks are struck through as well as muted, and their box is ticked.
- Find in the document marks the current match with an outline as well as a stronger color, and says *3 of 12*.

## Less motion

Uku has little motion to begin with: a few short fades, and nothing in the interface that moves while you read.
Animated pictures in a document play while they are on screen; large ones have a pause button. Settings ▸
Accessibility ▸ *Motion*: *System* (the default) follows your system: Windows' *Animation effects*, macOS's *Reduce
motion*, GNOME's animations. *Reduced* turns fades and sliding off and stops animated pictures; *Full* keeps them. The
page never animates when a document changes on disk.

## Keyboard

Everything in Uku can be done without a mouse, except moving a file into another folder (see below).

| Action | Shortcut |
|---|---|
| All shortcuts | F1 |
| Move between the toolbar, the sidebar and the page | F6 / Shift+F6 |
| Next / previous link (or button, task box) on the page | Tab / Shift+Tab, then Enter to follow a link |
| Next / previous heading | Alt+↓ / Alt+↑ |
| Scroll the page | Space / Shift+Space, Page Up / Page Down, arrows, Home / End |
| Find in the document | Ctrl+F, then Enter / Shift+Enter (or F3 / Shift+F3; Mac: ⌘G / ⇧⌘G) |
| Search the files | Ctrl+Shift+F |
| Back / forward | Alt+← / Alt+→ (Mac: also ⌘[ / ⌘]) |
| Open a file / a folder | Ctrl+O / Ctrl+Shift+O |
| Reload the document | F5 (Mac: ⌘R) |
| Show or hide the sidebar | Ctrl+Shift+L (Mac: also ⌃⌘S) |
| Edit / read | Ctrl+E |
| Collapse / expand all sections | Ctrl+Shift+C / Ctrl+Shift+E |
| Open a document side by side / go to side 1–4 | Ctrl+\ / Ctrl+1 to Ctrl+4 |
| Text size larger / smaller / 100 % | Ctrl+= / Ctrl+- / Ctrl+0 |
| Settings | Ctrl+, |
| Focus mode | F11 (Mac: also ⌃⌘F) |

In the sidebar, the arrow keys move through files and folders, F2 renames, Delete (Mac: ⌘⌫) deletes and the
context-menu key (or Shift+F10) opens an item's menu. Opening files and folders and reordering the folders of a
workspace and your pinned items (*Move up* / *Move down*) don't need a mouse; moving a file into another folder is still
done by dragging it. Pictures can be reached with Tab and opened larger with Enter (Esc closes them).

Short confirmations such as *Saved* or *Copied* disappear after a moment and are also read out to screen readers. After
some actions (such as unpinning everything or clearing the recent list), *Undo* is offered for 6 seconds, and stays
while the pointer is over it. Nothing else in Uku is timed. The keyboard focus is always visible: on a link, a ring goes
around the link's words.

## Screen readers

Uku tells screen readers how a document is built, not just its text:

- **Headings** have their level, so you can jump between them (also with Alt+↓ / Alt+↑ in Uku).
- **Lists** are lists, with each item's position (*2 of 5*); bullets aren't read out. Task boxes are named by their task.
- **Alerts, quotes, code blocks** (*Code, python*), **tables**, **footnotes**, **formulas** and **diagrams** are named,
  so you know where you are.
- **Links** are reached with Tab and read as links, with their address; pictures are read by their description.
- The page is a document named by the document's title; the sidebar is navigation, the search and find are search.
  Side by side, each side is named, and moving between them is announced.

Every button, field and menu item has a name, in all of Uku's languages. Things that happen without moving the focus
are read out: *Saved*, *Copied*, the number of matches while you type in find, a message such as *The file changed on
disk while you were editing it*, and the new text size.

Uku is built for Narrator and NVDA on Windows and VoiceOver on the Mac, but hasn't yet been tested end to end with each
of them, and screen reader support on Linux depends on your desktop. If anything in Uku doesn't work with your screen
reader, please tell me (below): it will be treated as a bug.

## Languages

Uku is available in English, German, Spanish, Russian, Ukrainian and Tatar, switchable at any time in Settings ▸
General without restarting.

## Tell me what doesn't work

If something in Uku is hard or impossible to use for you, write to
[garipov.dinar@gmail.com](mailto:garipov.dinar@gmail.com). Please mention your operating system and its version, and the
assistive technology or setting you use.
