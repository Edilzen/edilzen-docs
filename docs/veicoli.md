# Veicoli

**Percorso:** Gestione Aziendale › Veicoli (`/vehicles`)

*"Veicoli — Gestisci i tuoi veicoli".* Il parco mezzi dell'azienda. Il costo dei veicoli usati nei rapportini confluisce nella voce **Veicoli** dei costi di cantiere; le scadenze dei mezzi compaiono in [Scadenze](scadenze.md).

## Cosa trovi in questa pagina

- elenco e azioni di riga;
- creazione di un veicolo (costo al km o all'ora);
- profilo: Report, Scadenze, Profilo;
- gestione delle scadenze del mezzo.

## Elenco veicoli

| Controllo | Cosa fa |
|-----------|---------|
| **Aggiungi veicolo** | Apre la finestra *Crea nuovo veicolo* |
| Intestazioni di colonna | Ordinamento |
| Clic sulla riga / **⋯ › Vedi profilo** | Apre il profilo del veicolo |
| **⋯ › Vedi scadenze** | Apre direttamente la scheda *Scadenze* del veicolo |
| **⋯ › Elimina** | Elimina il veicolo |

| Colonna | Contenuto |
|---------|-----------|
| **Nome** | Modello e produttore |
| **Targa** | |
| **Alimentazione** | |
| **Scadenze** | Riepilogo scadenze |
| **Costo** | €/km o €/h |

## Aggiungere un veicolo

### Procedura

1. Premi **Aggiungi veicolo**.
2. Compila **Informazioni generali**: Modello, Produttore (facoltativo), Targa.
3. In **Specifiche** scegli la **Base di costo** – *"Scegli se il veicolo è calcolato al chilometro o all'ora"* – con l'interruttore **Al km** / **All'ora**: compare il campo **Costo/km** (€/km) oppure **Costo/ora** (€/h).
4. (Facoltativo) scegli l'**Alimentazione**: Benzina · Diesel · Elettrico · Ibrido · GPL · Metano · Altro.
5. Premi **Crea veicolo**.

### Messaggi di validazione

| Regola | Messaggio mostrato |
|--------|--------------------|
| Modello di almeno 2 caratteri | `Model must be at least 2 characters long` |
| Targa di almeno 2 caratteri | `Vehicle plate must be at least 2 characters long` |
| Costo orario obbligatorio con base *All'ora* | `Hourly cost is required when the cost basis is hourly` |

Annullando con dati inseriti: *"Scartare il nuovo veicolo?"* → **Continua a modificare** / **Scarta**.

## Profilo del veicolo

Intestazione **Nome (TARGA)** e menu **⋯** (voce **Elimina**). Tre schede.

### Report

*"Statistiche report dal … al …"* con selettore di periodo.

- Indicatori: **Cantieri**, **Distanza**, **Costo totale**.
- Tabella: **Data**, **Cantiere**, **Distanza**, **Costo**.
- Stato vuoto: *"Nessun report — Inizia creando un nuovo report per questo veicolo."*

### Scadenze

*"Tieni traccia delle scadenze per questo veicolo."*.

**Aggiungere una scadenza**

1. Premi **Aggiungi scadenza**.
2. Compila **Nome** e **Data di scadenza**.
3. Premi **Crea scadenza**.

| Regola | Messaggio mostrato |
|--------|--------------------|
| Nome di almeno 2 caratteri | `Deadline name must be at least 2 characters long` |
| Data valida | `Deadline must be a valid ISO date (YYYY-MM-DD)` |

Tabella: **Nome**, **Scadenza**, **Stato**, **Giorni** (giorni mancanti). Le scadenze servono anche per le **notifiche di scadenza**.

Stato vuoto: *"Nessuna scadenza impostata — Aggiungi scadenze per ricevere notifiche di scadenza."*

### Profilo

| Sezione | Contenuto |
|---------|-----------|
| **Immagine del veicolo** | **Cambia foto** – immagine mostrata nel profilo e negli elenchi |
| **Informazioni generali** | Modello, Produttore, Targa |
| **Costo** – *imposta come viene calcolato il veicolo* | Base di costo Al km / All'ora, Costo |
| **Specifiche** | Alimentazione |

Premi **Salva modifiche** per confermare.

## Eliminare un veicolo

**⋯ › Elimina** nell'elenco oppure **⋯ › Elimina** nel profilo.
