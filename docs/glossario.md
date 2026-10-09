# Glossario

## Indicatori EVM

L'**Earned Value Management (EVM)** confronta ciò che è stato pianificato, ciò che è stato realizzato e ciò che è stato speso. Edilzen mostra questi indicatori nella [Dashboard](dashboard.md) (valori aggregati) e nella [Panoramica del cantiere](cantieri.md#panoramica).

AC – Actual Cost
:   Costo effettivo sostenuto finora (in Edilzen: *Costo finora*, somma di operai, veicoli e materiali).

EV – Earned Value
:   Valore del lavoro effettivamente eseguito, cioè quanto "vale" l'avanzamento raggiunto rispetto al contratto.

EAC – Estimate At Completion
:   Stima del costo totale a fine lavori, proiettata sull'andamento attuale.

CPI – Cost Performance Index
:   **CPI = EV / AC.** Indica l'efficienza dei costi. **Sotto 1** i costi sostenuti superano il valore guadagnato (si sta spendendo più del previsto); sopra 1 si sta spendendo meno del valore prodotto.

SPI – Schedule Performance Index
:   Indice di rispetto dei tempi: in Edilzen confronta il **SAL** con il **tempo lavorativo di piano**. **Sotto 1** il cantiere è in ritardo; sopra 1 è in anticipo.

VAC – Variance At Completion
:   **VAC = Valore contratto − EAC.** È il **margine atteso a chiusura**: positivo = guadagno previsto, negativo = perdita prevista.

Risk score
:   Punteggio di rischio del cantiere calcolato da Edilzen e spiegato da **6 fattori** (es. COSTI, TEMPI, DATI). Fasce: **≥ 60** alto (cantiere *a rischio*, da seguire nella settimana), **35–59** medio, **< 35** basso. Vedi [Dashboard](dashboard.md#risk-score).

## Indicatori economici del cantiere

Valore contratto
:   Importo contrattuale pattuito con il cliente.

Margine teorico
:   Margine previsto sul contratto (in euro e percentuale).

Margine reale
:   Margine calcolato sui costi effettivamente sostenuti.

ROI (solo cantiere) / ROI (con costi aziendali)
:   Ritorno sull'investimento calcolato rispettivamente sui soli costi diretti del cantiere o includendo la quota di costi aziendali.

Costi aziendali
:   Costi generali dell'impresa non legati a un singolo cantiere; si possono includere nei calcoli con l'interruttore *Includi costi aziendali*.

Burn rate
:   Velocità con cui si consumano i costi nel tempo. Nella Dashboard è confrontata con quella pianificata, con una banda di **±2σ**.

σ (sigma) / z-score
:   σ è la deviazione standard. Lo **z‑score** misura di quante deviazioni standard un valore si discosta dalla media: Edilzen segnala come anomali i prezzi dei DDT con z‑score ≥ 2,5.

Cost-to-complete
:   Costo stimato ancora necessario per completare il cantiere.

Quadrante CPI × SPI
:   Grafico che classifica i cantieri combinando efficienza dei costi (CPI) e rispetto dei tempi (SPI).

Run-rate
:   Proiezione a fine anno basata sul ritmo attuale; nel grafico *Fatturato & netto* è la parte tratteggiata.

YTD / FY
:   *Year To Date* (da inizio anno a oggi) / *Fiscal Year* (intero esercizio).

## Documenti e pianificazione

SAL – Stato di Avanzamento Lavori
:   Percentuale di lavoro eseguito sul totale previsto. Vedi [SAL](sal.md).

DDT – Documento di Trasporto
:   Documento che accompagna la merce consegnata dal fornitore. Vedi [DDT](ddt.md).

Abbinamento
:   Collegamento tra un DDT e la fattura del fornitore corrispondente. Vedi [Fatture in entrata](fatture-in-entrata.md#abbinamento).

Rapportino
:   Resoconto dell'attività e delle ore lavorate in cantiere. Vedi [Rapportini](rapportini.md).

Affidabilità (DDT)
:   Livello di affidabilità dei dati estratti automaticamente da un DDT (es. *Media*).

AI Matcher
:   Funzione che riconosce le persone citate nei messaggi e nelle trascrizioni vocali dei bot, usando il *Soprannome per Bot & Rapportini*.

Template dal catalogo
:   Modello di cronoprogramma costruito scegliendo categorie di lavorazione con attività e durate predefinite.

Cronoprogramma / Gantt
:   Pianificazione temporale delle lavorazioni rappresentata con barre su un calendario. Vedi [Cantieri › Cronoprogramma](cantieri.md#cronoprogramma-gantt).

Categoria / Attività
:   Nel cronoprogramma, la categoria è una macro‑fase che raggruppa più attività (lavorazioni).

Dipendenza FS (Finish‑to‑Start)
:   Vincolo per cui un'attività può iniziare solo quando la precedente è terminata.

PERT
:   *Program Evaluation and Review Technique.* Stima della durata con tre valori: **o** = ottimistica, **m** = più probabile, **p** = pessimistica (in giorni). Edilzen la mostra per ogni attività e categoria come *PERT o/m/p*.

## Personale e costi

RAL
:   Retribuzione Annua Lorda del dipendente.

INPS datore
:   Contributi previdenziali a carico del datore di lavoro.

INAIL
:   Premio assicurativo contro gli infortuni sul lavoro, espresso come aliquota percentuale.

TFR
:   Trattamento di Fine Rapporto, accantonato ogni anno dal datore di lavoro.

Costo orario reale di cantiere
:   RAL × (1 + INPS datore + INAIL + TFR) ÷ ore lavorabili annue. Vedi [Personale](personale.md#calcolo-del-costo-orario).

Oneri datoriali ripartiti
:   Opzione che distribuisce i contributi a carico del datore sui cantieri in base alle ore lavorate.

Rivalsa INPS
:   Maggiorazione (4%) che alcuni liberi professionisti iscritti alla Gestione separata addebitano in fattura.

Cedolino
:   Busta paga mensile: riporta lordo, netto e costo azienda.

Ore interne
:   Ore lavorate non imputate a un cantiere. Vedi [Azienda](azienda.md#ore-interne).

## Fatturazione elettronica

CIG / CUP
:   *Codice Identificativo Gara* e *Codice Unico di Progetto*: codici obbligatori nei contratti e nelle fatture verso la Pubblica Amministrazione.

Split Payment
:   Scissione dei pagamenti: l'IVA viene versata direttamente all'Erario dal cliente (tipicamente la PA) anziché al fornitore.

REA
:   Repertorio Economico Amministrativo, il numero di iscrizione presso la Camera di Commercio.

EORI
:   Codice identificativo per le operazioni doganali nell'Unione europea.

Regime fiscale
:   Regime IVA/fiscale del soggetto (es. ordinario, forfettario), richiesto nella fattura elettronica.

Stabile organizzazione / Rappresentante fiscale
:   Sede fissa in Italia, o soggetto residente incaricato, di un'impresa non residente.

SDI – Sistema di Interscambio
:   Piattaforma dell'Agenzia delle Entrate che recapita le fatture elettroniche.

Codice destinatario (Codice SDI)
:   Codice che identifica il canale di ricezione del cliente: 7 caratteri per i privati/aziende (`0000000` se non disponibile), 6 caratteri (codice univoco ufficio) per la Pubblica Amministrazione.

PEC
:   Posta Elettronica Certificata, canale alternativo di recapito della fattura.

Ritenuta
:   Importo trattenuto alla fonte dal committente e versato all'Erario per conto del fornitore.

Bollo
:   Imposta di bollo dovuta su alcune fatture (es. operazioni esenti IVA oltre una certa soglia).

Cassa
:   Contributo alla cassa previdenziale di categoria, per alcune professioni.

Fattura in entrata (passiva)
:   Fattura ricevuta da un fornitore.

## Ruoli

Titolare
:   Controllo completo dell'organizzazione, inclusi fatturazione e dati legali.

Accesso completo
:   Utente (amministratore o membro) che usa tutta la piattaforma secondo il proprio livello.

Account bot
:   Account Telegram/WhatsApp che opera solo tramite un dipendente collegato.

Commercialista esterno
:   Accesso limitato a fatture, DDT, clienti e altri documenti contabili.
