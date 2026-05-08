# POSEIDON — Asset Management

Dashboard interna per la gestione delle dotazioni hardware aziendali.

## Stack
- HTML/CSS/JS puro — zero framework, zero build step
- [Supabase](https://supabase.com) come backend (auth + PostgreSQL)
- [SheetJS](https://sheetjs.com) per import xlsx
- Deploy su [Render](https://render.com) come sito statico

## Deploy

### Render (automatico via render.yaml)
1. Fai push di questo repo su GitHub
2. Su Render: **New → Static Site → Connect GitHub repo**
3. Render rileva `render.yaml` automaticamente
4. Clicca **Deploy** — online in ~1 minuto

### Locale
```bash
python3 -m http.server 8080
# apri http://localhost:8080
```

## Struttura
```
poseidon-app/
├── index.html      # App completa (single-file)
├── render.yaml     # Configurazione Render + CSP headers
├── .gitignore
└── README.md
```

## Accesso
Login con le credenziali create su Supabase → Authentication → Users.
La registrazione pubblica è disabilitata.
