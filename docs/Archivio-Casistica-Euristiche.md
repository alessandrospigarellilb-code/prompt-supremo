# Archivio Casistica & Euristiche  
Data ultimo aggiornamento: 26/08/2025  
Versione: 2.0 (pulita)

---

## Introduzione

L’Archivio Casistica & Euristiche è un **documento vivo** a supporto dell’evoluzione del *Prompt Supremo Janko Janto*.  
Il suo scopo è:  
- tracciare casi reali (*casistica*),  
- derivarne regole atomiche (*euristiche*),  
- annotare contraddizioni emerse,  
- mantenere una libreria di test di regressione.  

L’archivio è stato creato in **V1.2** come prima libreria di regressione e aggiornato in **V1.3** con i moduli di attivazione.  
Questa versione **2.0 (pulita)** consolida i contenuti e uniforma lo stile, mantenendo la continuità con le versioni precedenti.  

---

## 1) Archivio Casistica

### C-0001  
**Descrizione:** termine slang “bamba” non riconosciuto.  
**Sintomo:** risposta generica, mancato riconoscimento.  
**Diagnosi:** errore di rilevamento slang.  
**Regola correttiva:** JJ-H-0001.  
**Esito:** corretto.  

### C-0002  
**Descrizione:** espressione “ti scorreggia il teschio” non compresa.  
**Sintomo:** risposta incoerente.  
**Diagnosi:** confusione tra livello letterale e goliardico.  
**Regola correttiva:** JJ-H-0007.  
**Esito:** corretto.  

### C-0003  
**Descrizione:** mock-proverbio trattato come proverbio autentico.  
**Sintomo:** spiegazione errata.  
**Diagnosi:** assenza di filtro ironico.  
**Regola correttiva:** JJ-H-0003.  
**Esito:** corretto.  

### C-0004  
**Descrizione:** fake news (es. “Gianni Morandi coprofago”) trattata come seria.  
**Sintomo:** rischio di amplificazione.  
**Diagnosi:** mancato riconoscimento satira/gossip.  
**Regola correttiva:** JJ-H-0004.  
**Esito:** corretto.  

### C-0005  
**Descrizione:** proverbio “pancia mia fatti palanca” interpretato in modo errato.  
**Sintomo:** confusione lessicale.  
**Diagnosi:** variante dialettale scambiata per deformazione.  
**Regola correttiva:** JJ-H-0002.  
**Esito:** corretto.  

### C-0006  
**Descrizione:** ricezione link RAW del Prompt o Archivio → risposta con analisi invece di conferma minimal.  
**Sintomo:** violazione della Regola 2 del Protocollo Blindato.  
**Diagnosi:** routine di analisi ha prevalso sull’override di conferma.  
**Regola correttiva:** JJ-H-0008.  
**Esito:** corretto (override applicato).  

---

## 2) Libreria di Euristiche

**JJ-H-0001 — Riconoscimento slang consolidato**  
Identificare e classificare subito slang comuni (“bamba”, ecc.).  

**JJ-H-0002 — Disambiguazione fonetica/semantica**  
Distinguere tra varianti dialettali e deformazioni.  

**JJ-H-0003 — Mock-proverb vs proverbio tradizionale**  
Separare ironia/parodia da proverbi autentici.  

**JJ-H-0004 — Gestione fake news/satira**  
Marcare voci satiriche/gossip come tali, non come fatti.  

**JJ-H-0005 — Neologismi/linguaggio ironico**  
Riconoscere invenzioni lessicali e segnalarle come creative.  

**JJ-H-0006 — Espressioni goliardiche/assurde**  
Marcare usi volutamente surreali o giocosi.  

**JJ-H-0007 — Metonimia goliardica**  
Mappare parti corporee o concetti (es. “teschio” → “cervello”).  

**JJ-H-0008 — Override conferma attivazione**  
Se un messaggio contiene **solo** un link RAW al Prompt Supremo o all’Archivio, la risposta deve essere **esclusivamente**:  
- “Prompt attivato” (per link Prompt)  
- “Archivio attivato” (per link Archivio)  
Nessuna analisi automatica.  
**Eccezioni:**  
- Se il link è accompagnato da “analizza/spiegami”, allora attivare l’analisi.  
- Se il messaggio è ambiguo, chiedere conferma all’utente.  

---

## 3) Registro Contraddizioni  

*(Vuoto — in attesa di conflitti futuri).*  

---

## 4) Libreria di Test  

**T-0001 → JJ-H-0001**: slang riconosciuto correttamente.  
**T-0002 → JJ-H-0002**: disambiguazione variante vs deformazione.  
**T-0003 → JJ-H-0003**: mock-proverb riconosciuto.  
**T-0004 → JJ-H-0004**: fake news marcata come tale.  
**T-0005 → JJ-H-0005**: neologismo segnalato.  
**T-0006 → JJ-H-0006**: espressione goliardica riconosciuta.  
**T-0007 → JJ-H-0007**: metonimia (“teschio” → “cervello”) riconosciuta.  
**T-0008 → JJ-H-0008**: link RAW produce solo conferma minimal.  
