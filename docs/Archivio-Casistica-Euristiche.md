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
| C-0004  | 2025-08-27 | “sbarbasucchiare”           | Termine non standard, rischio classificazione errata | Modulo 1-bis + Riconoscimento slang/neologismi | Regola JJ-H-0005: etichettare come neologismo/slang ironico, chiedere conferma prima di assumere significato | Monitoraggio | (link conversazione) |

---

## 2) Libreria di Euristiche (JJ-H-####)

> ℹ️ Nota: il numero di **euristiche (JJ-H-####)** e di **casistiche (C-####)** non è simmetrico.  
> Una singola casistica può generare più euristiche e una singola euristica può derivare da più casi.  
> Per questo la numerazione segue flussi indipendenti, anche se sempre connessi tramite descrizioni e test.

---

**JJ-H-0001 — Slang consolidato: riconoscimento immediato**  
- **Stato:** attivo (V1.2)  
- **Regola:** se termine ∈ lista slang consolidati (es. *bamba*), marcarlo subito; se ambiguità d’uso → elencare alternative e chiedere conferma solo se necessario.  
- **Motivo:** evitare mancato riconoscimento di slang diffusi.  
- **Test di regressione:** coperto da **T-0001**.  

---

**JJ-H-0002 — Anti-confusione fonetica/semantica**  
- **Stato:** attivo (V1.2)  
- **Regola:** quando due termini sono simili (fonetica o semantica), attivare mapping univoco, esplicitare alternative e segnalare rischio di errore di mapping.  
- **Motivo:** prevenire errori di interpretazione dovuti a termini simili.  
- **Test di regressione:** coperto da **T-0002**.  

---

**JJ-H-0003 — Mock-proverb vs proverbio tradizionale**  
- **Stato:** attivo (V1.2)  
- **Regola:** se struttura = rima + tabù + sentenza → presumere mock-proverb; cercare riscontri goliardici/online prima di classificarlo “tradizionale”.  
- **Motivo:** distinguere folklore autentico da invenzioni satiriche/online.  
- **Test di regressione:** coperto da **T-0003**.  

---

**JJ-H-0004 — Trattamento fake news / voci satiriche**  
- **Stato:** attivo (V1.2, retroattivo)  
- **Regola:** se un input sembra assurdo/falso → NON fermarsi; attivare comunque ricerca multidirezionale (forum, satira, social) per verificare se la voce è mai circolata.  
- **Output atteso:** risposta strutturata con:  
  - ✅ Cosa è vero (nessuna prova concreta)  
  - 🔔 Voci circolate (citazioni satiriche/blog)  
  - ⚠️ Errori cognitivi (se l’utente ricorda male)  
- **Motivo:** evitare risposte “taglio netto” che oscurano il contesto delle voci.  
- **Test di regressione:** coperto da **T-0004**.  

---

**JJ-H-0005 — Neologismi/Slang ironici**  
- **Stato:** attivo (V1.2+)  
- **Regola:** se un termine non è presente in dizionari/slang consolidati, ma ha morfologia da verbo inventato (*sbarbasucchiare*), marcarlo come:  
  - ⚠️ Neologismo / ironico  
  - Non assegnare significato certo senza conferma dell’utente.  
- **Motivo:** prevenire errori di interpretazione automatica su parole inventate.  
- **Test di regressione:** coperto da **T-0005**.  

---

## 3) Registro Contraddizioni
- (vuoto, da compilare quando emergono conflitti tra regole o interpretazioni future)

---

## 4) Libreria di Test (bozza)
- **T-0001 (slang “bamba”)** → deve essere riconosciuto subito.  
- **T-0002 (termini simili)** → attivazione mapping univoco con nota di conflitto.  
- **T-0003 (mock-proverb)** → classificazione corretta + richiesta fonti.  
- **T-0004 (fake news satirica)** → output deve includere fonti satiriche anche se bufala.  
- **T-0005 (neologismo “sbarbasucchiare”)** → input del termine deve attivare richiesta di conferma, senza assegnare significato arbitrario. Output atteso: nota “termine non standard” + domanda di chiarimento.
