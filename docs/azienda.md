# Azienda

**Percorso:** Gestione Aziendale › Azienda (`/company`)

*"Costi aziendali, categorie di costo e fatture amministrative."* La visione economica **dell'impresa nel suo complesso**, organizzata in tre schede: **Panoramica**, **Costi**, **Ore interne**.

## Cosa trovi in questa pagina

- [Panoramica](#panoramica): indicatori aziendali, grafico e fatture amministrative con le relative azioni;
- [Costi](#costi): categorie e costi aziendali, anche ricorrenti;
- [Ore interne](#ore-interne): registrazione delle ore non di cantiere.

## Panoramica

### Indicatori

| Riquadro | Significato |
|----------|-------------|
| **Ricavi ad oggi** | Ricavi registrati finora |
| **Costi anno fiscale** | Costi dell'esercizio |
| **Costi amministrativi** | Costi di struttura |
| **Utile netto / operativo** | Risultato |

Sotto: grafico **Fatturato & netto** (come in [Dashboard](dashboard.md#fatturato-netto-anno-in-corso)).

### Fatture amministrative

Fatture fornitori di spese generali (non di cantiere). Colonne: **Fornitore**, **Numero**, **Data**, **Totale**, **Cantiere**, **Costo collegato**.

**Menu ⋯ di riga**

| Situazione | Voci disponibili |
|------------|------------------|
| Fattura **non collegata** a un costo | **Assegna a cantiere…** · **Collega a costo…** · **Crea costo amministrativo** |
| Fattura **già collegata** | **Assegna a cantiere…** · **Scollega** |

| Voce | Cosa fa |
|------|---------|
| **Assegna a cantiere…** | Apre *"Assegna a cantiere — Seleziona il cantiere a cui appartiene questa fattura amministrativa."* Scegli il cantiere dal menu (predefinito *Nessun cantiere*) e premi **Salva** (o **Annulla**) |
| **Collega a costo…** | Apre *"Collega a costo — Seleziona il costo aziendale a cui collegare questa fattura."* Scegli un costo esistente e conferma con il pulsante **Collega a costo…** (o **Annulla**) |
| **Crea costo amministrativo** | Crea subito un nuovo costo aziendale collegato alla fattura (vedi sotto) |
| **Scollega** | Rimuove il collegamento tra fattura e costo |

!!! warning "Azioni automatiche"
    **Crea costo amministrativo** non chiede conferma: crea **immediatamente** un costo aziendale chiamato *"&lt;Fornitore&gt; – &lt;Numero&gt;"*, con ricorrenza **Una tantum**, importo pari al totale della fattura e data pari alla data della fattura, e lo collega alla fattura (la colonna *Costo collegato* si compila). Il costo compare nella scheda **Costi**, dove può essere modificato o eliminato.

## Costi

*"Costi aziendali: Gestisci i costi aziendali, le ricorrenze e le categorie."* Questi sono i costi che entrano nei calcoli del cantiere quando si attiva **Includi costi aziendali**.

### Controlli

| Controllo | Cosa fa |
|-----------|---------|
| **Gestisci categorie** | Apre la finestra *Categorie di costo* |
| **Aggiungi costo** | Apre la finestra di inserimento costo |
| **⋯ › Modifica** | Modifica il costo |
| **⋯ › Elimina** | Elimina il costo |

Colonne: **Nome**, **Importo**, **Ricorrenza**, **Prossima scadenza**, **Fattura**.

### Gestire le categorie

1. Premi **Gestisci categorie**.
2. Nella finestra *Categorie di costo* cerca tra le categorie esistenti (se non ci sono risultati: *"Nessun risultato"*).
3. Premi **Nuova categoria**, compila **Nome** e **Categoria**, poi **Salva**.

### Aggiungere un costo

1. Premi **Aggiungi costo**.
2. Compila i campi:

    | Campo | Opzioni / note |
    |-------|----------------|
    | **Nome** | Descrizione del costo |
    | **Categoria** | *— Nessuna categoria* o una delle categorie create |
    | **Importo** | |
    | **Ricorrenza** | **Una tantum** · **Mensile** (predefinita) · **Trimestrale** · **Semestrale** · **Annuale** · **Personalizzata** |
    | **Data inizio** / **Data fine** | Periodo di validità |
    | **Note** | |
    | **Fattura** | *— Nessuna fattura* o una fattura amministrativa in entrata (per numero) |

3. Premi **Salva** (o **Annulla**).

I costi con ricorrenza compaiono in [Scadenze](scadenze.md) con tipo **Costo**; la colonna **Prossima scadenza** indica la prossima occorrenza.

## Ore interne

Ore lavorate dal personale **non imputate a un cantiere**.

### Registrare ore interne

Modulo in linea **Aggiungi ore**:

| Campo | Note |
|-------|------|
| **Dipendente** | Elenco di tutto il personale (cantiere, sede, liberi professionisti) |
| **Data** | Predefinita: oggi |
| **Ore** | |
| **Attività** | Descrizione dell'attività |

Premi **Registra ore**: la riga si aggiunge alla tabella **Dipendente**, **Data**, **Ore**, **Attività**. Ogni riga ha il pulsante **Elimina** per rimuoverla.
