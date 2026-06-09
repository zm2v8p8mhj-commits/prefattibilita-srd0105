# Prefattibilità SRD01.05 — CSR Puglia 2023–2027

Web app di studio di prefattibilità per il bando **SRD01.05 — Investimenti produttivi agricoli per la competitività** (Regione Puglia).

## Come si usa

Apri `index.html` nel browser (oppure la versione online su GitHub Pages), compila il form con i dati del fascicolo aziendale e del preventivo di progetto, premi **Calcola prefattibilità** e poi **Salva PDF** per scaricare il report.

Tutto il calcolo avviene nel browser: nessun dato viene inviato a server esterni.

## Cosa calcola

- **Fase 1 — Requisiti minimi (killer criteria):** CR01 soggettività, CR02 dimensione economica (PS ≥ 15.000 €, deroga olivicola ≥ 5.000 €), CR27 soglia minima di spesa (30.000 €), CR28 massimale cumulativo (3.000.000 € nel periodo 2023-2027).
- **Fase 2 — Aliquota di sostegno:** 80% giovane agricoltore, 65% zone svantaggiate (≥ 51% SAT), 60% base.
- **Fase 3 — Punteggio di selezione** (soglia minima 30 pt): principi P1–P8 con dettaglio analitico del calcolo.
- **Fase 4 — Analisi tecnica dell'investimento:** per ogni voce di spesa (macchinari standard e 4.0, impianti arborei, opere edili, impianti irrigui, invasi, rinnovabili, filiera corta, silos/celle frigo) l'app applica le regole di validazione e determina se la voce è prioritaria ai fini del P1:
  - **Macchinari 4.0:** requisito verificato con almeno 2 caratteristiche su 6 (programmazione HW/SW, interconnessione remota, integrazione logistica, interfaccia uomo-macchina, telemanutenzione, monitoraggio di processo).
  - **Impianti arborei:** esclusione di rinfittimenti/ripristino fallanze; specie già finanziate in precedenti Avvisi SRD01 non prioritarie; valorizzazione a Costi Standard (Metodologia UCS Impianti Arborei — RRN).
  - **Opere edili:** ammissibili solo in zona agricola con destinazione produttiva; computo metrico sul Prezzario Regionale OOPP Puglia luglio 2025.
  - **Investimenti irrigui:** prioritari con efficienza ≥ 85% (≥ 80% con acque reflue); verifica autorizzazione all'emungimento e obbligo misuratori.
- **Check-list documentale (Tabella 9)** generata in base al profilo e alle voci di spesa: sempre DOC01, DOC05, DOC07, DOC11, DOC20, DOC22; DOC02 per immobili in affitto; DOC08/09/10 per edilizia; DOC12 (3 preventivi SIAN) per beni fuori prezzario; DOC13 per beni unici; DOC14 per rinnovabili; DOC04 per investimenti irrigui. Con avviso sull'obbligo di gestione dematerializzata dei preventivi tramite portale SIAN.

## Note metodologiche

- Il punteggio P3 (localizzazione) è attribuito con criterio di prevalenza: quota ≥ 50% dell'investimento/SAT nella zona.
- La qualifica di Giovane Agricoltore è calcolata automaticamente: 41 anni non compiuti alla data DdS e primo insediamento da meno di 5 anni.
- Se un dato di input è assente (es. OTE per il P5), il principio è marcato "N.D." ed escluso dal calcolo.

Lo studio ha valore indicativo: l'esito definitivo resta di competenza dell'istruttoria dell'Autorità di Gestione.

---
Dott. Agr. Ruggero Manca · ODAF Lecce n° 636 · idearurale
