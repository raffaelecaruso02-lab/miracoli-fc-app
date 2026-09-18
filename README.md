# Miracoli FC — gestionale

App per il mister: rosa, appello a bordo campo, convocazioni stampabili,
matchday con lavagna tattica e tre tempi, export Excel per la segreteria.

Online su:
**https://raffaelecaruso02-lab.github.io/miracoli-fc-app/**

---

## Com'è fatta

Un solo file HTML, senza librerie né server. Si apre nel browser e i dati
restano nel telefono di chi la usa.

```
index.html      l'app intera (HTML + CSS + JavaScript)
manifest.json   permette di installarla come app
icons/          icone per la schermata Home
```

## Installarla sul telefono

Apri l'indirizzo qui sopra da Safari o Chrome, poi menu condividi →
**Aggiungi a schermata Home**. Diventa un'icona come le altre app, senza
barra del browser.

## Come si aggiorna

Apri `index.html` qui su GitHub, clicca la matita, incolla la nuova
versione, *Commit changes*. Dopo un minuto è online, e i dati già
inseriti sul telefono non si toccano: stanno nel browser, non nel file.

## ⚠️ Il backup non è facoltativo

I dati vivono nel browser del telefono. Se si svuota la cronologia, si
cambia dispositivo o si disinstalla l'app, **spariscono**.

Ogni fine mese: ⚙ → **Scarica un backup**. Viene fuori un file `.json`
da conservare (mandalo a te stesso su WhatsApp o per email). Si rimette
dentro da ⚙ → *Ripristina da un backup*.

L'export Excel serve a chi legge i dati, non a rimetterli nell'app: per
quello serve il backup JSON.

## Cosa fa

- **Appello** — rosa con quattro stati (presente, assente, giustificato,
  infortunato), "segna tutti presenti" per partire dal caso normale,
  note tecniche private, avvisi sui certificati medici in scadenza.
- **Gare** — creazione partita, convocati scelti guardando le presenze
  della settimana, e generazione del foglio convocazione in PNG già
  pronto da mandare nel gruppo WhatsApp delle famiglie.
- **Matchday** — formato 7v7 / 8v8 / 9v9, moduli, campo interattivo,
  schieramento diverso per ciascuno dei tre tempi, gol e assist,
  minutaggio per ragazzo e segnalazione di chi non è ancora entrato.
- **Report** — frequenza per atleta, certificati da sistemare, export
  Excel a più fogli.

## Icone

Quelle in `icons/` sono segnaposto. Per sostituirle basta caricare due
PNG quadrati del logo della società, 192×192 e 512×512, con gli stessi
nomi.
