# SAL – Stati di avanzamento lavori

**Percorso:** Applicazione › SAL (`/sal`)

*"SAL — Gestisci i documenti di Stato Avanzamento Lavori (SAL)".* Il SAL indica la percentuale di lavoro eseguito su un cantiere, ricavata dal cronoprogramma oppure inserita a mano.

## Cosa trovi in questa pagina

- elenco SAL;
- creazione con metodo *Dal cronoprogramma* o *Manuale*;
- dettaglio e modifica.

## Elenco SAL

| Controllo | Cosa fa |
|-----------|---------|
| **Nuovo SAL** | Apre la creazione (`/sal/create`) |
| **Cerca per data…** | Ricerca per data |
| Intestazioni **Cantiere**, **Data**, **Percentuale** | Ordinamento |
| Clic sulla riga | Apre il dettaglio |
| Paginazione | *N voci*, Previous / pagine / Next |

In questa tabella non c'è il menu ⋯ di riga.

## Creare un SAL

Pagina *"Aggiungi un SAL: scegli un punto sul cronoprogramma oppure inserisci la percentuale manualmente"*.

1. Premi **Nuovo SAL** (oppure **Nuovo SAL** nella scheda SAL del cantiere, che preimposta il cantiere).
2. Scegli il **Cantiere** (*Scegli un cantiere…*).
3. Compare il selettore **Metodo**:
    - **Dal cronoprogramma** – imposta la **Data sul cronoprogramma** (predefinita: oggi). *"La percentuale è calcolata dalla posizione di questa data sulla timeline del cronoprogramma."* Il campo **Percentuale di avanzamento** mostra il valore *derivato automaticamente*;
    - **Manuale** – digita direttamente la **Percentuale di avanzamento**.
4. (Facoltativo) scrivi le **Note**.
5. Premi **Crea**.

Il pulsante **Crea** resta disattivato finché il modulo non è completo e valido.

## Dettaglio del SAL

Titolo **"SAL del gg/mm/aaaa"**, con *Creato il* / *Aggiornato il* e pulsante **Modifica**. Scheda **Panoramica**:

| Elemento | Contenuto |
|----------|-----------|
| **Cantiere** | Nome, indirizzo, link **Vedi profilo** |
| **Data** | |
| **Percentuale** | |
| **Note** | |

Per modificarlo premi **Modifica**.

## Dove si usa il SAL

- scheda **SAL** del [cantiere](cantieri.md#sal) e collegamento **SAL xx%** nel Gantt;
- indicatore **SPI** e colonna **SAL** dei *Cantieri attivi* nella [Dashboard](dashboard.md);
- nella [fattura](fatture.md#4-cantieri-e-riferimenti), sezione SAL con **Aggiungi fase**.

!!! tip
    Con il metodo *Dal cronoprogramma* il SAL è coerente con la pianificazione: tieni aggiornato il cronoprogramma.
