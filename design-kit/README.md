# Design kit

Skill di design usate per costruire siti e interfacce che non abbiano il "look da AI".
Copie fedeli dei repository originali, con le loro licenze, così sono disponibili in ogni sessione
anche senza accesso a npm.

| Cartella | Origine | Versione (commit) | Licenza | Quando usarla |
| --- | --- | --- | --- | --- |
| `taste-skill/` | [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) (tasteskill.dev) | `12af471` | MIT | Direzione artistica di un sito nuovo: composizione, tipografia, palette, sezioni. Si parte da qui. |
| `impeccable/` | [pbakaus/impeccable](https://github.com/pbakaus/impeccable) (impeccable.style) | `e89e3ad` | Apache 2.0 | Revisione e rifinitura: `critique`, `audit`, `polish`, `typeset`, `layout`, `quieter`. |
| `emil-design-eng/` | [emilkowalski/skills](https://github.com/emilkowalski/skills) | `f1090be` | MIT | Dettagli e animazioni: cosa animare, durate, easing, rifinitura dei componenti. |

## Flusso di lavoro per un sito

1. **Materiale vero.** Testi, servizi, prezzi e foto presi dal sito attuale del cliente (link fornito da Filippo). Niente immagini di repertorio né testi generici.
2. **Direzione** con `taste-skill`: si sceglie una direzione per quel cliente specifico, diversa da sito a sito.
3. **Costruzione** in HTML/CSS statico, pubblicabile su Cloudflare.
4. **Controllo visivo** con Playwright (già installato nell'ambiente): screenshot desktop e mobile, poi revisione con `impeccable` (`critique` e `audit`) e correzione.
5. **Rifinitura** di animazioni e micro-dettagli con `emil-design-eng`, con moderazione.

## Aggiornare

```bash
git clone --depth 1 https://github.com/Leonxlnx/taste-skill.git
# copiare skills/taste-skill qui, aggiornare il commit nella tabella
```

Stessa cosa per `pbakaus/impeccable` (cartella `plugin/skills/impeccable`) e `emilkowalski/skills` (cartella `skills/emil-design-eng`).
