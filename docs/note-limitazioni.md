# Note e limitazioni

Questa pagina elenca, in modo neutro, comportamenti da conoscere e aree non ancora complete alla data di redazione della guida.

## Aree in sviluppo

| Area | Stato |
|------|-------|
| **Impostazioni › Fatturazione** | Pagina non ancora disponibile (contenuto segnaposto) |
| **Menu utente › Impostazioni account** | Pagina non ancora disponibile (contenuto segnaposto) |
| **Fatture › passaggio 1 "I miei dati"** | Il pannello non mostra campi: i dati del mittente sono quelli inseriti in [Dati legali](dati-legali.md) |

## Azioni automatiche (senza conferma)

!!! warning "Crea costo amministrativo"
    In **Azienda › Panoramica › Fatture amministrative**, la voce di menu **Crea costo amministrativo** crea **immediatamente**, senza finestra di conferma, un costo aziendale chiamato *"&lt;Fornitore&gt; – &lt;Numero&gt;"*, **Una tantum**, con l'importo e la data della fattura, e lo collega alla fattura (la colonna *Costo collegato* si compila). Il costo creato compare in **Azienda › Costi**, dove può essere modificato o eliminato. La stessa voce è presente anche nel menu ⋯ delle fatture amministrative non collegate in **Fatture in entrata**: usala solo quando vuoi davvero registrare il costo.

- **Riesegui abbinamento** (Fatture in entrata) ricalcola subito gli abbinamenti DDT ↔ fatture: può modificare abbinamenti esistenti.
- In **Profilo azienda** non è presente un pulsante *Salva*: modifica lingua e ripartizione costi con attenzione.

## Messaggi e interfaccia

- Alcuni **messaggi di validazione** compaiono in inglese (es. *"Name must be at least 2 characters long"*). In questa guida, per ogni modulo, la regola è spiegata in italiano accanto al messaggio.
- Alcune etichette secondarie possono comparire in inglese (es. il riquadro notifiche, i titoli della scheda *Revisiona abbinamenti* dopo l'apertura).
- I pulsanti a sola icona non hanno suggerimenti al passaggio del mouse.
- Nella creazione DDT con assistente AI, sotto i formati accettati il limite di dimensione non è indicato in chiaro.
- Nella cassa previdenziale della fattura, il campo *Importo Contributo* può mostrare un valore non numerico finché i campi da cui è calcolato sono vuoti.
- Aprendo il profilo di un cliente dall'elenco la pagina può risultare vuota: ricaricarla risolve.

## Dati di esempio

Le schermate di questa guida mostrano dati di prova; nomi di persone e organizzazione sono oscurati.
