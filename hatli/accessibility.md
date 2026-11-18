---
permalink: /hatli/accessibility/
---

# Hatli: Accessibility

**Last updated: November 18, 2026**

Hatli should work for everyone: whether you read and write your mail with a mouse, only the keyboard, a switch, your
voice or a screen reader; whether you need more contrast, larger text or less motion. This page lists what Hatli does
for that on Windows, macOS and Linux, where to find the settings, and what doesn't work yet.

Hatli aims to meet the [Web Content Accessibility Guidelines (WCAG) 2.2](https://www.w3.org/TR/WCAG22/) at level AA,
where they apply to a desktop app. Much of it is checked by Hatli's automated tests before every release (see
[How it is checked](#how-it-is-checked)).

The settings below are in **Settings** (Ctrl+,): *Appearance* for themes, text size and fonts, *Accessibility* for
motion, links, the focus ring and announcements. The search box at the top of Settings finds any setting by its words.

Shortcuts are written for Windows and Linux; on a Mac, use ⌘ for Ctrl.

## See it the way you need

- **Themes.** Settings ▸ Appearance: *System* (the default) follows your system's light or dark setting, or choose
  *Light*, *Sand*, *Aurora*, *Dark*, *Forest*, *Midnight*, *High contrast* or *High contrast light*, and one of nine
  accent colors. You can choose which theme your system's light and dark each show, and make two themes of your own
  from any of them.
- **High contrast, dark or light**, at a contrast of 7:1 or more.
- **Your system's contrast settings.** On *System*, Hatli switches to high contrast by itself when your system's is
  on: the light one for a light contrast theme (such as Windows' *Desert*), the dark one otherwise. On Windows it also
  takes the colors of your contrast theme. On a Mac, *Increase contrast* does the same.
- **Readable colors.** Text has a contrast of at least 4.5:1 with its background, and the focus ring, borders and
  states at least 3:1, in every theme and with every accent color.
- **Bigger text.** Ctrl+= and Ctrl+- make the text larger or smaller, from 85 % to 200 % (Ctrl+0 goes back to 100 %).
  The whole window grows with it, and the panes give way rather than squeeze: even a narrow window still works. The
  text of messages has a size of its own in Settings ▸ Appearance, also from 85 % to 200 %.
- **Fonts.** Settings ▸ Appearance: Inter, Atkinson Hyperlegible, Literata, Andika, OpenDyslexic or any font installed
  on your computer, chosen apart for Hatli itself and for your mail.
- **Density.** *Compact*, *Comfortable* or *Spacious*: how much room the rows and lists have.
- **Plain text.** Settings ▸ Mail ▸ *Prefer plain text* shows a message's plain-text version, in your font and colors,
  when it has one.

## Not just color

Nothing in Hatli is told only by color:

- An account's color always comes with its name or its initials.
- Unread messages are bold as well as marked.
- Flagged, pinned and snoozed messages have icons and names.
- Links are underlined (Settings ▸ Accessibility ▸ *Underline links*, on by default).
- Errors say what is wrong in words.

## Less motion

Hatli's motion is short and only shows where a change came from: nothing blinks, nothing loops, and nothing moves while
you read.

Settings ▸ Accessibility ▸ Motion: *System* (the default) follows your system: Windows' *Animation effects*, macOS's
*Reduce motion*, GNOME's animations. *Reduced* turns off every fade and slide in Hatli, its standard controls included;
*Full* keeps them.

## Keyboard

Everything in Hatli can be done without a mouse. Single letters act only when you aren't typing in a text field.

| Action | Shortcut |
|---|---|
| Command palette: every command, every group, any message | Ctrl+K |
| Move between the sidebar, the message list and the message | F6 / Shift+F6 |
| Next / previous conversation | J / K, or ↓ / ↑ |
| Open a conversation in its own window | Enter |
| New message | Ctrl+N or C |
| Reply, reply all, forward | R, Shift+R, F |
| Archive, delete (with Undo) | E, Delete |
| Flag, pin, snooze until tomorrow, read or unread | S, P, H, U |
| Search | / or Ctrl+F |
| Send (in a message or the quick reply); save an event or a contact | Ctrl+Enter |
| On an address you are writing to: move between To, Cc and Bcc; change it; remove it | ←, Enter, Delete |
| Go to the account group at that place | Ctrl+1 to Ctrl+9 |
| Mail, Contacts, Calendar | Ctrl+Shift+1, 2, 3 |
| Show or hide the sidebar | Ctrl+B |
| Focus mode | Ctrl+Shift+F |
| Refresh | F5 |
| Text size larger / smaller / 100 % | Ctrl+= / Ctrl+- / Ctrl+0 |
| Settings | Ctrl+, |
| Close the palette or a dialog, leave focus mode, clear the search | Esc |
| Quit | Ctrl+Q |

⋯ ▸ **Keyboard shortcuts** (on a Mac, in the menu bar) lists them, and Settings ▸ Accessibility ▸ *Keys* too.

**Nothing only by drag.** Every drag has a command: *Move to…* for messages, *Move up* and *Move down* for accounts and
groups, and moving an account to another group in Settings.

**Visible focus.** The keyboard focus always has a 2-pixel ring. Settings ▸ Accessibility ▸ *Always show the focus
ring* shows it after mouse clicks too.

**Easy to hit and to name.** Every button and box you can click is at least 24 × 24 pixels, most 36. Every control's
name contains the words it shows, so voice control (Voice Access, Voice Control, Dragon) finds it by what you see.

**No time limits.** Nothing you have to do in Hatli is timed. Messages such as *Archived* stay for six seconds with
*Undo* and can be dismissed; every action that removes something can be undone, and *Undo send* gives you time to
take back a message after pressing Send (Settings ▸ Mail).

## Screen readers

Hatli works with Narrator and NVDA on Windows, VoiceOver on the Mac and Orca on Linux, and tells them how the window is
built, not just its text:

- **The parts of the window** (the sidebar, the message list, the conversation) are named regions, and F6 moves
  between them.
- **A message in the list** is read as one sentence, its state first: *Unread, flagged. Timur Ganiev. Launch plan… 3
  messages.*
- **A message's own text**, its links and its tables are read as a document, inside the conversation.
- **Headings** have their level, and lists their items.
- **What happens** without moving the focus is read out: *Archived*, *Sent*, *12 results*, *Showing Work*, and errors
  when sending. Settings ▸ Accessibility ▸ *Announce actions* (on by default) turns this on and off.
- **Who a message is from**: the address is always shown and read beside the sender's name, and where a link really
  goes is shown before you open it.

Every button, field and menu item has a name, in all of Hatli's languages.

## What doesn't work yet

These are known gaps. They're being worked on, and this page changes when each is fixed:

- **Screen readers haven't been tested end to end.** Hatli is built for Narrator, NVDA and VoiceOver, and its automated
  tests check what they are told, but a full session with each is still to come. On Linux, how much reaches Orca
  depends on your desktop and hasn't been measured yet.
- **Voice Control on the Mac** hasn't been tried through a whole session yet.
- **HTML mail is shown as its sender designed it**, colors included; it isn't yet recolored by your theme or by high
  contrast. *Prefer plain text* (Settings ▸ Mail) shows the plain version where a message has one.

## How it is checked

Before every release, Hatli's automated tests check that every control has a name (in English and German) on every
screen, the roles of lists, rows and their state, regions and headings, moving between the parts of the window with
F6, what is announced, contrast in all eight themes with every accent color, targets of at least 24 pixels, names that
contain their visible words, and no animation when motion is reduced. By hand, on each system, the published build is
used with the keyboard alone, the screen readers above, high contrast, grayscale, reduced motion and text at 200 %.

## Languages

Hatli is available in English, German, Spanish, Russian, Ukrainian and Tatar, switchable at any time in Settings ▸
General without restarting.

## Tell me what doesn't work

If something in Hatli is hard or impossible to use for you, write to
[garipov.dinar@gmail.com](mailto:garipov.dinar@gmail.com). It will be treated as a bug. Please mention your operating
system and its version, and the assistive technology or setting you use.
