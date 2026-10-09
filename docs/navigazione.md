# Navigazione generale

L'interfaccia di Edilzen è composta da un **menu laterale** (sidebar) a sinistra, una **barra superiore** e l'**area di lavoro** centrale. I comportamenti comuni a tutte le pagine (ricerca, ordinamento, tema, notifiche, menu utente, scorciatoie) sono descritti in [Comportamenti comuni](comportamenti-comuni.md).

## Cosa trovi in questa pagina

- la mappa completa delle voci di menu con i relativi percorsi;
- la struttura tipica di una pagina di Edilzen.

## Mappa del menu

| Gruppo | Voce | Percorso | Pagina |
|--------|------|----------|--------|
| Panoramica | Dashboard | `/dashboard` | [Dashboard](dashboard.md) |
| Gestione Cantiere | Cantieri | `/worksites` | [Cantieri](cantieri.md) |
| | Cronoprogrammi | `/chronoprograms` | [Cronoprogrammi](cronoprogrammi.md) |
| Gestione Aziendale | Dipendenti | `/employees` | [Personale](personale.md) |
| | Clienti | `/customers` | [Clienti](clienti.md) |
| | Veicoli | `/vehicles` | [Veicoli](veicoli.md) |
| | Scadenze | `/deadlines` | [Scadenze](scadenze.md) |
| | Azienda | `/company` | [Azienda](azienda.md) |
| Applicazione | Rapportini | `/reports` | [Rapportini](rapportini.md) |
| | DDT | `/ddts` | [DDT](ddt.md) |
| | SAL | `/sal` | [SAL](sal.md) |
| | Fatture | `/invoices` | [Fatture](fatture.md) |
| | Fatture in entrata | `/incoming-invoices` | [Fatture in entrata](fatture-in-entrata.md) |
| | Chiedi a Edilzen | `/ask-edilzen` | [Chiedi a Edilzen](chiedi-a-edilzen.md) |
| Impostazioni | Impostazioni Bot | `/bot` | [Bot](bot.md) |
| | Impostazioni Azienda › Team | `/settings/team` | [Team e ruoli](team.md) |
| | Impostazioni Azienda › Fatturazione | `/settings/billing` | [Fatturazione](fatturazione.md) |
| | Impostazioni Azienda › Dati legali | `/settings/legal-data` | [Dati legali](dati-legali.md) |
| | Impostazioni Azienda › Profilo Azienda | `/settings/profile` | [Profilo azienda](profilo-azienda.md) |

!!! note "Etichette"
    La voce di menu *Dipendenti* apre la pagina intitolata **Personale**; la voce *Rapportini* apre la pagina intitolata **Report**.

## Struttura tipica di una pagina

1. **Intestazione**: titolo e descrizione della sezione (es. *Cantieri – Gestisci i tuoi cantieri*).
2. **Pulsante di creazione** arancione in alto a destra: apre una finestra di dialogo (Dipendenti, Clienti, Veicoli) o una pagina `…/create` (Cantieri, Rapportini, DDT, SAL, Fatture); Rapportini e DDT offrono anche l'**Assistente AI (chat)**.
3. **Schede** (se presenti), es. *DDT / Revisiona abbinamenti*.
4. **Ricerca e filtri** sopra la tabella.
5. **Tabella** con colonne ordinabili, clic sulla riga per il dettaglio e **menu ⋯** per le azioni.
6. **Paginazione** in fondo.

Le **pagine di dettaglio** hanno un titolo con il nome dell'elemento, un menu **⋯** in alto a destra (tipicamente con *Elimina*) e delle schede; il nome della scheda compare anche nell'indirizzo (es. `/worksites/<id>/overview`).
