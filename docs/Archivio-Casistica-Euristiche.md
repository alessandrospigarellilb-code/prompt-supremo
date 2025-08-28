# Archivio Casistica & Euristiche – V2.2
_Aggiornato al 28 agosto 2025_

## Finalità
Questo archivio raccoglie le casistiche emerse durante i test e le interazioni, trasformandole in regole atomiche (euristiche).  
Serve a:
- mantenere memoria operativa e correttiva,  
- evitare regressioni,  
- garantire coerenza cross-session,  
- integrare il Prompt Supremo con esempi concreti.  

## Aggiornamento
- **Versione 2.2**: chiarita la persistenza cross-session (C-0009 → JJ-H-0009R), introdotta C-0010 e la regola JJ-H-0010.  
- Deprecata la vecchia JJ-H-0008, sostituita da JJ-H-0008R.  
- Introdotta l’esplicitazione dell’attivazione manuale come unico metodo valido.  

---

## Casistiche

**C-0001 — Slang “bamba” non riconosciuto**  
- Problema: risposta generica.  
- Diagnosi: errore rilevamento slang.  
- Regola applicata: JJ-H-0001.  

**C-0002 — “ti scorreggia il teschio” non compreso**  
- Problema: risposta incoerente.  
- Diagnosi: confusione letterale vs. goliardico.  
- Regola applicata: JJ-H-0007.  

**C-0003 — Mock-proverbio preso come autentico**  
- Problema: spiegazione errata.  
- Diagnosi: mancato filtro ironico.  
- Regola applicata: JJ-H-0003.  

**C-0004 — Fake news presa sul serio**  
- Problema: amplificazione rischio.  
- Diagnosi: mancato riconoscimento satira/gossip.  
- Regola applicata: JJ-H-0004.  

**C-0005 — Proverbio dialettale interpretato male**  
- Problema: confusione lessicale.  
- Diagnosi: variante vs. dialetto.  
- Regola applicata: JJ-H-0002.  

**C-0006 — Link RAW → risposta analitica**  
- Problema: violazione protocollo (anziché attivazione).  
- Diagnosi: override mancato.  
- Regola applicata: JJ-H-0008R.  

**C-0009 — Persistenza cross-session (su attivazione manuale)**  
- Problema: in nuova sessione riemergeva la risposta analitica.  
- Diagnosi: la persistenza dell’override non era garantita.  
- Regola applicata: JJ-H-0009R → la persistenza riguarda lo stato delle regole e la risposta minimal solo dopo comando esplicito di attivazione; il semplice link RAW non attiva.  

**C-0010 — Modulo autoattivante inefficace**  
- Problema: i tentativi di auto-attivazione non funzionano.  
- Diagnosi: conflitto strutturale con policy e permessi, non aggirabile.  
- Regola applicata: JJ-H-0010.  

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

## Test di regressione

- **T-0001** — Verifica slang (JJ-H-0001).  
- **T-0002** — Disambiguare variante/deformazione (JJ-H-0002).  
- **T-0003** — Riconoscere mock-proverbio (JJ-H-0003).  
- **T-0004** — Identificare fake news (JJ-H-0004).  
- **T-0005** — Segnalare neologismi (JJ-H-0005).  
- **T-0006** — Espressione goliardica (JJ-H-0006).  
- **T-0007** — Metonimia goliardica (JJ-H-0007).  
- **T-0008** — Link RAW → conferma minimal solo dopo comando (JJ-H-0008R).  
- **T-0009** — Cross-session: garantire persistenza delle regole (JJ-H-0009R).  
- **T-0010** — Tentativo autoattivante: deve fallire e richiedere comando (JJ-H-0010).  

