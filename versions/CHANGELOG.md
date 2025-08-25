# Changelog – Prompt Supremo Janko Janto

## V1.1 – 2025-08-25
Stato: stable · Data: 25/08/2025  
Contenuto: import del Prompt Supremo Janko Janto – V1.1, copia fedele dalla chat.  
Delta: prima release nel repo, nessuna differenza da versioni precedenti.  
Scopo: fissare base ufficiale per il versioning, in vista di V1.2 e successive.  

## [1.2] – 26/08/2025
### Added
- **Modulo 1-bis (Errori/Ambiguità avanzato):** gestione nomi, luoghi, date, refusi, termini inventati o tecnici di nicchia, con generazione ipotesi alternative e ranking di plausibilità.
- **Regola JJ-H-0001:** riconoscimento immediato slang consolidati (es. *bamba*).
- **Regola JJ-H-0002:** anti-confusione fonetica/semantica con mapping univoco e nota esplicita di rischio.
- **Regola JJ-H-0003:** distinzione mock-proverb vs proverbi tradizionali, con ricerca in fonti goliardiche/online.
- **Regola JJ-H-0004:** trattamento fake news/voci satiriche → ricerca multidirezionale obbligatoria anche per bufale evidenti.
- **Regola JJ-H-0005:** gestione neologismi/slang ironici → marcare come non standard e chiedere conferma all’utente.
- **Libreria di Test (bozza):** T-0001 fino a T-0005.
- **Archivio Casistica & Euristiche:** introdotto come documento esterno RAW collegato al Prompt.

### Changed
- Maggiore enfasi su voci e falsi ricordi, con suddivisione in:  
  - 🔔a Fake news diffuse  
  - 🔔b Malintesi/falsi ricordi  
  - 🔔c Provocazioni/meme  
- Output strutturato reso obbligatorio in ogni risposta, con liste ✅/❓/🔔/⚠️/📚 e sezione metodo.

### Fixed
- Corretto errore di mancato riconoscimento slang “bamba” (ora coperto da JJ-H-0001).
