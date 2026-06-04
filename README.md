<div align="center">

# 🚀 GestionaleV2 — Releases

**Repository ufficiale per la distribuzione degli aggiornamenti del Gestionale V2.**

[![Latest Release](https://img.shields.io/github/v/release/Sunacchi/GestionaleV2-releases?style=flat-square&logo=github&label=Ultima%20Release&color=4c9ed9)](https://github.com/Sunacchi/GestionaleV2-releases/releases/latest)
[![Pipeline Status](https://img.shields.io/github/actions/workflow/status/Sunacchi/GestionaleV2-releases/release.yml?branch=main&style=flat-square&logo=githubactions&label=Pipeline)](https://github.com/Sunacchi/GestionaleV2-releases/actions)
[![License](https://img.shields.io/github/license/Sunacchi/GestionaleV2-releases?style=flat-square&color=brightgreen&label=Licenza)](./LICENSE)
[![Releases](https://img.shields.io/github/downloads/Sunacchi/GestionaleV2-releases/total?style=flat-square&label=Download%20Totali&color=orange)](https://github.com/Sunacchi/GestionaleV2-releases/releases)

---

*Distribuire aggiornamenti non è mai stato così semplice.*

</div>

---

## 📋 Indice

- [Descrizione](#-descrizione)
- [Struttura del Repository](#-struttura-del-repository)
- [Guida all'Utilizzo](#-guida-allutilizzo)
- [Creare una Nuova Release](#-creare-una-nuova-release)
- [Regole di Contributo](#-regole-di-contributo)
- [Supporto e Referenze](#-supporto-e-referenze)

---

## 📖 Descrizione

Questo repository è dedicato esclusivamente alla **distribuzione e alla gestione degli aggiornamenti ufficiali** del [Gestionale V2](https://github.com/Sunacchi/GestionaleV2) — un'applicazione desktop progettata per semplificare e velocizzare le attività amministrative.

### Cosa trovi qui:

- 📦 **Pacchetti di release** pronti all'installazione
- 📝 **Changelog dettagliati** per ogni versione
- 📌 **Istruzioni di installazione e aggiornamento**
- 🔧 **File di supporto** per la distribuzione automatica

> **Nota:** Per il codice sorgente, le issue e il progetto principale, fai riferimento al repository [GestionaleV2](https://github.com/Sunacchi/GestionaleV2).

---

## 🗂️ Struttura del Repository

Il repository è organizzato per versione, seguendo il formato [Semantic Versioning](https://semver.org/lang/it/):

```plaintext
GestionaleV2-releases/
│
├── v2.1.0/                          # Ultima release
│   ├── GestionaleV2-Setup-2.1.0.exe # Installer per Windows
│   ├── GestionaleV2-2.1.0.zip       # Archivio alternativo
│   ├── changelog.md                 # Novità della versione
│   └── istruzioni-installazione.md  # Guida all'installazione
│
├── v2.0.6/                          # Release precedente
│   ├── GestionaleV2-Setup-2.0.6.exe
│   ├── changelog.md
│   └── ...
│
├── v2.0.5/
│   └── ...
│
└── README.md                        # Questo file
```

---

## 🛠️ Guida all'Utilizzo

### Scaricare e installare un aggiornamento

1. Accedi alla **[sezione Releases](https://github.com/Sunacchi/GestionaleV2-releases/releases)** di questo repository.
2. Individua l'**ultima versione disponibile** (contrassegnata come *Latest*).
3. Nella sezione **Assets**, scarica:
   - `GestionaleV2-Setup-x.x.x.exe` — per un'installazione guidata su Windows
   - oppure il file `.zip` — per un'installazione manuale
4. Esegui il file scaricato e segui le istruzioni a schermo.
5. Consulta il `changelog.md` incluso per scoprire le novità della versione.

> 💡 L'applicazione include un **updater automatico** basato su Tauri che notifica la disponibilità di nuovi aggiornamenti direttamente dall'interfaccia.

---

## 🔖 Creare una Nuova Release

> Questa sezione è rivolta agli **sviluppatori e manutentori** del progetto.

### Procedura passo-passo

1. **Compila il progetto** dal repository principale [GestionaleV2](https://github.com/Sunacchi/GestionaleV2) seguendo le istruzioni di build.
2. **Crea una nuova directory** con il numero di versione:
   ```
   mkdir vX.Y.Z
   ```
3. **Copia i file binari** (installer `.exe`, archivio `.zip`, ecc.) nella nuova directory.
4. **Aggiorna il changelog** (`changelog.md`) con le modifiche introdotte nella versione:
   - Funzionalità aggiunte
   - Bug risolti
   - Breaking changes (se presenti)
5. **Aggiorna le istruzioni di installazione** se sono cambiati prerequisiti o passaggi.
6. **Crea il tag e la release** su GitHub:
   ```bash
   git tag -a vX.Y.Z -m "Release vX.Y.Z"
   git push origin vX.Y.Z
   ```
7. **Pubblica la release** dalla [pagina delle Releases](https://github.com/Sunacchi/GestionaleV2-releases/releases/new), allegando i file dalla directory `vX.Y.Z/`.

---

## 🤝 Regole di Contributo

Per mantenere il repository ordinato e professionale, rispetta le seguenti linee guida:

- **Struttura ordinata** — Ogni versione deve avere la propria directory nominata `vX.Y.Z`.
- **Documentazione completa** — Ogni directory di release deve contenere almeno un `changelog.md`.
- **Semantic Versioning** — Usa [SemVer](https://semver.org/lang/it/) per nominare versioni e directory (`MAJOR.MINOR.PATCH`).
- **Nessun file inutile** — Non caricare file temporanei, di debug o non correlati alla release.
- **Messaggio di commit chiaro** — Segui il formato [Conventional Commits](https://www.conventionalcommits.org/it/v1.0.0/) (es. `release: v2.1.0`).

---

## 💬 Supporto e Referenze

| Risorsa | Link |
|---|---|
| 🏠 Repository principale | [GestionaleV2](https://github.com/Sunacchi/GestionaleV2) |
| 📦 Tutte le releases | [Releases](https://github.com/Sunacchi/GestionaleV2-releases/releases) |
| 🐛 Segnala un problema | [Apri una Issue](https://github.com/Sunacchi/GestionaleV2-releases/issues/new) |

> Per problemi relativi all'**applicazione** (bug, suggerimenti, richieste di funzionalità), apri una issue nel [repository principale](https://github.com/Sunacchi/GestionaleV2/issues).
> Per problemi relativi a **download o aggiornamenti**, apri una issue in [questo repository](https://github.com/Sunacchi/GestionaleV2-releases/issues).

---

<div align="center">

Realizzato con ❤️ da [Sunacchi](https://github.com/Sunacchi)

</div>
