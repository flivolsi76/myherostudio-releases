# MyHeroStudio

**L'ambiente di sviluppo che tiene sotto controllo ogni modifica dell'intelligenza artificiale.**
Di [MyHeroSoft](https://myherosoft.com/) · [myherostudio.myherosoft.com](https://myherostudio.myherosoft.com)

MyHeroStudio è un editor per Windows costruito attorno a **Claude Code**: Claude scrive il codice, MyHeroStudio ti dice sempre *cosa* ha cambiato, *perché*, *cosa coinvolge* e *come tornare indietro*. Regole, protezioni e controlli girano sul tuo computer, prima che le modifiche arrivino ai file.

> **30 giorni di prova gratuita**, poi abbonamento mensile. Serve un abbonamento Claude (Pro, Max, Team o Enterprise) oppure una chiave API Anthropic.

---

## Perché MyHeroStudio

- **Ogni modifica tracciata.** Per ogni richiesta a Claude: i file toccati, le righe aggiunte e tolte, il motivo spiegato da Claude, le classi e i metodi coinvolti.
- **Torni indietro quando vuoi.** Un file, una richiesta intera o tutto: con la valutazione di cosa si romperebbe *prima* di annullare.
- **Claude lavora dentro le tue regole.** File protetti, cartelle consentite, comandi vietati, segreti, dipendenze, architettura: bloccati prima che succeda.
- **Tutto sul tuo computer.** Il codice resta da te; l'IA è quella del tuo account Claude, alle condizioni di Anthropic.

## Le caratteristiche

### Controllo delle modifiche
- **File modificati sotto la chat**, come in Cursor: ultima richiesta e tutta la chat, `+N −M` per file, clic per vedere le differenze, **Annulla tutto** per l'ultima richiesta.
- **Storia** di tutte le richieste: chi ha cambiato cosa, quando e perché; filtri e ricerca.
- **Blueprint e mappa del progetto**: classi, metodi, collegamenti tra i file, metodi più lunghi, cicli tra moduli.
- **Annullamento intelligente**: prima di tornare indietro MyHeroStudio valuta l'impatto (con un controllo sul codice e con Claude) e ti avvisa se altri file dipendono da quella modifica.
- **Punto di ripristino git** automatico a ogni richiesta, senza toccare i tuoi rami.
- **Rete di sicurezza** a fine richiesta: anche le modifiche fatte da comandi o script vengono rilevate e registrate.

### Regole per l'IA
- **File protetti** (es. `.env`, `package.json`): Claude non li modifica senza il tuo **Consenti**, nemmeno con comandi del terminale o script.
- **Perimetro**: le cartelle in cui Claude può scrivere; il resto è bloccato o chiede conferma.
- **Comandi vietati**: `git push`, `npm publish`, `rm -rf`, `DROP TABLE`, `curl … | sh` fermati prima di partire.
- **Segreti nel codice**: password, chiavi e token bloccati prima che finiscano nei file.
- **Dipendenze nuove** con controllo della licenza (le copyleft si possono bloccare).
- **Regole di architettura** (es. «l'interfaccia non usa il database»), controllate a ogni scrittura.
- **Tetto per richiesta** (file e righe) e **budget** di utilizzo per richiesta e al giorno.
- **Controllo a fine richiesta**: test e compilazione automatici; se falliscono Claude deve sistemare prima di chiudere.
- **Conformità all'AI Act europeo**: regole per Claude sulle pratiche vietate, trasparenza e usi ad alto rischio, con avviso delle novità ufficiali.

### Metodo di lavoro con più ruoli
- **Controllore, collaudatore, operatore, revisore, segretario**: un compito passa da criteri di accettazione, test protetti, implementazione, revisione con un modello diverso e nota finale.
- **Ticket**: lavora su un ticket di Jira, Linear o GitHub; le richieste ne prendono l'etichetta e a fine lavoro il commento è pronto (pubblicato solo con la tua conferma).

### Agenti, skill e strumenti
- **Agenti** di MyHeroStudio e **agenti tuoi**, con il loro compito e il loro modello, a fine richiesta o quando li chiami.
- **Agenti nel cloud**: routine di Claude che girano anche a computer spento (es. «ogni mattina le mail importanti»), in sola lettura di partenza.
- **Skill** dal catalogo ufficiale di Anthropic o da un indirizzo, **globali**: installate una volta, valgono in tutti i progetti.
- **Server MCP** e **31 piattaforme** collegabili con un clic (GitHub, GitLab, Jira, Linear, Notion, Slack, Figma, Stripe…).
- **Browser integrato** che Claude usa per provare le tue pagine.

### Pensato per lavorare tranquilli
- **Un account Claude per progetto**, oppure una chiave API per progetto, conservata nel portachiavi sicuro di Windows.
- **Layout fisso**: file a sinistra, codice e browser al centro, chat a destra, impostazioni accanto.
- **Italiano e inglese**, che seguono la lingua dell'editor.
- **Aggiornamenti sicuri**: firmati digitalmente, installati solo quando premi *Riavvia e aggiorna*; se una versione nuova non parte, MyHeroStudio torna da solo a quella di prima. I tuoi progetti non vengono mai toccati.

## Installare

1. Scarica `MyHeroStudio-Setup-<versione>-x64.exe` dall'[ultima versione](../../releases/latest).
2. Avvialo: si installa per il tuo utente, senza permessi da amministratore.
3. Se Windows mostra «Windows ha protetto il PC» (SmartScreen): **Ulteriori informazioni → Esegui comunque**.
4. Al primo avvio MyHeroStudio propone **Claude Code** (estensione ufficiale di Anthropic) e la lingua.

Requisiti: Windows 10 o 11 a 64 bit, un abbonamento Claude o una chiave API Anthropic.

## Prezzo

**30 giorni gratis**, senza carta. Poi abbonamento mensile per utente (prezzo sulla [pagina del prodotto](https://myherostudio.myherosoft.com)). Allo scadere della licenza i tuoi progetti e Claude Code restano come sono: si spengono solo le funzioni di MyHeroStudio.

---

# English

**The development environment that keeps every AI change under control.** By [MyHeroSoft](https://myherosoft.com/).

MyHeroStudio is a Windows editor built around **Claude Code**: Claude writes the code, MyHeroStudio always tells you *what* changed, *why*, *what it affects* and *how to go back*. Rules, protections and checks run on your computer, before changes reach your files.

- **Every change tracked**: files, added and removed lines, Claude's reason, affected classes and methods; changed files under the chat like Cursor, with **Undo all**.
- **Go back any time** with an impact check before undoing; automatic git restore point per request.
- **Rules for the AI**: protected files, allowed folders, forbidden commands, secrets, new dependencies with license check, architecture rules, per-request limits and budget, end-of-request tests, EU AI Act guidance.
- **Multi-role working method**: controller, tester, operator, reviewer, secretary; tickets from Jira, Linear, GitHub.
- **Agents** (local and cloud routines), **global skills**, **MCP servers** and 31 one-click platforms, integrated browser.
- **One Claude account or API key per project**, Italian and English UI, **safe signed updates** with automatic rollback.

**30-day free trial**, then a monthly subscription. Download the latest `MyHeroStudio-Setup-<version>-x64.exe` from [Releases](../../releases/latest) (Windows 10/11 x64). Requires Claude Code and a Claude subscription or an Anthropic API key.
