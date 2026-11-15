---
name: permesso-costruire-dpr380
description: "Supporto documentale al regime del permesso di costruire ai sensi del D.P.R. 380/2001 (Testo unico edilizia), artt. 11, 12, 15, 20. Aiuta a inquadrare le caratteristiche del titolo, i presupposti per il rilascio, l'efficacia temporale e la decadenza e il procedimento per il rilascio. Use when a designer, technician or applicant must frame the building permit regime, its prerequisites, the procedure and time limits, and the temporal validity/forfeiture under the Italian Testo unico edilizia; it is a documentary aid, does not draft the application or the asseverazione, does not decide whether an intervention needs a permit rather than SCIA/CILA (see modulistica-edilizia-unificata), does not compute the construction contribution and does not replace the SUE, the designer or the Municipality."
license: MIT
area: edilizia-urbanistica-catasto
title: "Permesso di costruire: presupposti, procedimento e decadenza - DPR 380/2001"
summary: "Regime del permesso di costruire (DPR 380/2001): caratteristiche e soggetti (art. 11), presupposti - conformita' urbanistica e urbanizzazioni (art. 12), efficacia e decadenza - inizio 1 anno/fine 3 anni (art. 15), procedimento, termini e silenzio-assenso (art. 20)."
normative_refs:
  - "D.P.R. 6/6/2001 n. 380 - artt. 11 (caratteristiche) e 12 (presupposti per il rilascio)"
  - "D.P.R. 6/6/2001 n. 380 - artt. 15 (efficacia temporale e decadenza) e 20 (procedimento)"
  - "D.L. 11/11/2026 n. 205 (GU n. 263, vigente dal 12/11/2026, da convertire) - art. 9: Campi Flegrei, piani comunali: consumo di suolo per nuove costruzioni/ristrutturazioni solo in casi eccezionali"
version: 0.2.0-alpha
status: alpha
tags:
  - dpr-380-2001
  - testo-unico-edilizia
  - permesso-di-costruire
  - titolo-edilizio
  - silenzio-assenso
  - decadenza
---

# Permesso di costruire: presupposti, procedimento e decadenza - DPR 380/2001

## Quando usare questa skill

Usala quando devi **inquadrare il regime del permesso di costruire** e ancorarlo al
**D.P.R. 380/2001** (Testo unico edilizia), **artt. 11, 12, 15, 20**:

- **caratteristiche del titolo** - **art. 11**: soggetti legittimati (proprietario o
  chi abbia titolo), **trasferibilita'** con l'immobile ai successori/aventi causa,
  **irrevocabilita'**, **onerosita'** (art. 16), il rilascio **non incide** sulla
  proprieta' ne' limita i **diritti dei terzi**;
- **presupposti per il rilascio** - **art. 12**: **conformita'** agli strumenti
  urbanistici, ai regolamenti edilizi e alla disciplina vigente; esistenza o
  **previsione delle opere di urbanizzazione primaria**; **misure di salvaguardia**
  in caso di strumenti adottati;
- **efficacia temporale e decadenza** - **art. 15**: **inizio** lavori entro **un
  anno** dal rilascio, **ultimazione** entro **tre anni** dall'inizio; **proroga**
  motivata; **decadenza di diritto** per la parte non eseguita e per **contrastanti
  previsioni urbanistiche**; nuovo permesso per la parte non ultimata;
- **procedimento per il rilascio** - **art. 20**: **sportello unico** (SUE),
  **asseverazione** del progettista, **responsabile del procedimento**, termini
  (**60 giorni** istruttoria, **30 giorni** provvedimento), **interruzione/
  sospensione** dei termini, **conferenza di servizi**, **silenzio-assenso** e
  relativi limiti (vincoli), **sanzioni** per false attestazioni.

**Non e' una skill di calcolo e non redige gli atti**: non compila la domanda ne'
l'asseverazione, non sceglie il titolo (PdC vs SCIA/CILA), non calcola il contributo
di costruzione e non sostituisce il SUE, il progettista o il Comune.

## Cosa NON fa (limiti)

- Non **decide** se un intervento richieda il **permesso di costruire** anziche'
  SCIA/CILA/edilizia libera (art. 10 e la scelta del titolo): rinvio a
  `modulistica-edilizia-unificata`.
- Non **redige** la domanda di permesso, gli **elaborati** o l'**asseverazione** del
  progettista (art. 20 c. 1).
- Non **calcola** il **contributo di costruzione** (art. 16): coperto da altra skill
  DPR 380.
- Non tratta l'**agibilita'** (art. 24), la **vigilanza/sanzioni** (artt. 27 ss.) ne'
  le specificita' delle **leggi regionali** di semplificazione (richiamate all'art.
  20 c. 12).

## Sotto-attivita'

| Task | Descrizione |
|---|---|
| [`inquadra-presupposti-caratteristiche`](tasks/inquadra-presupposti-caratteristiche.md) | Verifica i presupposti per il rilascio (conformita' urbanistica, urbanizzazioni, salvaguardia; art. 12) e le caratteristiche del titolo (legittimazione, trasferibilita', onerosita'; art. 11) |
| [`verifica-procedimento-termini-decadenza`](tasks/verifica-procedimento-termini-decadenza.md) | Ricostruisce il procedimento e i termini (art. 20: 60/30 giorni, interruzione, conferenza di servizi, silenzio-assenso) e l'efficacia temporale/decadenza (art. 15: 1 anno/3 anni, proroga) |

## Zona dei Campi Flegrei: regime speciale D.L. 205/2026 - stato al 15 novembre 2026

Per immobili e interventi nella **zona di intervento dei Campi Flegrei** (art. 1 c. 5: territorio dei comuni di Bacoli, Napoli e Pozzuoli ricompreso nella zona del Piano straordinario dell'art. 2 del D.L. 140/2023; per le funzioni degli artt. 12, 13 e 13-bis del D.L. 144/2026 anche il comune di Monte di Procida) si applica il regime speciale del **D.L. 11 novembre 2026, n. 205** "Piano straordinario per i Campi Flegrei nonche' ulteriori disposizioni urgenti di protezione civile" (GU SG n. 263 dell'11/11/2026, in vigore dal **12/11/2026**, art. 28). Fonte: https://www.gazzettaufficiale.it/eli/id/2026/11/11/26G00225/sg - testo in [`references/fonti/dl-205-2026-gu-263.md`](references/fonti/dl-205-2026-gu-263.md).

- **Art. 9 (consumo del suolo)**: nella zona gli strumenti urbanistici comunali prevedono consumo di suolo per interventi di **nuova costruzione** o di **ristrutturazione edilizia** (D.P.R. 380/2001 art. 3 c. 1 lett. d ed e) **"soltanto in casi eccezionali"**: per riduzione del rischio, adeguamento funzionale e igienico-sanitario degli immobili esistenti, protezione civile, mobilita', fornitura di servizi essenziali, da motivare adeguatamente, ed **esclusivamente** se e' dimostrata l'**insostenibilita' tecnica ed economica di riqualificare o rigenerare aree gia' edificate** (modalita' da definire con ordinanza del Commissario) e la compatibilita' con la pianificazione di protezione civile. La norma si rivolge agli strumenti urbanistici, non al singolo titolo: per il presupposto della **conformita' urbanistica** (art. 12) verificare lo strumento urbanistico vigente e le ordinanze del Commissario.
- **Decreto-legge non ancora convertito**: il decreto "sara' presentato alle Camere per la conversione in legge" (art. 28); le disposizioni possono cambiare in sede di conversione. Ricontrollare questa sezione alla pubblicazione della legge di conversione in GU.
- **Ordinanze del Commissario**: sugli interventi relativi al patrimonio edilizio privato la Conferenza di servizi permanente si esprime "nelle modalita' e nei casi stabiliti con ordinanza del Commissario" (art. 10 c. 3 lett. d); le procedure per i lavori privati nella zona vanno quindi verificate sulle ordinanze commissariali vigenti.
- **Segnalalo all'utente** quando l'immobile o l'opera ricade nella zona. La skill non ricostruisce il regime speciale ne' il contenuto delle ordinanze: rinvia al testo del decreto e agli atti del Commissario.

## Riferimenti normativi

- **D.P.R. 6/6/2001 n. 380** (Testo unico edilizia) - **artt. 11** (caratteristiche),
  **12** (presupposti), **15** (efficacia temporale e decadenza), **20**
  (procedimento per il rilascio).
- **D.L. 11/11/2026 n. 205** (Campi Flegrei) - artt. 1, 9, 10, 28; decreto-legge da convertire in legge.

Dettaglio in `references/sources.yaml`,
`references/fonti/dpr-380-2001-permesso.md`,
`references/estratti/permesso-costruire-checklist.md`.

## Avvertenza

Skill di **supporto documentale**: la scelta del titolo edilizio, la stesura della
domanda e dell'asseverazione, l'istruttoria, il calcolo del contributo e ogni
determinazione sul caso concreto restano in capo al **progettista**, al **SUE** e al
**Comune**, con le leggi regionali applicabili. **Non sostituisce** il progettista, lo
sportello unico per l'edilizia (SUE) ne' il Comune, ne' la lettura degli artt. 11, 12,
15 e 20 del D.P.R. 380/2001.
