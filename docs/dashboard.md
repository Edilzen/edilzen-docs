# Dashboard

**Percorso:** Panoramica › Dashboard (`/dashboard`)

La Dashboard è la pagina iniziale: *"La tua azienda a colpo d'occhio"*. Riassume lo stato economico, di avanzamento e di rischio di tutti i cantieri attivi. In alto è riportato il nome dell'azienda; sotto si trovano i riquadri (widget) descritti di seguito. Ogni riquadro ha in alto a destra un codice identificativo (es. *W01 · KPI-STRIP*, *W04 · PL-FORECAST*, *W10 · TABELLA-CANTIERI*, *W41 · BURN-RATE*), utile come riferimento.

## Cosa trovi in questa pagina

| Riquadro | Domanda a cui risponde |
|----------|------------------------|
| Comando portfolio | Come vanno complessivamente costi, tempi e margini? Quanti cantieri sono a rischio? |
| Fatturato & netto | Quanto ho fatturato e guadagnato da inizio anno, e dove arriverò a fine anno? |
| Cantieri attivi | Qual è la situazione di ciascun cantiere? |
| Burn rate portfolio | Sto spendendo come previsto? |
| Risk score | Perché un cantiere è a rischio? |
| Quadrante CPI × SPI | Quali cantieri sono in ritardo e/o fuori budget? |
| Meteo Cantieri | Il meteo ostacolerà i lavori? |
| Cost-to-complete & VAC | Quanto manca da spendere e con quale margine finale? |
| DDT da revisionare | Ci sono prezzi anomali nei DDT? |
| Mappa cantieri | Dove sono i cantieri e quanto sono a rischio? |

Nella Dashboard non si inseriscono dati: gli indicatori sono calcolati da Edilzen a partire dalle informazioni registrate nelle altre sezioni (cantieri, rapportini, DDT, fatture, SAL, cronoprogrammi).

![Dashboard](img/01_dashboard.png){ .screenshot }

## Comando portfolio

*Indici EVM aggregati sui cantieri attivi – aggiornato oggi.*

| Indicatore | Formula / significato mostrato | Come leggerlo |
|------------|-------------------------------|---------------|
| **CPI medio** | EV / AC | Sotto 1 = i costi sostenuti superano il valore guadagnato |
| **SPI medio** | SAL vs tempo lavorativo di piano | Sotto 1 = avanzamento in ritardo rispetto al piano |
| **VAC portfolio** | Valore contratto − EAC | Margine atteso a chiusura sull'insieme dei cantieri |
| **A rischio** | N° cantieri a rischio / N° cantieri attivi | Cantieri con *risk score ≥ 60*, da seguire nella settimana |

Per le definizioni vedi il [Glossario](glossario.md).

## Fatturato & netto (anno in corso)

Grafico *cumulato da fatture e ledger*:

| Elemento | Significato |
|----------|-------------|
| **FATTURATO** (linea blu) | Fatturato cumulato da inizio anno |
| **NETTO** (linea scura) | Risultato netto cumulato |
| Parte **tratteggiata** | Previsione *run‑rate* fino a fine anno |
| **YTD** | Valore da inizio anno a oggi |
| **NET FY** / **FY atteso** | Netto previsto a fine esercizio |

Lo stesso grafico compare in [Azienda › Panoramica](azienda.md#panoramica).

## Cantieri attivi

Tabella dei cantieri attivi con i principali indicatori per ciascuno:

| Colonna | Contenuto |
|---------|-----------|
| **Cantiere** | Nome del cantiere |
| **Cliente** | Committente |
| **SAL** | Percentuale di avanzamento |
| **CPI** / **SPI** | Indici di costo e di tempo |
| **VAC** | Margine atteso a chiusura |
| **Ritardo** | *in linea* oppure ritardo stimato nel formato *+N gg · X k€* (giorni di ritardo e relativo impatto economico) |
| **Risk** | Risk score con etichetta di fascia (es. *ALTO*, *BASSO*) |

La colonna **SAL** è rappresentata con una barra di avanzamento.

Cliccando su una riga si apre la [scheda del cantiere](cantieri.md#scheda-di-dettaglio-del-cantiere).

## Burn rate portfolio

Confronta la **spesa effettiva** con quella **pianificata**.

| Controllo / elemento | Cosa fa |
|----------------------|---------|
| **7G / 14G / 30G** | Cambia la finestra temporale (ultimi 7, 14 o 30 giorni) |
| Serie **COSTI EFFETTIVI** | Spesa realmente sostenuta |
| Serie **PIANO** | Spesa prevista dal piano |
| Banda **μ ± 2σ** | Fascia di normalità (media ± due deviazioni standard) |
| Pulsanti per cantiere (es. *Nome cantiere · CPI … · SPI …*) | Mostrano il burn rate del solo cantiere scelto |
| **tutti** | Torna alla vista dell'intero portafoglio |
| **+ / −** | Zoom avanti / indietro sul grafico |

Una spesa che esce dalla banda segnala un'accelerazione o un rallentamento anomalo dei costi.

## Risk score

Spiega il punteggio di rischio attraverso **6 fattori esplicabili** (ad esempio **COSTI**, **TEMPI**, **DATI**), così da capire *perché* un cantiere è considerato a rischio e su quale aspetto intervenire.

## Quadrante CPI × SPI

Grafico a quattro quadranti che posiziona ogni cantiere in base a **CPI** (costi) e **SPI** (tempi): permette di distinguere a colpo d'occhio i cantieri in regola, quelli in ritardo, quelli fuori budget e quelli critici su entrambi i fronti.

## Meteo Cantieri

Previsioni meteo a **4 giorni** per i cantieri e conteggio dei **giorni a rischio meteo nei prossimi 14 giorni**, utile per riorganizzare le lavorazioni all'aperto.

## Cost-to-complete & VAC

Per ogni cantiere (vista **tutti**) mostra il **costo stimato per completare** i lavori e il **VAC** (margine atteso a chiusura).

## DDT da revisionare

Elenca i DDT con **anomalie di prezzo**, individuate statisticamente quando il prezzo di una riga si discosta dalla norma con uno **z‑score ≥ 2,5**. Da qui si individuano i documenti da controllare nella sezione [DDT](ddt.md).

## Mappa cantieri

Mappa geografica dei cantieri, colorati in base al risk score:

| Colore / fascia | Risk score |
|-----------------|-----------|
| Rischio alto | ≥ 60 |
| Rischio medio | 35 – 59 |
| Rischio basso | < 35 |

La posizione dei cantieri deriva dalle coordinate (Latitudine/Longitudine) presenti nel [Profilo del cantiere](cantieri.md#profilo).

!!! tip "Uso consigliato"
    A inizio settimana controlla **A rischio** e la **Mappa**, apri il **Risk score** per capire quale fattore pesa di più, poi verifica **Meteo Cantieri** e **DDT da revisionare**.
