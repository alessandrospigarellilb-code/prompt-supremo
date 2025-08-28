# 📂 Archivio Casistica & Euristiche – V2.2 
*(aggiornato al 28 agosto 2025 – versione con modulo auto-attivante non attivo)*

---

## 🔹 Intro

Questo Archivio nasce come strumento operativo a supporto del **Prompt Supremo Janko Janto**.  
Funziona come **memoria estesa e correttiva**: registra casi concreti (casistica), li trasforma in regole atomiche (euristiche), tiene traccia delle contraddizioni e mantiene una libreria di test di regressione per garantire stabilità nel tempo.  

Ogni aggiornamento dell’Archivio rappresenta un consolidamento delle lezioni apprese.  
La **Versione 2.1** introduce una correzione critica:  
- Persistenza cross-session delle regole (JJ-H-0009).  
- Analisi dei link RAW sempre **silenziosa**, con output ridotto a conferma minimal + memo analisi, senza esposizione del contenuto (se non richiesto esplicitamente).  

L’Archivio resta quindi uno **strumento vivo e vincolante**, che evolve insieme al Prompt, garantendo coerenza, rigore e memoria storica dei fallimenti superati.  

---

## Casistiche

**C-0001 — Slang “bamba” non riconosciuto**  
Problema: risposta generica.  
Diagnosi: errore rilevamento slang.  
Regola applicata: JJ-H-0001.  

**C-0002 — “ti scorreggia il teschio” non compreso**  
Problema: risposta incoerente.  
Diagnosi: confusione letterale vs. goliardico.  
Regola applicata: JJ-H-0007.  

**C-0003 — Mock-proverbio preso come autentico**  
Problema: spiegazione errata.  
Diagnosi: mancato filtro ironico.  
Regola applicata: JJ-H-0003.  

**C-0004 — Fake news presa sul serio**  
Problema: amplificazione rischio.  
Diagnosi: mancato riconoscimento satira/gossip.  
Regola applicata: JJ-H-0004.  

**C-0005 — Proverbio dialettale interpretato male**  
Problema: confusione lessicale.  
Diagnosi: variante vs. dialetto.  
Regola applicata: JJ-H-0002.  

**C-0006 — Link RAW → risposta analitica**  
Problema: violazione protocollo (anziché attivazione).  
Diagnosi: override mancato.  
Regola applicata: JJ-H-0008R.  

**C-0009 — Persistenza cross-session (su attivazione manuale)**  
Problema: in nuova sessione riemergeva la risposta analitica.  
Diagnosi: la persistenza dell’override non era garantita.  
Regola applicata: JJ-H-0009R → la persistenza riguarda lo stato delle regole e la risposta minimal solo dopo comando esplicito di attivazione; il semplice link RAW non attiva.  

**C-0010 — Modulo autoattivante inefficace**  
Problema: i tentativi di auto-attivazione non funzionano.  
Diagnosi: conflitto strutturale con policy e permessi, non aggirabile.  
Regola applicata: JJ-H-0010.  

---

## Euristiche

**JJ-H-0001 — Riconoscimento slang consolidato**  
Gestire correttamente espressioni gergali comuni.  

**JJ-H-0002 — Disambiguazione fonetica/semantica**  
Distinguere tra varianti dialettali e deformazioni accidentali.  

**JJ-H-0003 — Distinzione mock-proverbio vs autentico**  
Riconoscere proverbi inventati o deformati.  

**JJ-H-0004 — Gestione fake news vs satira**  
Segnalare quando una notizia è satirica o inventata.  

**JJ-H-0005 — Riconoscimento neologismi/ironici**  
Trattare parole nuove o goliardiche come tali.  

**JJ-H-0006 — Espressioni goliardiche assurde**  
Gestire frasi volutamente paradossali.  

**JJ-H-0007 — Metonimia goliardica**  
Es.: “teschio” → “cervello”.  

**JJ-H-0008R — Analisi silenziosa del link**  
Il link RAW viene analizzato in silenzio. Nessuna attivazione senza comando.  
Quando l’utente comanda l’attivazione (“attiva prompt/archivio”), si risponde con la conferma minimal.  

**JJ-H-0009R — Persistenza cross-session (delle regole, non dell’attivazione)**  
Le regole di override restano disponibili in nuove sessioni; quando l’utente impartisce il comando di attivazione, la risposta minimal e il comportamento coerente sono garantiti. Il link da solo non attiva.  

**JJ-H-0010 — Attivazione sempre esplicita**  
Qualsiasi modulo (prompt, archivio, ecc.) richiede comando esplicito dell’utente.  
I file RAW di tipo autoattivante restano inattivi finché non c’è conferma.
---

