# prova_a — People Survey with Statistics (MIT App Inventor)

Exam/assignment project ("tarefa"/"prova_a") for the Computer Science/IT class.


**Original date (internal metadata of the `.aia` files):**
- `tarefa-v1.aia`: 11/18/2021, 03:41 UTC
- `tarefa-v2-final.aia`: 11/18/2021, 04:54 UTC (about an hour later — the final submitted version)

## What the app does
A data-collection form: for each person, the user enters **name** (`txt_nome`), **age** (`txt_idade`), picks a **gender** from a list (`lis_sexo`) and a **car brand** from a list (`lis_carro`). Tapping `btn_cadastrar` saves the entry to a local database (`BDpessoas`, TinyDB) and updates a set of running statistics shown on screen:

- Total number of people registered (`lbl_resultado_de_pessoas`)
- Total number of men over 27 years old (`lbl_total_homens_27`)
- Total number of women under 50 years old (`lbl_total_mulheres_abaixo_de_50_anos`)
- Total number of women who own a Chevrolet (`lbl_total_mulheres_chevrolet`)

`btn_sair` closes the app. `Notificador1` shows validation alerts (e.g. empty fields).

## Components used
- `TinyDB` for local storage
- `ListPicker`/`Spinner`-style lists for gender and car brand
- `Notifier` for alerts
- Multiple `HorizontalArrangement` layout containers

## Files
- [`tarefa-v1.aia`](tarefa-v1.aia) — earlier version, saved 03:41 UTC.
- [`tarefa-v2-final.aia`](tarefa-v2-final.aia) — final version, saved about an hour later (04:54 UTC). Both are kept to show the project's progression on the same day.
