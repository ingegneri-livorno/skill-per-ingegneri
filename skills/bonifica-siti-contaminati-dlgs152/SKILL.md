---
name: bonifica-siti-contaminati-dlgs152
description: "Supporto documentale alla procedura di bonifica dei siti contaminati ai sensi del Titolo V della Parte quarta del D.Lgs. 152/2006: aiuta a orientarsi tra le definizioni chiave, la procedura operativa a iniziativa del responsabile, il procedimento a iniziativa della pubblica amministrazione con ordinanza (art. 244), le aree di ridotte dimensioni (art. 249) e le sanzioni penali (art. 257). Use when an Italian consultant or operator must map the contaminated-site remediation procedure, its deadlines and the actors involved; it is a documentary aid and does not read the CSC tables, does not run the risk analysis nor draft the characterization plan."
license: MIT
area: ambiente-territorio-mobilita
title: "Bonifica siti contaminati - D.Lgs. 152/2006 Titolo V"
summary: "Procedura di bonifica dei siti contaminati (D.Lgs. 152/2006 Titolo V): definizioni CSC/CSR (art. 240), procedura del responsabile (art. 242), ordinanza PA (art. 244: 150 giorni, sostituzione regionale, D.L. 177/2026), aree ridotte (art. 249), sanzioni (art. 257)"
normative_refs:
  - "D.Lgs. 3/4/2006 n. 152 (testo vigente) - Parte quarta Titolo V, artt. 240, 242, 244, 249, 257"
  - "D.L. 8/10/2026 n. 177 (GU n. 234 dell'8/10/2026, in vigore dal 9/10/2026, da convertire in legge) - art. 5: modifiche agli artt. 244 e 252 D.Lgs. 152/2006 e all'All. 5 Tab. 2"
version: 0.2.0-alpha
status: alpha
tags:
  - dlgs-152-2006
  - bonifica
  - siti-contaminati
  - analisi-di-rischio
  - testo-unico-ambientale
---

# Bonifica siti contaminati - D.Lgs. 152/2006 Titolo V

## Quando usare questa skill

Usala quando devi orientarti sulla **procedura di bonifica dei siti
contaminati** ai sensi del **Titolo V della Parte quarta del D.Lgs. 152/2006**:

- distinguere le **definizioni** (CSC, CSR, sito potenzialmente contaminato /
  contaminato / non contaminato, MISE, MISO, messa in sicurezza permanente,
  bonifica, ripristino) (art. 240);
- seguire la **procedura operativa** a iniziativa del responsabile (art. 242) con
  i suoi termini (24 ore, 48 ore, 30 giorni, 6 mesi, 60 giorni);
- capire il **procedimento a iniziativa della PA** con ordinanza (art. 244),
  incluso il **termine di 150 giorni** e il **potere sostitutivo della regione**
  introdotti dal D.L. 177/2026;
- conoscere le **aree di ridotte dimensioni** (art. 249) e le **sanzioni** (art.
  257).

**Non e' una skill di calcolo**: non legge i valori CSC (Allegato 5), non esegue
l'analisi di rischio (Allegato 1) ne' redige il piano di caratterizzazione
(Allegato 2).

## Cosa NON fa (limiti)

- Non riproduce i **valori CSC** (Allegato 5) ne' calcola le **CSR**: rinvia agli
  allegati e ai criteri/software di analisi di rischio.
- Non redige il **piano di caratterizzazione**, il progetto di bonifica ne' i
  piani di monitoraggio.
- Non tratta i **SIN** (siti di interesse nazionale, art. 252) ne' oneri reali e
  privilegi (artt. 250, 253) oltre ai richiami.
- Non sostituisce il tecnico competente ne' l'autorita' (regione, provincia,
  comune, ARPA).

## Sotto-attivita'

| Task | Descrizione |
|---|---|
| [`diagnosi-procedura`](tasks/diagnosi-procedura.md) | Dato l'evento (potenziale contaminazione, contaminazione storica, esito indagine preliminare), individua lo step della procedura dell'art. 242, i termini e gli attori, distinguendo sotto/sopra CSC e sopra CSR |
| [`checklist-adempimenti`](tasks/checklist-adempimenti.md) | Verifica la completezza degli adempimenti e dei termini (comunicazioni, autocertificazione, piano di caratterizzazione, analisi di rischio) e le sanzioni (art. 257) |

## Riferimenti normativi

- **D.Lgs. 3/4/2006 n. 152** (TUA), Parte quarta Titolo V, testo vigente su
  Normattiva:
  - **art. 240** (definizioni), **art. 242** (procedure operative), **art. 244**
    (ordinanze PA), **art. 249** (aree ridotte), **art. 257** (sanzioni penali).
- **D.L. 8/10/2026 n. 177** (GU SG n. 234 dell'8/10/2026), in vigore dal
  9/10/2026 (art. 6) e **presentato alle Camere per la conversione in legge**:
  verificare sempre il testo convertito. **Art. 5**: art. 244 c. 3 (ordinanza
  entro 150 giorni dalla comunicazione del c. 1) e nuovo c. 4-ter (la regione
  assegna alla provincia fino a 30 giorni, poi adotta l'ordinanza con il supporto
  SNPA); art. 252 c. 3 (aree marine dei SIN); All. 5 Tab. 2 METALLI (soppresse
  la decima e la sedicesima riga); estensione dell'art. 6 c. 1 D.L. 153/2024
  (semplificazioni siti orfani) agli interventi di bonifica finanziati dai Fondi
  ex art. 1 c. 177 L. 178/2020 e art. 1 c. 6 L. 147/2013. Non modifica gli artt.
  242, 245, 250.

Dettaglio in `references/sources.yaml`, `references/fonti/dlgs-152-2006.md`,
`references/estratti/bonifica-siti-checklist.md`.

## Avvertenza

Skill di **supporto documentale**: i valori CSC, l'analisi di rischio e i
progetti richiedono la lettura degli allegati e l'intervento di tecnici
qualificati; la decisione spetta all'autorita' competente.
