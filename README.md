# GestionaleV2-releases

Repository per le release del **Gestionale V2**.

## Inizializzazione del repository

Segui questi passaggi per inizializzare il repository in locale.

### 1. Clona il repository

```bash
git clone https://github.com/Sunacchi/GestionaleV2-releases.git
cd GestionaleV2-releases
```

### 2. Verifica il branch predefinito

```bash
git branch -a
```

### 3. Aggiungi i file iniziali

Se il repository è vuoto o deve contenere i file di release, copia i file necessari dentro questa cartella.

### 4. Crea il primo commit

```bash
git add .
git commit -m "chore: inizializza repository"
```

### 5. Pubblica sul repository remoto

```bash
git push origin HEAD
```

## Uso previsto

Questo repository serve a distribuire e aggiornare il **Gestionale V2**.
Può contenere:

- pacchetti di release
- file di aggiornamento
- istruzioni di distribuzione
- changelog delle versioni

## Note

- Mantieni una struttura chiara per versione, ad esempio `v1.0.0/`
- Aggiungi un changelog per ogni release
- Se necessario, documenta i prerequisiti di installazione o aggiornamento
