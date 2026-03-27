# Pubblicare su GitHub Pages (Caso A)

Obiettivo: pubblicare `app-ads.txt` alla root di `https://st3fez.github.io/`.

## 1) Crea il repo su GitHub

Su GitHub crea un repository **pubblico** chiamato:

`st3fez.github.io`

## 2) Carica questi file nella root del repo

In questa cartella (`st3fez.github.io/`) trovi già:

- `app-ads.txt`
- `index.html`

## 3) Push (da PowerShell)

Esegui questi comandi dalla root del workspace (qui):

```powershell
cd st3fez.github.io
git init
git add -A
git commit -m "Add app-ads.txt for AdMob"
git branch -M main
git remote add origin https://github.com/st3fez/st3fez.github.io.git
git push -u origin main
```

## 4) Abilita Pages

Su GitHub: `Settings → Pages`

- **Source**: `Deploy from a branch`
- **Branch**: `main` + `/ (root)`

## 5) Verifica URL

Apri nel browser:

- `https://st3fez.github.io/app-ads.txt`

Deve mostrare esattamente la riga di AdMob.

