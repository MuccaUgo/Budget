# Budget

Webapp per tenere le entrate e le uscite mese per mese, pensata per iPhone 14.
Prende il posto del foglio Numbers `BUDGET.numbers`.

**Apri l'app:** https://muccaugo.github.io/Budget/

## Cosa fa

- **Inserimento veloce.** Tocchi +, scrivi l'importo con il tastierino e scegli una delle descrizioni che usi più spesso. La categoria si imposta da sola.
- **Quanto ti resta.** Per il mese in corso mostra l'avanzo, quanto puoi spendere al giorno fino a fine mese, il ritmo rispetto ai mesi precedenti e l'avanzo stimato.
- **Dove vanno i soldi.** Categorie, spese più grandi, piccole spese sotto i 10 €, giorni della settimana in cui spendi di più, fonti di entrata.
- **Obiettivo di risparmio.** Se lo imposti, l'importo giornaliero tiene conto di quello che vuoi mettere da parte.
- **Soldino**, la moneta mascotte, cambia faccia in base a come va il mese: sorride se sei in linea, suda se stai spendendo troppo in fretta, festeggia i mesi in cui risparmi tanto.
- **Funziona offline** e si installa sulla schermata Home come un'app.

## Installazione su iPhone

1. Apri il link in **Safari**.
2. Tocca **Condividi**, poi **Aggiungi alla schermata Home**.
3. Apri Budget dall'icona sulla Home. Importa i dati da qui, non dalla scheda di Safari: l'app sulla Home tiene i dati separati da Safari.

## I tuoi dati

I movimenti restano **solo sul dispositivo**, non su questo repository né su un server.

- **Backup:** scheda *Backup* › *Salva backup su iCloud* › *Salva su File* › iCloud Drive. L'app ti ricorda di farlo se passano più di 7 giorni.
- **Ripristino:** *Ripristina da un backup* e scegli il file `.json`. Con **Unisci** puoi combinare i dati di iPhone e Mac senza doppioni.
- **Su Mac con Chrome o Edge** puoi attivare il *Backup automatico*: scegli un file in iCloud Drive e l'app lo aggiorna a ogni modifica.
- **Esporta per Numbers o Excel:** crea un CSV con tutti i movimenti.

Per importare il vecchio foglio Numbers usa *Ripristina da un backup* con il file `Budget-da-Numbers.json`.

## Aggiornare l'app

Dopo aver cambiato i file, aumenta il numero in `CACHE` dentro `sw.js` (per esempio `budget-v2`), così gli iPhone scaricano la nuova versione.

## File

| File | Contenuto |
|---|---|
| `index.html` | L'app completa: interfaccia, grafici, salvataggio |
| `sw.js` | Service worker per l'uso offline |
| `manifest.webmanifest` | Nome, colori e icone per l'installazione |
| `icons/` | Icone dell'app |
| `fonts/` | Font Fredoka (licenza SIL OFL, vedi `fonts/OFL.txt`) |
