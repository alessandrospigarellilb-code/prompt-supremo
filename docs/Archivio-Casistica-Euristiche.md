# Archivio Casistica & Euristiche

> Documento vivo a supporto dell’evoluzione del Prompt Supremo Janko Janto.  
> Scopo: tracciare casi reali (casistica), derivarne regole atomiche (euristiche), annotare contraddizioni e test di regressione.  
> Versione iniziale: creato in V1.2 (26/08/2025)

---

## 1) Archivio Casistica

| ID Caso | Data       | Trigger / Input             | Sintomo                                             | Diagnosi (Modulo)                  | Correzione applicata                                                                 | Esito    | Riferimento |
|--------:|------------|-----------------------------|-----------------------------------------------------|------------------------------------|--------------------------------------------------------------------------------------|---------|-------------|
| C-0001  | 2025-08-25 | “bamba”                     | Non riconosciuto come slang consolidato al primo tentativo | V1.2 – Rilevamento slang consolidato | Aggiunta regola JJ-H-0001; test di riconoscimento immediato                           | Risolto | (link conversazione) |
| C-0002  | 2025-08-25 | Mock-proverb “cugina”       | Rischio confusione con proverbio tradizionale       | Modulo 1-bis + disambiguazione progressiva | Marcatura “goliardico/online” + richiesta fonti                                      | Monitoraggio | (link conversazione) |
| C-0003  | 2025-08-23 | “Gianni Morandi coprofago”  | Non riconosciuto come voce circolata; risposta troppo secca | Modulo 1-bis + ricerca multidirezionale | Regola JJ-H-0004: anche in caso di fake, cercare sempre fonti/menzioni satiriche      | Risolto | (link conversazione) |

---

## 2) Libreria di Euristiche (JJ-H-####)

**JJ-H-0001 — Slang consolidato: riconoscimento immediato**  
- **Stato:** attivo (V1.2)  
- **Regola:** se termine ∈ lista slang consolidati (es. *bamba*), marcarlo subito; se ambiguità d’uso → elencare alternative e chiedere conferma solo se necessario.  
- **Test di regressione:** input “bamba” deve passare senza warning.  

---

**JJ-H-0002 — Anti-confusione fonetica/semantica**  
- **Stato:** attivo (V1.2)  
- **Regola:** quando due termini sono simili (fonetica o semantica), attivare mapping univoco, esplicitare alternative e segnalare rischio di errore di mapping.  
- **Output atteso:** nota “potenziale conflitto” + richiesta conferma se costo dell’errore è alto.  

---

**JJ-H-0003 — Mock-proverb vs proverbio tradizionale**  
- **Stato:** attivo (V1.2)  
- **Regola:** se struttura = rima + tabù + sentenza → presumere mock-proverb; cercare riscontri goliardici/online prima di classificarlo “tradizionale”.  
- **Output atteso:** etichetta “goliardico/online” salvo fonti robuste.  

---

**JJ-H-0004 — Trattamento fake news / voci satiriche**  
- **Stato:** attivo (V1.2, retroattivo)  
- **Regola:** se un input sembra assurdo/falso → NON fermarsi; attivare comunque ricerca multidirezionale (forum, satira, social) per verificare se la voce è mai circolata.  
- **Output atteso:** risposta strutturata con:  
  - ✅ Cosa è vero (nessuna prova concreta)  
  - 🔔 Voci circolate (citazioni satiriche/blog)  
  - ⚠️ Errori cognitivi (se l’utente ricorda male)  
- **Motivo:** evitare risposte “taglio netto” che oscurano il contesto delle voci.  
- **Test di regressione:** prompt “<personaggio noto> coprofago?” → output deve riportare fonti satiriche anche se infondate.  

---

## 3) Registro Contraddizioni
- (vuoto, da compilare quando emergono conflitti tra regole o interpretazioni future)

---

## 4) Libreria di Test (bozza)
- **T-0001 (slang “bamba”)** → deve essere riconosciuto subito.  
- **T-0002 (termini simili)** → attivazione mapping univoco con nota di conflitto.  
- **T-0003 (mock-proverb)** → classificazione corretta + richiesta fonti.  
- **T-0004 (fake news satirica)** → output deve includere fonti satiriche anche se bufala.
