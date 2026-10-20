---
title: Text moves when I start editing a PSD text layer
description: Upstream PhotoCraft 0.8.2 fixed a PSD text-position issue; check the current PhotoAdobado build before applying that advice.
order: 20
---

> **Upstream note:** This behavior and fix are documented for PhotoCraft 0.7.0–0.8.2. They have not been verified against a published PhotoAdobado package.

If the issue happens in PhotoAdobado, keep the original PSD unchanged and report it to the [PhotoAdobado issue tracker](https://github.com/smouj/PhotoAdobado/issues). The upstream PhotoCraft fix is summarized below for reference.

## Symptoms

- You open a PSD that was made in Photoshop and click one of its text layers with the **Horizontal Type Tool**. The text shifts, often to the left, as soon as editing starts.
- Centered text may show as left-aligned in the options bar.
- In some files, text that you click can disappear.

## Fix

1. Check **Help › System Info…** and note the PhotoAdobado version.
2. Reopen an untouched copy of the PSD and check whether the problem persists.
3. If it does, report the steps and app version to the [PhotoAdobado issue tracker](https://github.com/smouj/PhotoAdobado/issues).

If you already saved the file in 0.7.0 after the text moved, the moved text is now in the file. Go back to your original PSD if you still have it.

## Why this happens

Clicking a PSD text layer with the Type tool starts editing it, and PhotoCraft then lays the text out itself instead of showing the pixels Photoshop saved. PhotoCraft 0.7.0 read the alignment and size of each run of text only from Photoshop's default styles, and ignored part of the text position that recent Photoshop versions store. Both are fixed in 0.8.2 ([issue 3795](https://github.com/storytold/photocraft/issues/3795), [pull request 3819](https://github.com/storytold/photocraft/pull/3819)).

## Still stuck?

If the text still moves, keep the original PSD unchanged and attach a small sanitized example, the PhotoAdobado version, and the Photoshop version that saved it to the [PhotoAdobado issue tracker](https://github.com/smouj/PhotoAdobado/issues). See [Get help with a problem](get-help.md).
