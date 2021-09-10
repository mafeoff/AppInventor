# MyPiano — Virtual Piano (MIT App Inventor)

Classroom project built for the Computer Science/IT class, based on the MIT App Inventor "MyPiano" template. It simulates a small 8-key piano on the phone screen.

**Original date (internal metadata of the `.aia` file):** 09/10/2021

## What the app does
The screen has 8 buttons, one for each musical note (**C, D, E, F, G, A, B**, and the high octave, **HIGH C**). When a button is tapped:

1. The app sets the corresponding audio file (`CNote.wav`, `DNote.wav`, etc.) as the source of the `Player1` component.
2. It updates a `Label` on screen showing which note was played (e.g. "C", "D"...).
3. It plays the sound through `Player1`.

In other words, it's a functional simple instrument: each key has its own real piano sound recorded as a project asset (`assets/CNote.wav`, `assets/DNote.wav`, etc.), and the app swaps the player's audio source on every click.

## Components used
- 8 `Button` components (one per note)
- 1 `Label` (shows the last note played)
- 1 `Player` (plays the `.wav` files)
- 1 `HorizontalArrangement` (lays the buttons out side by side)

## Files
- [`MyPiano_template_1B2.aia`](MyPiano_template_1B2.aia) — source project, can be reopened at [ai2.appinventor.mit.edu](https://ai2.appinventor.mit.edu) via *Import project*.
- [`MyPiano_template_1B2.apk`](MyPiano_template_1B2.apk) — compiled app, ready to install on Android.
