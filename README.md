# MyHeroStudio — rilasci

Qui si scarica **MyHeroStudio** di [MyHeroSoft](https://myherosoft.com/): l'ambiente di sviluppo che controlla ogni modifica di Claude Code (cosa cambia, perché, cosa coinvolge e come tornare indietro).

Questo repository contiene solo le versioni pubblicate. Il codice di MyHeroStudio non è pubblico.

## Installare

1. Apri l'ultima versione in [Releases](../../releases/latest) e scarica `MyHeroStudio-Setup-<versione>-x64.exe`.
2. Avvialo. Si installa per il tuo utente, senza permessi da amministratore.
3. Windows può mostrare «Windows ha protetto il PC» (SmartScreen), perché il programma non è ancora firmato digitalmente: scegli **Ulteriori informazioni → Esegui comunque**.
4. Al primo avvio MyHeroStudio propone di installare **Claude Code**, l'estensione ufficiale di Anthropic. Serve un abbonamento Claude (Pro, Max, Team o Enterprise) oppure una chiave API Anthropic, a carico di chi usa il programma.

Requisiti: Windows 10 o 11 a 64 bit.

## Aggiornamenti

MyHeroStudio controlla da solo se c'è una versione nuova, la scarica in sottofondo e la installa solo quando premi **Riavvia e aggiorna**. Ogni versione è firmata digitalmente da MyHeroSoft e viene verificata prima dell'installazione. Se una versione nuova non parte, il programma torna da solo a quella di prima. I tuoi progetti e le tue impostazioni non vengono mai toccati.

## File in questo repository

- `latest-stable.json`, `latest-beta.json`: l'ultima versione di ogni canale (firmata), letta dal programma per gli aggiornamenti.
- [Releases](../../releases): installer e file firmato di ogni versione.

---

**English.** MyHeroStudio releases by MyHeroSoft. Download the latest `MyHeroStudio-Setup-<version>-x64.exe` from [Releases](../../releases/latest) (Windows 10/11 x64, per-user install). Claude Code and a Claude subscription or Anthropic API key are required. Updates are signed, installed only when you choose "Restart and update", and roll back automatically if the new version does not start.
