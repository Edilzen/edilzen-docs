# Rapportini

**Percorso:** Applicazione › Rapportini (`/reports`)

*"Report — Gestisci i tuoi report giornalieri".* Il rapportino registra la giornata di lavoro in un cantiere: persone presenti con attività e ore, veicoli con km/ore, meteo, note e lavori di terzi. Le ore × [costo orario](personale.md#calcolo-del-costo-orario) generano la voce **Operai** del cantiere; i veicoli la voce **Veicoli**.

## Cosa trovi in questa pagina

- [Elenco e filtri](#elenco-rapportini);
- [Creare un rapportino](#creare-un-rapportino) con l'Assistente AI o con il modulo;
- [Dettaglio](#dettaglio-del-rapportino), [modifica](#modificare-un-rapportino), PDF ed eliminazione.

## Elenco rapportini

| Controllo | Cosa fa |
|-----------|---------|
| **Aggiungi report** | Apre la creazione (`/reports/create/bot`, modalità Assistente AI) |
| Selettore di periodo (predefinito **1m Questo mese**) | Limita l'elenco al periodo (1m, 1s, 1a, 1g, 7g, 31g, 365g, Intervallo personalizzato) |
| **Cerca report…** | Ricerca per testo |
| **Cantieri** (filtro) | Selezione multipla dei cantieri, con il numero di rapportini di ciascuno |
| Intestazioni di colonna | Ordinamento |
| Clic sulla riga | Apre il dettaglio |
| **⋯ › Modifica** | Apre la modifica |
| **⋯ › Scarica PDF** | Scarica il rapportino in PDF |
| **⋯ › Elimina** | Elimina il rapportino |

| Colonna | Contenuto |
|---------|-----------|
| **Numero** | Numero progressivo |
| **Data** | Giorno di lavoro |
| **Cantiere** | Nome e indirizzo |
| **Dipendenti** / **Liberi professionisti** / **Veicoli** | Presenti nel rapportino |
| **Fonte** | Origine (es. *web* o bot) e autore |
| **Approvazione** | Stato (es. *Approvato*) |

## Creare un rapportino

Pagina *"Compila il modulo o usa l'assistente AI per creare un nuovo report"*. In alto il selettore **Metodo di inserimento**:

- **Assistente AI (Chat) · Veloce** (`/reports/create/bot`)
- **Modulo manuale (Form)** (`/reports/create/form`)

=== "Assistente AI (Chat)"

    1. Leggi il messaggio iniziale: *"Ciao! Descrivimi il lavoro svolto (cantiere, dipendenti, ore, veicoli…) e preparo il report per te."*
    2. Scrivi nel campo *"Scrivi o pronuncia il tuo messaggio..."* – puoi anche **dettare a voce**.
    3. Premi **Invia**.
    4. L’assistente usa la descrizione per preparare il rapportino (riquadro *Prepara il tuo report*).

    !!! tip
        Indica sempre cantiere, persone (anche con il soprannome), ore, attività e mezzi usati.

=== "Modulo manuale (Form)"

    | Campo | Obbl. | Note |
    |-------|:-----:|------|
    | **Cantiere** | ✔ | Elenco ricercabile (nome + indirizzo) |
    | **Data** | | Predefinita: oggi; calendario |
    | **Meteo** | | Nessun meteo · Sereno · Nuvoloso · Pioggia · Temporale · Neve · Grandine · Nebbia · Vento |
    | **Nota** | ✔ | Descrizione della giornata |
    | **Lavori di terzi** | | Lavorazioni eseguite da terzi |

    **Dipendenti** (facoltativo) – *"Seleziona i dipendenti che hanno lavorato su questo report."*

    1. Premi **Aggiungi dipendente**: si aggiunge la riga *Dipendente - n*.
    2. Scegli il **Dipendente** (elenco dei *dipendenti cantiere*, con iniziali e soprannome), le **Ore di lavoro** e l'**Attività**.
    3. Per togliere una riga usa il cestino (*Rimuovi riga dipendente*).

    Se non ne aggiungi compare *"Nessun dipendente aggiunto"*.

    **Liberi professionisti** (facoltativo) – **Aggiungi libero professionista** → Libero professionista, Ore di lavoro, Attività.

    **Veicoli** (facoltativo) – **Aggiungi veicolo** → *Veicolo n*: Veicolo (nome / marca / targa), **Distanza** (km), **Ore di utilizzo**.

    Premi **Crea Report**.

    | Regola | Messaggio mostrato |
    |--------|--------------------|
    | Cantiere obbligatorio | `Worksite is required` |
    | Nota obbligatoria | `Note cannot be empty` |

Dalla scheda **Report** di un cantiere, **Aggiungi Report** apre la creazione con il cantiere già selezionato.

## Dettaglio del rapportino

Titolo **"Report di &lt;giorno&gt; &lt;data&gt;"**, pulsanti **Modifica** e **Scarica PDF**, due schede.

**Panoramica**

| Blocco | Contenuto |
|--------|-----------|
| Cantiere | Nome, indirizzo, pulsante **Apri cantiere** |
| **Data**, **Meteo**, **Nota** | |
| **Dipendenti** | Numero; per ciascuno: nome (soprannome), attività, ore, pulsante **Vedi profilo** |
| **Ore lavorate** | Totale |
| **Liberi professionisti** | Elenco o *"Nessun libero professionista registrato in questo report."* |
| **Veicoli** | Elenco o *"Nessun veicolo registrato in questo report."* |

**Dettagli** – *Informazioni*: **Fonte** (es. Web), **Creato da**, **Creato il**, **Aggiornato il**.

## Modificare un rapportino

1. **⋯ › Modifica** nell'elenco, oppure **Modifica** nel dettaglio (`/reports/<id>/edit`, *"Aggiorna i dettagli del report."*).
2. Modifica i campi (gli stessi del modulo manuale; la data ha la **×** *Cancella data*).
3. Premi **Aggiorna Report**.

## Scaricare il PDF

**⋯ › Scarica PDF** nell'elenco oppure **Scarica PDF** nel dettaglio.

## Eliminare un rapportino

**⋯ › Elimina** nell'elenco.

I rapportini sono consultabili anche nella scheda [Report del cantiere](cantieri.md#report), nel [profilo del dipendente](personale.md#report) e nel [profilo del veicolo](veicoli.md#report). I rapportini inviati dai [bot](bot.md) riportano la fonte bot.
