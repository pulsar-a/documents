---
permalink: /brinebook/accessibility/
---

# Brinebook: Accessibility

**Last updated: November 20, 2026**

Brinebook should work for everyone: whether you use a mouse, only the keyboard, your voice or a screen reader; whether
you need more contrast, larger text or less motion. This page lists what Brinebook does for that on Windows, macOS and
Linux, where to find the settings, and what doesn't work yet.

Brinebook aims to meet the [Web Content Accessibility Guidelines (WCAG) 2.2](https://www.w3.org/TR/WCAG22/) at level
AA, where they apply to a desktop app. Much of it is checked automatically before every release (see
[How it is checked](#how-it-is-checked)).

The settings below are in **Settings ▸ Look** (Ctrl+,). The search box at the top of Settings finds any setting by its
words. Shortcuts are written for Windows and Linux; on a Mac, use ⌘ for Ctrl.

## See it the way you need

- **Themes.** Settings ▸ Look ▸ *Theme*: *Match system* (the default) follows your system's light or dark setting, or
  choose *Glass light*, *Glass*, *Console light*, *Console*, *High contrast, light* or *High contrast*. You can also
  pick an accent color.
- **High contrast, dark or light.** White on black with a yellow accent, or black on white with a blue accent, every
  edge drawn, with a contrast of 7:1 or more.
- **Your system's contrast settings.** On *Match system*, Brinebook switches to its high contrast theme, light or dark,
  when your system asks for high contrast.
- **Readable colors.** Text has a contrast of at least 4.5:1 with what it sits on, in every theme, with every accent
  color, and over the glass themes' background picture (Settings ▸ Look tells you from which *Tint* every word reads
  clearly over your picture). *Dim background* and *Tint* make the glass more solid if you want plainer pages.
- **Bigger text.** Settings ▸ Look ▸ *Text size*, from 85 % to 200 %. The whole window grows with it, and nothing is cut
  off.
- **Fonts.** Settings ▸ Look ▸ *Font*: Brinebook's own fonts, or any font installed on your computer.

## Not just color

Nothing in Brinebook is told only by color:

- A ferment's status (preparing, fermenting, done, failed) always has its name beside its color, and what needs you
  says why in words.
- Wherever a color marks a kind of thing, its name is beside it.
- A rating has its number of stars named, and a failed ferment says *Failed* and why.
- The pH line marks pH 4.6 with a dashed line, named in words.

## Less motion

Brinebook has little motion to begin with: short fades and slides when you point at or choose something, and nothing
that moves while you read or type. Nothing loops and nothing blinks.

Settings ▸ Look ▸ *Motion*: on *Match system* it follows your system (Windows' *Animation effects*, macOS's *Reduce
motion*, GNOME's animations); *Reduced* takes out every animation, the standard controls' included.

## Keyboard

Everything in Brinebook can be done without a mouse, with a visible focus ring on what has the keyboard.

| Action | Shortcut |
|---|---|
| New batch | Ctrl+N |
| Ferments, Jars, Recipes, Pantry | Ctrl+1 to Ctrl+4 |
| Settings | Ctrl+, |
| Open the chosen item | Enter |
| Back from a page to its list | Alt+← |
| The ferment before / after on the shelf | Alt+↑ / Alt+↓ |
| Delete the chosen ferment (asked first, Undo after) | Delete |
| An item's menu | Context-menu key or Shift+F10 |
| The next field, its number selected | Tab or Enter in a number field |
| Add a line to the journal | Enter in the journal's line |
| Open or close the phone's pane | Ctrl+P |
| Paste copied photos | Ctrl+V outside a field |
| Search the settings | Ctrl+F in Settings |
| A photo shown large: the one before / after, first / last | ← / →, Home / End |
| The photo editor: rotate right / left | R / Shift+R |
| The photo editor: move the crop by 1 % / 10 % | Arrows / Shift+arrows |
| The photo editor: make the crop wider, narrower, taller, shorter | Alt+arrows |
| Close what is open (a message, the phone's pane, a photo, the editor, Settings) | Esc |

**Nothing only by drag.** Photos can be moved from the phone's inbox with *Move to…*, and pasted with Ctrl+V, as well
as dragged.

**Easy to hit and to name.** Every button and box you can press is at least 24 × 24 pixels. Controls are named by the
words they show, so voice control (Voice Access, Voice Control, Dragon) finds them by what you see.

**No time limits.** Nothing you have to do is timed. A message such as *Caraway sauerkraut deleted* stays six seconds,
longer while the pointer is on it, and is also read out to screen readers; Esc closes it.

**Asked before it's gone.** Brinebook asks before deleting or finishing something, and everything deleted can be
brought back with *Undo*. Settings ▸ Confirmations sets which questions it asks.

## Screen readers

Brinebook works with Narrator and NVDA on Windows, VoiceOver on the Mac and Orca on Linux:

- **Every control has a name**, in all six of Brinebook's languages.
- **A ferment on the shelf is read as one sentence**, its status first: *Fermenting. Garlic dill pickles. Day 5. On the
  counter · 1 day left · then In the fridge. pH 4.4.* A journal entry likewise.
- **Headings** carry their level, and the rail on the left is a landmark.
- **The salt to add** is read out as it changes while you type the weights.
- **The pH line** is read in words.
- **Each star** of a rating says how many stars it gives.
- **What happened is said** without moving the keyboard: *Added to the log*, *Caraway sauerkraut deleted*, how many
  settings a search found.

## What doesn't work yet

These are known gaps. They're being worked on, and this page changes when each is fixed:

- **Screen readers haven't been tested end to end.** Brinebook is built for Narrator, NVDA, VoiceOver and Orca, and its
  automated tests check that everything has a name, but a full session with each is still to come. On Linux, how much
  reaches Orca depends on your desktop.
- **No key moves between the window's regions** (the rail, the list, the page, the phone's pane) at once; Tab goes
  through them in order.
- **Charts** (the pH and temperature lines) are read in words as a whole; you can't yet step through them reading by
  reading.
- **Your system's text size** (such as Windows' *Text size*) isn't followed yet; use Settings ▸ Look ▸ *Text size*.

## How it is checked

Before every release, Brinebook's automated tests check that every control in every section has a name and is at least
24 × 24 pixels, that names follow the language, that a ferment is read as one sentence, that reduced motion leaves
nothing moving, and that the high contrast themes draw every edge. Every theme's colors are checked for contrast when
they are made.

## Languages

Brinebook is available in English, German, Spanish, Russian, Ukrainian and Tatar, switchable at any time in Settings ▸
General without restarting. Your journal stays as you wrote it.

## Tell me what doesn't work

If something in Brinebook is hard or impossible to use for you, write to
[garipov.dinar@gmail.com](mailto:garipov.dinar@gmail.com). It will be treated as a bug. Please mention your operating
system and its version, and the assistive technology or setting you use.
