# Fatture in entrata e abbinamento

**Percorso:** Applicazione › Fatture in entrata (`/incoming-invoices`)

*"Fatture in entrata — Fatture ricevute dai fornitori."* Le fatture passive vengono attribuite a un cantiere o all'intera azienda e i loro articoli vengono **abbinati** alle righe dei [DDT](ddt.md).

## Cosa trovi in questa pagina

- elenco fatture e azioni di riga;
- scheda **Abbinamento** e pulsante **Riesegui abbinamento**;
- dettaglio della fattura.

## Elenco fatture

| Controllo | Cosa fa |
|-----------|---------|
| **Riesegui abbinamento** | Rilancia l'abbinamento automatico DDT ↔ fatture (vedi sotto) |
| Schede **Fatture in entrata** / **Abbinamento** | Passano tra elenco e revisione |
| **Cerca fatture…** | Ricerca per testo |
| Intestazioni di colonna | Ordinamento |
| Clic sulla riga / **⋯ › Visualizza** | Apre il dettaglio |
| **⋯ › Crea costo amministrativo** | Presente per le fatture amministrative non collegate: crea un costo aziendale collegato (vedi [Azienda](azienda.md#fatture-amministrative)) |
| **⋯ › Elimina** | Elimina la fattura |

| Colonna | Contenuto |
|---------|-----------|
| **Numero** | Numero della fattura |
| **Fornitore** | |
| **Data** | |
| **Totale** | |
| **DDT** | Numero di DDT collegati |

## Abbinamento

*"Revisione abbinamento: Abbina le righe dei DDT agli articoli delle fatture ricevute."*

Qui compaiono i DDT i cui articoli non corrispondono completamente a quelli della fattura e che richiedono una revisione. Stato vuoto: *"Nessun DDT da revisionare — Ogni DDT è completamente abbinato o in attesa di una fattura ricevuta."*

### Riesegui abbinamento

Il pulsante **Riesegui abbinamento** ricalcola gli abbinamenti automatici tra DDT e fatture, ad esempio dopo aver caricato nuovi DDT o corretto dei dati.

!!! warning
    L'operazione parte subito e può modificare gli abbinamenti esistenti.

L'esito è visibile nei DDT: colonna **Stato** (*Abbinato*) e campo **Fattura collegata** (es. *Corrispondenza completa*).

## Dettaglio della fattura

Titolo = numero della fattura; pulsante **Elimina**. La pagina è di consultazione.

**Dettagli**

| Campo | Contenuto |
|-------|-----------|
| **Fornitore**, **P.IVA fornitore** | |
| **Numero**, **Data**, **Totale** | |
| **Cantiere** | Cantiere di imputazione ("—" se nessuno) |
| **Fonte** | Origine (es. Web) |
| **File** | File della fattura elettronica |

**Articoli** – badge *Non assegnato* con il numero di articoli non attribuiti a un cantiere. Colonne: **#**, **Codice articolo**, **Descrizione** (con unità di misura), **Quantità**, **Prezzo unitario**, **IVA**, **Cantiere** (o *Non assegnato*), **Totale**; in fondo il totale.

**DDT referenziati** – numeri dei DDT citati dalla fattura.

## Collegamenti con altre sezioni

- Fatture di spese generali → tabella *Fatture amministrative* in [Azienda › Panoramica](azienda.md#panoramica), dove si possono assegnare a un cantiere o collegare a un costo.
- Scadenze di pagamento → [Scadenze](scadenze.md) (tipo *Fattura*).
