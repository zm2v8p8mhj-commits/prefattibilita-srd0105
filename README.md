# Scheda preliminare di prefattibilità SRD01.05 — CSR Puglia 2023–2027

Web app per compilare una scheda preliminare orientativa per il bando **SRD01.05 — Investimenti produttivi agricoli per la competitività** (Regione Puglia).

Lo strumento è pensato per il primo colloquio con la ditta: raccoglie i dati dichiarati dal richiedente, produce un pre-studio firmabile per presa visione e rimanda le verifiche documentali al successivo conferimento di incarico.

## Come si usa

Apri `index.html` nel browser (oppure la versione online su GitHub Pages), carica eventualmente il fascicolo aziendale AGEA in PDF per precompilare i dati disponibili, integra o correggi manualmente le informazioni dichiarate dalla ditta e la prima ipotesi di investimento, premi **Calcola prefattibilità** e poi **Salva PDF** per scaricare il report.

Tutto il calcolo avviene nel browser: nessun dato viene inviato a server esterni. La lettura del PDF usa PDF.js caricato da CDN al momento dell'import; se non c'è connessione internet, la compilazione manuale resta sempre disponibile.

## Cosa calcola

- **Fase 1 — Requisiti minimi (killer criteria):** CR01 soggettività, CR02 dimensione economica (PS ≥ 15.000 €, deroga olivicola ≥ 5.000 €), CR27 soglia minima di spesa (30.000 €), CR28 massimale cumulativo (3.000.000 € nel periodo 2023-2027), CR31 titolo di disponibilità degli immobili.
- **Import fascicolo AGEA:** precompilazione orientativa di anagrafica, CUAA, data di nascita, sede, OTE/PS, PS olivicola, presenza di affitto/comodato e quote P3 ricavabili dai vincoli del fascicolo.
- **Fase 2 — Aliquota di sostegno:** 80% giovane agricoltore, 65% zone svantaggiate (≥ 51% SAT), 60% base.
- **Fase 3 — Punteggio di selezione** (soglia minima 30 pt): principi P1–P8 con dettaglio analitico del calcolo.
- **Fase 4 — Analisi tecnica dell'investimento:** per ogni voce di spesa (macchinari standard e 4.0, impianti arborei, opere edili, impianti irrigui, invasi, rinnovabili, filiera corta, silos/celle frigo) l'app applica le regole di validazione e determina se la voce è prioritaria ai fini del P1:
  - **Macchinari 4.0:** requisito verificato con almeno 2 caratteristiche su 6 (programmazione HW/SW, interconnessione remota, integrazione logistica, interfaccia uomo-macchina, telemanutenzione, monitoraggio di processo).
  - **Impianti arborei:** esclusione di rinfittimenti/ripristino fallanze; specie già finanziate in precedenti Avvisi SRD01 non prioritarie; valorizzazione a Costi Standard (Metodologia UCS Impianti Arborei — RRN).
  - **Opere edili:** ammissibili solo in zona agricola con destinazione produttiva; computo metrico sul Prezzario Regionale OOPP Puglia luglio 2025.
  - **Investimenti irrigui:** prioritari con efficienza ≥ 85% (≥ 80% con acque reflue); verifica autorizzazione all'emungimento e obbligo misuratori.
- **Check-list documentale (Tabella 9)** generata in base al profilo e alle voci di spesa: sempre DOC01, DOC05, DOC07, DOC11, DOC20, DOC21, DOC22; DOC02 per immobili non in proprietà con titolo idoneo; DOC03 per soggetti collettivi/società; DOC08/09/10 per edilizia; DOC12 per beni fuori prezzario; DOC13 per beni unici; DOC14 per rinnovabili; DOC19 per sostenibilità finanziaria; DOC04 per investimenti irrigui. Con avviso sull'obbligo di gestione dematerializzata dei preventivi tramite portale SIAN.

## Note metodologiche

- Il punteggio P3 (localizzazione) è calcolato in modo ponderato rispetto al valore dell'investimento ricadente in ciascuna zona, come previsto dall'Avviso SRD01.05 generalista.
- Le quote P3 importate dal fascicolo sono indicative: il fascicolo descrive particelle/vincoli, mentre il bando richiede la ponderazione sul valore dell'investimento localizzato nelle aree valorizzate.
- La qualifica di Giovane Agricoltore è acquisita come dichiarazione preliminare e va verificata con la documentazione in fase di incarico.
- Se un dato di input è assente (es. OTE per il P5), il principio è marcato "N.D." ed escluso dal calcolo.

La scheda ha valore preliminare e orientativo: non costituisce asseverazione, Domanda di Sostegno, garanzia di ammissibilità o garanzia di finanziamento. L'esito definitivo resta di competenza dell'istruttoria dell'Autorità di Gestione.

---
Dott. Agr. Ruggero Manca · ODAF Lecce n° 636 · idearurale
