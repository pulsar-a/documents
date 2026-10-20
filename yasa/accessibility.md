---
permalink: /yasa/accessibility/
---

# Yasa: Accessibility

**Last updated: October 20, 2026**

Yasa should work for everyone, whether you use a mouse, only the keyboard, a screen reader, or need more contrast,
larger text or less motion. This page lists what Yasa does for that on the Mac, and where to find the settings.

## See it the way you need

- **Light, dark and high contrast.** Settings → Appearance & accessibility → *Theme*. *Follow system* (the default)
  follows your Mac's Light or Dark appearance. *High contrast* has stronger borders, no tinted backgrounds and no
  translucency; Yasa switches to it by itself when *Increase contrast* is on in System Settings → Accessibility →
  Display.
- **Readable colors.** All text has a contrast of at least 4.5:1 with its background, and borders, icons and the
  keyboard focus ring at least 3:1, in every theme and with every accent color. Yasa's automated tests check this
  with every build.
- **Bigger.** Zoom the whole app from 80 % to 200 % with ⌘= and ⌘−, or in Settings → Appearance & accessibility →
  *Zoom*. Layouts rearrange instead of cutting text off; anything shortened shows in full in a tooltip and to screen
  readers.
- **Larger click targets.** Settings → Appearance & accessibility → *Larger click targets* makes rows and buttons
  taller.
- **Less transparency.** *Reduce transparency* in the same place makes window backgrounds solid.

## Not just color

Nothing in Yasa is told only by color:

- Priority shows **!**, **!!** or **!!!** next to its color.
- An overdue deadline has a warning icon and says *Overdue*, not just red.
- A list's color always comes with its name.
- Done tasks have a checkmark; the current task is labelled *Current task*.
- Board columns have names, and can have icons as well as colors.

## Less motion

Yasa follows **Reduce motion** in System Settings → Accessibility → Display. You can also choose in Settings →
Appearance & accessibility → *Animations*: *Follow system*, *Reduced* or *Full*. With reduced motion there's no start
animation, and rows, cards and the menu bar popover appear and move without sliding or fading.

## Keyboard

Everything in Yasa works without a mouse, including moving cards on a board.

| | |
|---|---|
| Command palette: every command by name | ⌘K |
| All shortcuts | ? |
| Move between the sidebar, the list and the details | F6 |
| Add a task | ⌘N |
| Complete the selected task | Space |
| Plan for My Day / This Week | ⌘T / ⇧⌘T |
| Switch between list and board | ⌘E |
| Move a task or card | ⌥ + arrow keys |
| Undo | ⌘Z |
| Mini window | ⇧⌘M |

Every drag and drop also has a menu command (*Move to list…*, *Move to column…*). Deadlines can be typed the way
you'd say them: *tomorrow*, *fri 18:00*, *+3d*. Nothing in Yasa is timed, and **undo** covers everything you do.

## Screen readers

Every button, field and menu item in Yasa has a name for screen readers, in all of Yasa's languages. A task is read
with everything about it, for example: *"Renew passport. Not done. In My Day. Due Friday, October 24, overdue. High
priority. Tags: errand. Checklist 2 of 5. List Home, column To Do."* Changes that happen without moving the focus are
announced, such as *"Moved to In Progress, 2 of 4"* when you move a card, or *"Deleted Renew passport."* (⌘Z brings it
back).

VoiceOver on the Mac is still being tested end to end. If anything in Yasa doesn't work with VoiceOver or Voice
Control, please tell us (below): it will be treated as a bug.

## Languages

Yasa is available in English, German, Spanish, Russian, Ukrainian and Tatar, switchable at any time in Settings →
General without restarting.

## Tell us what doesn't work

If something in Yasa is hard or impossible to use for you, write to [garipov.dinar@gmail.com](mailto:garipov.dinar@gmail.com). Please mention your Mac's macOS version
and the assistive technology or setting you use.
