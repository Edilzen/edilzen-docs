# Scadenze

**Percorso:** Gestione Aziendale › Scadenze (`/deadlines`)

*"Riepilogo di tutte le scadenze di veicoli e fatture in entrata."* Un unico elenco per scadenze dei **veicoli**, delle **fatture** in entrata e dei **costi** aziendali.

## Cosa trovi in questa pagina

| Controllo | Cosa fa |
|-----------|---------|
| **Cerca scadenza…** | Ricerca per testo |
| Menu **Tipo** (predefinito *Tutti i tipi*) | **Tutti i tipi** · **Veicolo** · **Fattura** · **Costo** |
| Menu **Stato pagamento** | **Da pagare** · **Pagate** |
| Intestazioni di colonna | Ordinamento su Nome, Tipo, Riferimento, Scadenza, Importo, Pagata |
| Interruttore nella colonna **Pagata** | Segna la scadenza come **Pagata** o **Da pagare** |

| Colonna | Contenuto |
|---------|-----------|
| **Nome** | Descrizione della scadenza |
| **Tipo** | Veicolo, Fattura o Costo |
| **Riferimento** | Veicolo, fattura o costo di origine |
| **Scadenza** | Data |
| **Importo** | Importo dovuto |
| **Pagata** | Stato di pagamento (interruttore) |

## Procedure

### Vedere solo ciò che resta da pagare

1. Imposta **Stato pagamento = Da pagare**.
2. Eventualmente filtra per **Tipo**.
3. Ordina per **Scadenza** per vedere prima le più vicine.

### Segnare una scadenza come pagata

Nella riga, attiva l'interruttore della colonna **Pagata**: l'etichetta passa da *Da pagare* a *Pagata*. La riga comparirà filtrando per **Pagate**.

## Da dove arrivano le scadenze

| Tipo | Origine |
|------|---------|
| **Veicolo** | Scheda *Scadenze* del [profilo veicolo](veicoli.md#scadenze) |
| **Fattura** | [Fatture in entrata](fatture-in-entrata.md) |
| **Costo** | Costi con ricorrenza registrati in [Azienda › Costi](azienda.md#costi) |

## Stato vuoto

Se nessuna scadenza corrisponde ai filtri: *"Nessuna scadenza — Non ci sono scadenze che corrispondono ai filtri selezionati."*
