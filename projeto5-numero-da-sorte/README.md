# Projeto_5 — Lucky Number Generator (MIT App Inventor)

Small single-screen classroom exercise for the Computer Science/IT class.

**Original date (internal metadata of the `.aia` file):** 09/03/2021

## What the app does
Tapping `btn_1` runs a procedure called `Sorte` ("Luck"): it generates a random integer between 2–50 into `lbl_1`, and another random integer between 19–80 into `lbl_2`. If, by chance, both random numbers come out equal, the app automatically re-rolls (a `while` loop keeps calling `Sorte` until the two numbers differ). `btn_Limpar` clears both labels.

## Components used
- 2 `Button` (Draw / Clear)
- 2 `Label` (show the two "lucky" numbers)
- `math_random_int` blocks for the random draws, inside a `while` loop that guarantees distinct results

## Files
- [`Projeto_5.aia`](Projeto_5.aia) — source project, can be reopened at [ai2.appinventor.mit.edu](https://ai2.appinventor.mit.edu) via *Import project*.
- [`Projeto_5.apk`](Projeto_5.apk) — compiled app, ready to install on Android.
