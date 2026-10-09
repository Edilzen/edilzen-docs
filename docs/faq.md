# FAQ e flussi tipici

## Flussi tipici

### Configurare l'azienda (primo avvio)

1. **Dati legali** – completa anagrafica, regime fiscale, sede legale e REA ([Dati legali](dati-legali.md)).
2. **Profilo azienda** – scegli la **lingua** e il criterio di **ripartizione dei costi aziendali** ([Profilo azienda](profilo-azienda.md)).
3. **Personale** – inserisci dipendenti (RAL, ore, INAIL…) e liberi professionisti (tariffa oraria), con il **soprannome** usato in cantiere ([Personale](personale.md)).
4. **Veicoli** – inserisci i mezzi con base di costo al km o all'ora ([Veicoli](veicoli.md)).
5. **Costi aziendali** – registra i costi ricorrenti in [Azienda › Costi](azienda.md#costi).
6. **Team e bot** – invita i collaboratori e crea i bot Telegram/WhatsApp ([Team](team.md), [Bot](bot.md)).

### Aprire un nuovo cantiere

1. Verifica che il committente sia in [Clienti](clienti.md) (altrimenti **Aggiungi cliente**).
2. **Cantieri › Nuovo Cantiere**: nome, indirizzo, cliente, **valore contratto**, **margine target**, eventuali **CIG/CUP**, date → **Crea Cantiere**.
3. Nel **Profilo** del cantiere inserisci **Latitudine/Longitudine** per mappa e meteo.
4. Nella scheda **Cronoprogramma** usa **Template › Template dal catalogo** per generare le lavorazioni, poi adatta date, durate e dipendenze.

### Pianificare il cronoprogramma

1. Imposta la data di **Inizio**.
2. Crea **Categorie** e **Attività** (o parti dal **Template**), con inizio, durata (gg) ed eventuale importo (€).
3. Collega le attività trascinando la maniglia di una barra sulla lavorazione successiva (dipendenza **FS**).
4. Usa **Strumenti** (Squadre, Rese e quantità, Attese, Adatta la timeline, Vai a oggi) e la scala **Giorno / Settimana / Mese**.
5. Verifica **Salvato**; se serve, **Esporta** in JSON, PNG, SVG o PDF (o **Apri** un file `.json`).

### Registrare la giornata in cantiere

- **Dal bot**: il capocantiere scrive o manda un vocale al bot Telegram/WhatsApp; il rapportino compare in **Rapportini** con *Fonte: bot* (approvato in automatico se l'opzione del bot è attiva).
- **Dal web**: **Rapportini › Aggiungi report** → *Assistente AI (Chat)* descrivendo la giornata, oppure *Modulo manuale* (cantiere, data, meteo, nota, dipendenti con ore, liberi professionisti, veicoli) → **Crea Report**.

### Gestire DDT e fatture dei fornitori

1. **DDT › Aggiungi DDT** → carica la foto o il PDF (assistente AI) oppure compila il modulo; indica il cantiere.
2. Quando arriva la fattura del fornitore in [Fatture in entrata](fatture-in-entrata.md), controlla la scheda **Abbinamento** (usa **Riesegui abbinamento** se necessario).
3. Verifica in **DDT › Revisiona abbinamenti** i DDT da controllare e, in Dashboard, i **DDT da revisionare** per anomalie di prezzo.
4. Controlla che i DDT risultino **Abbinato** e **Approvato**.

### Registrare un SAL e fatturarlo

1. **SAL › Nuovo SAL**: scegli il cantiere e il metodo **Dal cronoprogramma** (indica la data: la percentuale è calcolata dal Gantt) oppure **Manuale** (digiti la percentuale) → **Crea**.
2. **Fatture › nuova fattura**: compila gli 8 passaggi; al passaggio 4 usa **Aggiungi fase** per collegare il SAL ed eventuali **CIG/CUP**.
3. Controlla il **Totale fattura** e premi **Verifica e procedi**.

### Generare i cedolini

1. **Dipendenti › ⋯ › Vedi profilo › Cedolini**.
2. Scegli **Anno** e **Mese** → **Genera cedolino**; nella tabella trovi lordo, netto e costo azienda.

### Tenere sotto controllo costi e rischio

1. In **Dashboard** controlla *A rischio*, *Risk score* (fattori), *Quadrante CPI×SPI*, *Burn rate* e *Mappa cantieri*.
2. Apri il cantiere: in **Panoramica** analizza *Costo finora*, *Margine reale*, CPI, VAC e la tabella **Risultati** (per categoria, articolo, data o documento).
3. Attiva **Includi costi aziendali** per il risultato comprensivo dei costi generali.

### Dare accesso al commercialista

**Team › Invita membro** → email, livello **Commercialista esterno** → **Invia invito**. Vedrà solo fatture, DDT, clienti e altri documenti contabili.

## Domande frequenti

??? question "Cosa significa un CPI sotto 1?"
    Significa che i costi sostenuti superano il valore del lavoro eseguito: il cantiere sta spendendo più di quanto "guadagna" con l'avanzamento. Vedi [Glossario](glossario.md).

??? question "Perché il margine cambia attivando «Includi costi aziendali»?"
    Perché ai costi diretti del cantiere viene aggiunta la quota di costi generali dell'impresa (sezione [Azienda](azienda.md)). Il *ROI (con costi aziendali)* è quindi normalmente più basso del *ROI (solo cantiere)*.

??? question "Che differenza c'è tra «Fatture» e «Fatturazione»?"
    **Fatture** (menu *Applicazione*) serve a emettere fatture verso i tuoi clienti. **Fatturazione** (menu *Impostazioni Azienda*) riguarda la fatturazione del servizio Edilzen ed è attualmente **in sviluppo**.

??? question "Un cantiere non compare tra i cronoprogrammi «Presente». Perché?"
    Il cantiere non ha ancora un cronoprogramma: lo stato è *Da creare*. Apri il cantiere e crea la pianificazione nella scheda **Cronoprogramma**.

??? question "Chi può modificare i dati legali dell'azienda?"
    I **Titolari**, che hanno il controllo completo dell'organizzazione inclusi fatturazione e dati legali.

??? question "Un account bot può accedere all'applicazione web?"
    No. Gli account bot operano solo tramite il dipendente collegato e non possono accedere come le persone. Vedi [Bot](bot.md).

??? question "Che codice SDI uso per un cliente privato?"
    Il codice `0000000`. In alternativa la fattura può essere recapitata tramite PEC, se indicata.

??? question "Come faccio a far riconoscere un operaio dal bot?"
    Compila il campo **Soprannome per Bot & Rapportini** nella sua scheda: l'AI Matcher lo usa per riconoscerlo nei messaggi e nei vocali.

??? question "Posso inserire la percentuale di un SAL a mano?"
    Sì: nella creazione del SAL scegli il metodo **Manuale** e digita la percentuale. Con il metodo **Dal cronoprogramma** la percentuale è invece calcolata dalla data scelta sul Gantt.

??? question "«Crea costo amministrativo» chiede conferma?"
    No: in **Azienda › Panoramica › Fatture amministrative** la voce crea subito un costo *Una tantum* collegato alla fattura. Se lo crei per errore, eliminalo da **Azienda › Costi**. Vedi [Note e limitazioni](note-limitazioni.md).

??? question "Come comprimo il menu laterale?"
    Con il pulsante in alto a sinistra della barra superiore oppure con **Ctrl+B**. Vedi [Comportamenti comuni](comportamenti-comuni.md).

??? question "Come esporto un cronoprogramma?"
    Nella scheda **Cronoprogramma** del cantiere: **Esporta ▾** → JSON, PNG, SVG o PDF. Il file JSON può essere reimportato con **Apri**.

??? question "Quali tipi di documento posso emettere?"
    Tutti i codici da **TD01** a **TD29** previsti dalla fattura elettronica (elenco completo in [Fatture › Tipo documento](fatture.md#tipo-documento-td)).

??? question "Come segno pagata una scadenza?"
    In [Scadenze](scadenze.md), con la colonna **Pagata**. Usa i filtri *Da pagare / Pagate* per controllare la situazione.

??? question "Quanto possono pesare gli allegati di una fattura?"
    Fino a **3,5 MB**.

??? question "Come cambio la partita IVA dell'azienda?"
    In [Dati legali](dati-legali.md) P.IVA e codice fiscale non sono modificabili direttamente: usa **Richiedi modifica**.

??? question "Posso usare il tema scuro?"
    Sì: usa il pulsante **Cambia tema** nella barra superiore.
