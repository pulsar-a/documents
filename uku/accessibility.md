---
permalink: /uku/accessibility/
---

# Uku: Accessibility

**Last updated: November 11, 2026**

Uku should work for everyone: whether you read with a mouse, only the keyboard, a switch, your voice or a screen reader;
whether you need more contrast, larger text, more space between the lines, less motion or the text read aloud. This page
lists what Uku does for that on Windows, macOS and Linux, where to find the settings, and what doesn't work yet.

Uku aims to meet the [Web Content Accessibility Guidelines (WCAG) 2.2](https://www.w3.org/TR/WCAG22/) at level AA,
where they apply to a desktop app. Much of it is checked by Uku's automated tests before every release (see
[How it is checked](#how-it-is-checked)).

Most of these settings are in **Settings ▸ Accessibility** (Ctrl+,), grouped by need: *Seeing*, *Reading*,
*Listening*, *Motion* and *Keyboard*. The welcome page links there too, and the search box at the top of Settings finds
any setting by its words.

Shortcuts are written for Windows and Linux; on a Mac, use ⌘ for Ctrl and ⌥ for Alt, except where the table says
otherwise. These are the default shortcuts: you can change any of them in Settings ▸ Keyboard.

## See it the way you need

- **Themes.** The **Aa** button in the toolbar, or Settings ▸ Appearance: *System* (the default) follows your system's
  light or dark setting, or choose *Light*, *Sepia* (warm paper for long reading), *Sage*, *Dusk*, *Dark*, *Espresso*,
  *Night* (near black), *High contrast* or *High contrast light*. You can also pick an accent color.
- **High contrast, dark or light.** *High contrast* is black with white text, a yellow accent and a cyan focus ring;
  *High contrast light* is white with black text, dark blue links and a purple focus ring, at 7:1 or more. In both,
  alerts and messages are outlined instead of tinted. Settings ▸ Accessibility ▸ Seeing has a *High contrast* switch.
- **Your system's contrast settings.** On *System*, Uku switches to high contrast by itself when your system's is on:
  the light one for a light contrast theme (such as Windows' *Desert*), the dark one otherwise. On Windows it also takes
  the colors of your contrast theme, wherever they keep enough contrast. On a Mac, *Increase contrast* does the same.
- **Readable colors.** Text has a contrast of at least 4.5:1 with its background, and the focus ring, borders and other
  parts at least 3:1, in every theme and with every accent color, including code and its syntax colors.
- **Bigger text.** Ctrl+= and Ctrl+- make the document's text larger or smaller, from 70 % to 400 % (Ctrl+0 goes back
  to 100 %); Ctrl and the mouse wheel, or pinching on a trackpad, do the same. Also in **Aa** ▸ *Text size* and
  Settings ▸ Reading. The page reflows to fit the window: even in a narrow window at 400 %, nothing is cut off and only
  wide tables and code scroll sideways. The rest of the window keeps its size.
- **Fonts.** Settings ▸ Reading ▸ *Font*: Sans, Serif, Mono, Literata, Atkinson Hyperlegible, OpenDyslexic, Andika, or
  any font installed on your computer. Code has its own font, also in Settings ▸ Reading.
- **Line width.** **Aa** ▸ *Line width*: narrow, medium, wide or the full window.
- **Text spacing.** Settings ▸ Reading: *Line spacing* (up to 2.4), *Letter spacing* and *Word spacing* (up to 0.12 and
  0.32 of the text's height), and *Paragraph spacing* (up to double). They apply to everything on the page but code, and
  nothing is cut off even at the widest spacing and a large text size.

## Help with reading

- **Easy reading.** Settings ▸ Accessibility ▸ Reading: one switch for a plain font (Atkinson Hyperlegible), more room
  between lines, letters, words and paragraphs, a narrow column, no slanted letters and a soft page. It never makes
  anything tighter than you had set it, and when you turn it off, your own choices are back.
- **Reading ruler.** Settings ▸ Accessibility ▸ Reading: a clear band across the line you're reading, with the rest of
  the page dimmed, so your eye keeps its line. It follows the pointer, or Alt+Shift+↓ / Alt+Shift+↑ move it a line at a
  time. You can choose how much the rest is dimmed and how many lines the band covers. Off by default.
- **Quiet focus mode.** Settings ▸ Accessibility ▸ Reading: in focus mode (F11), only the text is left: no heading
  marks, corner tools or reading progress, the properties folded and nothing moving. What it hides can still be reached
  with the keyboard. Off by default.
- **Read aloud** (Windows for now): Ctrl+Shift+U, or ⋯ ▸ *Read aloud*, reads the page with your computer's own voices,
  from where you are to the end. The sentence being read is tinted and the word being said is underlined, and the page
  keeps up with it. A bar at the bottom has the previous and next sentence, pause, the speed (0.5× to 2×) and stop;
  Alt+Shift+← / Alt+Shift+→ go a sentence back or on, Esc stops. Formulas are read in words, pictures by their
  description and diagrams by what they show. Settings ▸ Accessibility ▸ Listening sets the voice, the speed and
  whether code is read too. With *Automatic*, Uku picks a voice in the document's language (from `lang` in its front
  matter), and tells you if your computer has none. Uku uses only voices installed on your computer, never an online
  service.

## Not just color

Nothing in Uku is told only by color:

- Alerts (*Note*, *Tip*, *Important*, *Warning*, *Caution*) have an icon and their name, not only a tint.
- Links are underlined as well as colored, and show what a click does: a link to a place on the same page has a dotted
  underline, a link that leaves Uku (a website, an email address, a file another app opens) has a small ↗, and a link
  to a file that doesn't exist has a dashed underline and, when clicked, says *Can't find …*.
- Done tasks are struck through as well as muted, and their box is ticked.
- Find in the document marks the current match with an outline as well as a stronger color, and says *3 of 12*.
- Added and removed lines in code keep their `+` and `−`.
- A folder's color is also named in its tooltip and to screen readers.

Everything Uku tells apart by color is tested to stay apart for people with protanopia, deuteranopia and tritanopia, in
every theme. Diagrams use a palette made to be told apart with any kind of color vision.

## Less motion

Uku has little motion to begin with: a few short fades, and nothing in the interface that moves while you read. The page
never animates when a document changes on disk, and read aloud moves the page in jumps, never by sliding.

Settings ▸ Accessibility ▸ Motion: *System* (the default) follows your system: Windows' *Animation effects*, macOS's
*Reduce motion*, GNOME's animations. *Reduced* turns off every fade, slide and easing in Uku, its standard controls
included; *Full* keeps them.

Animated pictures (GIF, WebP) play only while they are on screen. *Animated pictures* in the same group: *Play while
motion is on* (the default), *Click to play* (each stays still until you press its play button) or *Never*. A picture's
own play button always plays it.

## Keyboard

Everything in Uku can be done without a mouse.

| Action | Shortcut |
|---|---|
| All shortcuts | F1 |
| Move between the toolbar, the sidebar and the page | F6 / Shift+F6 |
| Next / previous link (or button, task box) on the page | Tab / Shift+Tab, then Enter to follow a link |
| Next / previous heading | Alt+↓ / Alt+↑ |
| Fold or unfold a heading's section | Enter on the heading |
| Fold / unfold all sections | Ctrl+Shift+C / Ctrl+Shift+E |
| Everything on the page, by kind (headings, links, tables, pictures…) | Ctrl+J |
| Where am I (the section, how far you've read) | Ctrl+Shift+I |
| Scroll the page | Space / Shift+Space, Page Up / Page Down, arrows, Home / End |
| Find in the document | Ctrl+F, then Enter / Shift+Enter (or F3 / Shift+F3; Mac: ⌘G / ⇧⌘G) |
| Search the files | Ctrl+Shift+F |
| Back / forward | Alt+← / Alt+→ (Mac: also ⌘[ / ⌘]) |
| Open a file / a folder | Ctrl+O / Ctrl+Shift+O |
| Close the document / the workspace | Ctrl+W / Ctrl+Shift+W |
| Reload the document | F5 (Mac: ⌘R) |
| Show or hide the sidebar | Ctrl+Shift+L (Mac: also ⌃⌘S) |
| Edit / read | Ctrl+E |
| Open a document side by side / go to side 1–4 | Ctrl+\ / Ctrl+1 to Ctrl+4 |
| Read aloud: start, pause, go on | Ctrl+Shift+U |
| Read aloud: previous / next sentence | Alt+Shift+← / Alt+Shift+→ |
| Reading ruler: a line down / up | Alt+Shift+↓ / Alt+Shift+↑ |
| Text size larger / smaller / 100 % | Ctrl+= / Ctrl+- / Ctrl+0 |
| Undo what a message offers to undo | Ctrl+Z (outside the editor) |
| Settings | Ctrl+, |
| Focus mode | F11 (Mac: also ⌃⌘F) |

**Ctrl+J** lists what the page holds, in reading order: headings, links, tables, pictures, diagrams, formulas, code,
lists, quotes, alerts and tasks, each with what it says. Pick a kind, type to narrow the list, and Enter goes there.
**Ctrl+Shift+I** says, and shows, which document you're in, which section (*Install, section 3 of 8*) and how far
you've read.

**Reading keys.** Turn on *Reading keys* in Settings ▸ Accessibility ▸ Keyboard (off by default), and on the page a
single letter goes to the next element of its kind, as in a screen reader's browse mode: **H** heading (**1**–**6** a
heading of that level), **T** table, **K** link, **G** picture, **D** diagram, **F** formula, **C** code block, **L**
list, **Q** quote, **A** alert, **X** task. With Shift, the one before. When there's none left, Uku says so, and nothing
moves. On a keyboard layout other than English, the key in the same place works.

**Nothing only by hover or drag.** The tools of a code block, diagram, formula or table (copy, source, *Show as text*,
expand) show when Tab reaches them, not only under the pointer. In the sidebar, the arrow keys move through files and
folders, F2 renames, Delete (Mac: ⌘⌫) deletes, and the context-menu key (or Shift+F10) opens an item's menu, with
*Move to…* to move a file or folder, and *Move up* / *Move down* to reorder pinned items and a workspace's folders. To
make the sidebar or a side wider or narrower, Tab to the line between them and press ← or →. A link's menu (open it
with another app, copy its address and more) opens with the context-menu key too. Pictures can be reached with Tab and
opened larger with Enter (Esc closes them).

**Easy to hit and to name.** Every button and box you can click is at least 24 × 24 pixels, even where it looks
smaller, such as a task's box or the × buttons. Every control's name contains the words it shows (or its tooltip's), so
voice control (Voice Access, Voice Control, Dragon) finds it by what you see.

**No time limits.** Short confirmations such as *Saved* or *Copied* disappear after a moment and are also read out to
screen readers. After some actions (such as unpinning everything or clearing the recent list), *Undo* is offered for 6
seconds, and stays while the pointer is over it or it has the keyboard focus; Ctrl+Z undoes it too. Nothing else in Uku
is timed.

The keyboard focus is always visible: on a link, a ring goes around the link's words.

## Screen readers

Uku tells screen readers how a document is built, not just its text:

- **Headings** have their level, so you can jump between them (also with Alt+↓ / Alt+↑ in Uku). A heading whose section
  can fold says whether it is expanded or collapsed, and your screen reader's own commands fold it.
- **Lists** are lists, with each item's position (*2 of 5*); bullets aren't read out. Task boxes are named by their task.
- **Tables** are tables with header cells, named with their size (*Table, 4 columns, 12 rows*).
- **Code blocks** are named with their language and length (*Code, python, 12 lines*).
- **Pictures** are read by their description. A picture without one says so (*Picture, no description: chart.png*), and
  a picture marked as decorative (`alt=""`) isn't read at all.
- **Formulas** are read in words (*square root of x plus 1, end of root*), not as raw TeX; the TeX is there as help.
- **Diagrams** (Mermaid) are described by their structure in words: a flowchart's boxes and arrows in order, a sequence's
  messages, a pie chart's slices with their shares. If the diagram has its own `accTitle` and `accDescr`, those are used.
  *Show as text* in a diagram's tools puts the same text on the page for everyone.
- **Alerts, quotes and footnotes** are named, so you know where you are.
- **Links** are reached with Tab and read as links, with their address.
- **The document's language.** When a document's front matter gives a language (`lang: tt`) other than Uku's, the page
  and *Where am I* say so (*Language: Tatar*).
- **The window.** The page is a document named by the document's title; the sidebar is navigation, the search and find
  are search, the toolbar is a toolbar. Side by side, each side is named, and moving between them is announced.

Every button, field and menu item has a name, in all of Uku's languages. Things that happen without moving the focus
are read out: *Saved*, *Copied*, the number of matches while you type in find, a message such as *The file changed on
disk while you were editing it*, the new text size, *no more headings* at either end, and read aloud starting, pausing
and stopping (but not the text it reads, so it doesn't talk over itself). Dialogs are announced by their question.

## For people who write the documents

If you use an AI agent with Uku (Settings ▸ AI agents), its check of a document also points out what makes the
document hard to follow with a screen reader: pictures without a description, a heading level skipped, link words that
say nothing (*click here*, a bare address), a table without a header row, a diagram without a title or description.
Each hint says why it matters and how to fix it, so the agent can fix it as it writes.

## What doesn't work yet

These are known gaps. They're being worked on, and this page changes when each is fixed:

- **Screen readers haven't been tested end to end.** Uku is built for Narrator and NVDA on Windows and VoiceOver on the
  Mac, and its automated tests check what they are told, but a full session with each is still to come. On Linux, how
  much reaches Orca hasn't been measured yet and depends on your desktop.
- **A paragraph is read as a whole.** Your screen reader can't yet move through it by line, word or character, or spell
  a word.
- **Tables, code, formulas and diagrams are read as a whole.** A table's cells can't yet be reached one by one, code
  isn't read line by line with its indentation, and you can't yet step through a formula or a diagram part by part.
- **The screen reader's voice doesn't switch to a document's language** by itself; Uku says the language instead. (Read
  aloud does switch.)
- **Read aloud works on Windows only** for now; on macOS and Linux, use your system's own speech for now.
- **Your system's text size** (such as Windows' *Text size*) isn't followed by Uku's own buttons and menus yet; the page
  can be made larger with Ctrl+=.
- **Animated pictures that flash quickly** aren't detected yet. Set *Animated pictures* to *Click to play* or *Never*
  if flashing affects you.

## How it is checked

Before every release, Uku's automated tests check that every control has a name (in English and German) on every
screen, the roles of the page's headings, lists, tables and other parts, moving by links and headings and with F6, what
is read out, contrast in every theme and accent color, colors for every kind of color vision, targets of at least 24
pixels, names that contain their visible words, no animation when motion is reduced, and nothing cut off at large text
sizes, wide spacing and in a narrow window.

## Languages

Uku is available in English, German, Spanish, Russian, Ukrainian and Tatar, switchable at any time in Settings ▸
General without restarting.

## Tell me what doesn't work

If something in Uku is hard or impossible to use for you, write to
[garipov.dinar@gmail.com](mailto:garipov.dinar@gmail.com). It will be treated as a bug. Please mention your operating
system and its version, and the assistive technology or setting you use.
