# GoldenBoyMafe — People Survey & Charts (MIT App Inventor)

Two-screen classroom project for the Computer Science/IT class.

**Original date (internal metadata of the `.aia` file):** 09/27/2021

## What the app does

**Screen1 — Data entry**
A simple form to register people: name, age and gender (radio buttons `sexo`/`mark_sexo`). Each entry is stored in a local database (`bd_pessoas`, a TinyDB). On submit (`btn_ok`), the app:
- Saves the person's data.
- Recalculates and displays running statistics: total number of people registered (`lbl_pessoas`), total number of men (`lbl_total_de_homem`), and the average age of women (`lbl_media_de_mulher`).
- `btn_limpar` clears the input fields to register a new person.

**Screen2 — Charts**
Reads the same database (`bdpessoa`) and draws pie and column charts (`pizza`, `coluna`) with the `ChartMaker` extension, rendered inside a `WebViewer`. A "voltar" (back) button returns to Screen1.

## Components used
- `TinyDB` for local storage of the people database
- `Notifier` for alerts
- `ChartMaker` extension + `WebViewer` for pie/bar charts on Screen2
- Multiple `HorizontalArrangement` layout containers

## Files
- [`GoldenBoyMafe.aia`](GoldenBoyMafe.aia) — source project, can be reopened at [ai2.appinventor.mit.edu](https://ai2.appinventor.mit.edu) via *Import project*.
