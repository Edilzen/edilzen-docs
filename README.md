# Edilzen – Documentazione utente

Documentazione utente (in italiano) della piattaforma **app.edilzen.com**, scritta in Markdown e generata come sito statico con [MkDocs](https://www.mkdocs.org/) + [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/).

- Produzione: **https://docs.edilzen.com**
- Preview Pages: **https://edilzen-docs.pages.dev**
- Repo: **https://github.com/Edilzen/edilzen-docs**

## Struttura

```
edilzen-docs/
├── mkdocs.yml          # configurazione del sito e menu di navigazione
├── requirements.txt    # dipendenze Python per la build
├── docs/
│   ├── *.md            # una pagina per sezione dell'applicazione
│   ├── img/            # screenshot (dati sensibili dell'account oscurati)
│   └── stylesheets/extra.css
├── .github/workflows/  # deploy automatico su Cloudflare Pages
└── README.md
```

## Anteprima in locale

```bash
python -m venv .venv
# Windows: .\.venv\Scripts\Activate.ps1
# macOS/Linux: source .venv/bin/activate
pip install -r requirements.txt
mkdocs serve            # http://127.0.0.1:8000
mkdocs build --strict   # genera il sito statico in ./site
```

## Deploy (GitHub → Cloudflare Pages)

Ogni push su `main` esegue `.github/workflows/deploy.yml`: build MkDocs e upload sul progetto Pages `edilzen-docs`.

### Secret GitHub richiesti

In **Settings → Secrets and variables → Actions** del repo:

| Secret | Valore |
|--------|--------|
| `CLOUDFLARE_API_TOKEN` | Token API con permesso **Cloudflare Pages — Edit** (e Account — Read) |
| `CLOUDFLARE_ACCOUNT_ID` | `3cba4a3cbdef2568cc875fe8818d94e0` |

Crea il token su: https://dash.cloudflare.com/profile/api-tokens (template *Edit Cloudflare Workers* va bene).

### Dominio `docs.edilzen.com`

Il custom domain è già collegato al progetto Pages. Nel DNS di `edilzen.com` (account Cloudflare che gestisce la zona) aggiungi:

| Type | Name | Content | Proxy |
|------|------|---------|-------|
| CNAME | `docs` | `edilzen-docs.pages.dev` | Proxied |

Dopo la propagazione, lo stato del dominio in Pages passa ad *Active* e https://docs.edilzen.com diventa raggiungibile.

### Deploy manuale locale

```bash
pip install -r requirements.txt && mkdocs build --strict
npx wrangler pages deploy site --project-name edilzen-docs
```

## Aggiornare la documentazione

- Modifica o aggiungi file in `docs/`.
- Per nuove pagine aggiungi la voce nella sezione `nav:` di `mkdocs.yml`.
- Esegui `mkdocs build --strict` per verificare link e riferimenti prima del push.
