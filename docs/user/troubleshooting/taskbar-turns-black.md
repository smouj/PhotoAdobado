---
title: The Windows taskbar turns black when PhotoCraft is maximized
description: Upstream PhotoCraft 0.8.2 fixed a Windows taskbar issue; check the current PhotoAdobado build before applying that advice.
order: 10
---

> **Upstream note:** The taskbar issue and fix below are documented for PhotoCraft 0.7.0–0.8.2. They have not been verified against a published PhotoAdobado package.

If this happens in PhotoAdobado, check the app version and Windows version, then report the issue to the [PhotoAdobado issue tracker](https://github.com/smouj/PhotoAdobado/issues).

## Symptoms

- You maximize the PhotoCraft window, or switch it to full screen, and the Windows taskbar turns completely black or is hidden.
- After you resize the window and maximize it again, a black bar the height of the taskbar stays at the bottom of the screen.

## Fix

1. Check your version in **Help › System Info…**.
2. Restart PhotoAdobado and test whether the taskbar behavior persists.
3. If it does, send your app version, Windows version, and steps to the [PhotoAdobado issue tracker](https://github.com/smouj/PhotoAdobado/issues).

A user who saw the black taskbar on 0.7.0 confirmed that it is gone in 0.8.2 ([issue 3864](https://github.com/storytold/photocraft/issues/3864)).

## Why this happens

PhotoCraft draws its own title bar. When such a window was maximized, Windows sized it to cover the whole screen, taskbar included, took it for a full-screen app and dropped the taskbar's background. The fix keeps a maximized PhotoCraft window clear of the taskbar ([issue 3144](https://github.com/storytold/photocraft/issues/3144), [pull request 3308](https://github.com/storytold/photocraft/pull/3308)).

## Still stuck?

If the problem persists, include a screenshot if it helps explain what you see. Do not attach private photos or documents; see [Get help with a problem](get-help.md).
