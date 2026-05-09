# Toolmind

Landing page hub che raccoglie tutti i tool AI di Paolo. Sito statico hostato su GitHub Pages.

## Struttura

```
toolmind/
├── index.html      # unica pagina
├── style.css       # tema dark, font Inter
└── CLAUDE.md
```

## URL

`paolosem.github.io/toolmind` (dominio custom da aggiungere in futuro)

## Design

- Tema **dark** (`#0a0a0f` background)
- Accent: viola `#6c63ff`
- Font: Inter (Google Fonts)
- Layout: header sticky, hero, griglia tool, sezione about, footer
- Responsive: sotto 900px le card diventano single column

## Tool presenti

| Tool | Bot | Landing | Stato |
|------|-----|---------|-------|
| Vocale2Testo | `@davocaleatesto_bot` | `vocale2testo.it` | Live |
| Doc2Testo | `@doc2testo_bot` | — | Live |

## Come aggiungere un nuovo tool

1. Copia un blocco `<article class="tool-card">` in `index.html`
2. Aggiorna icona, nome, descrizione, feature list e link
3. Cambia il contatore `stat-number` nella sezione about (attualmente "2")
4. Commit e push su `master` → GitHub Pages si aggiorna in automatico

## Contatto "Suggerisci un tool"

Il bottone nella card "coming soon" punta a `https://t.me/Paolo_Sem`.

## Deploy

GitHub Pages su branch `master`, root `/`. Nessuna build step — file statici serviti direttamente.
