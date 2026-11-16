# DEMSY# JPAD — site web

Flask + SQLite. Administration : `/admin/login`.

## Test local (Windows)
Double-cliquez `run_jpad.bat` (ou : `python -m venv .venv`, `.venv\Scripts\python -m pip install -r requirements.txt`, `.venv\Scripts\python app.py`).
Au premier lancement, **le mot de passe admin temporaire s'affiche dans la fenêtre noire** (une seule fois).
Site : http://127.0.0.1:5000 — Admin : http://127.0.0.1:5000/admin/login

## Mot de passe oublié / ancienne base avec « 4509 »
```
set JPAD_ADMIN_USERNAME=admin
set JPAD_ADMIN_PASSWORD=UnNouveauMotDePasseLong
.venv\Scripts\flask --app app reset-admin
```
Si votre ancienne base contient l'utilisateur `demsy`, utilisez `JPAD_ADMIN_USERNAME=demsy`.

## Mise en ligne
Voir **DEPLOIEMENT.md**.
