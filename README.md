# Edilzen – Documentazione utente

Documentazione utente (in italiano) della piattaforma **app.edilzen.com**, scritta in Markdown e generata come sito statico con [MkDocs](https://www.mkdocs.org/) + [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/).

## Struttura

```
edilzen-docs/
├── mkdocs.yml          # configurazione del sito e menu di navigazione
├── requirements.txt    # dipendenze Python per la build
├── docs/
│   ├── *.md            # una pagina per sezione dell'applicazione
│   ├── img/            # screenshot (dati sensibili dell'account oscurati)
│   └── stylesheets/extra.css
└── README.md
```

## Anteprima in locale

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
mkdocs serve            # http://127.0.0.1:8000
mkdocs build --strict   # genera il sito statico in ./site
```

## Deploy su Cloudflare Pages

1. Pubblica questa cartella in un repository Git (GitHub o GitLab).
2. In Cloudflare: **Workers & Pages → Create → Pages → Connect to Git** e seleziona il repository.
3. Imposta la build così:

| Impostazione | Valore |
|--------------|--------|
| Framework preset | `None` (oppure *MkDocs*) |
| Build command | `pip install -r requirements.txt && mkdocs build` |
| Build output directory | `site` |
| Root directory | `/` (o la sottocartella che contiene `mkdocs.yml`) |
| Variabile d'ambiente | `PYTHON_VERSION` = `3.12` |

4. **Save and Deploy.** Ogni push sul branch di produzione ripubblica il sito.

### Alternativa: upload diretto (senza Git)

```bash
pip install -r requirements.txt && mkdocs build
npx wrangler pages deploy site --project-name edilzen-docs
```

## Aggiornare la documentazione

- Modifica o aggiungi file in `docs/`.
- Per nuove pagine aggiungi la voce nella sezione `nav:` di `mkdocs.yml`.
- Esegui `mkdocs build --strict` per verificare link e riferimenti prima del deploy.
