---
name: verifica-progettazione-dlgs36
description: "Supporto documentale al RUP (responsabile unico del progetto), al soggetto verificatore e al progettista per la verifica della progettazione e la validazione del progetto posto a base di gara nei contratti pubblici di lavori, ai sensi del D.Lgs. 31 marzo 2023, n. 36 (Codice dei contratti pubblici), art. 42. Use when a project procedure manager (RUP), a design checker, or a designer must frame the design verification and the validation of the project put out to tender under D.Lgs. 36/2023 art. 42; it is a documentary aid and does NOT perform the verification, does NOT draft the verification report or the validation act, does NOT reproduce annex I.7 or the seismic obligations, and does NOT replace the RUP, the checker, or the designer."
license: MIT
area: appalti-opere-pubbliche
title: "Verifica della progettazione e validazione del progetto (D.Lgs. 36/2023 art. 42)"
summary: "Inquadra la verifica della progettazione e la validazione del progetto a base di gara (D.Lgs. 36/2023 art. 42): oggetto e tempi per livello (1), RUP e incompatibilita' (2), effetti - deposito sismico e denuncia al genio civile assolti (3), validazione (4), Allegato I.7 (5)."
normative_refs:
  - "D.Lgs. 31 marzo 2023, n. 36 (Codice dei contratti pubblici) - art. 42 (Verifica della progettazione): oggetto e tempi, RUP e incompatibilita', effetti, validazione, rinvio all'Allegato I.7"
  - "Rinvio (non riprodotti): Allegato I.7 D.Lgs. 36/2023 (contenuti, modalita' e soggetti della verifica); art. 41 (livelli di progettazione); DPR 380/2001 artt. 65, 93-94 (deposito sismico)"
  - "D.L. 11/11/2026 n. 205 (GU n. 263 dell'11/11/2026, vigente dal 12/11/2026, da convertire) - art. 10: Campi Flegrei, progetti pubblici approvati in Conferenza di servizi permanente (art. 38 Codice)"
version: 0.2.0-alpha
status: alpha
tags:
  - verifica-progettazione
  - validazione-progetto
  - dlgs-36-2023
  - contratti-pubblici
  - rup
---

# Verifica della progettazione e validazione del progetto (D.Lgs. 36/2023 art. 42)

## Quando usare questa skill

Usala quando un **RUP** (responsabile unico del progetto), un **soggetto verificatore** o un
**progettista** deve **inquadrare** la **verifica della progettazione** e la **validazione** del progetto
posto a base di gara nei **contratti pubblici di lavori**, secondo il **D.Lgs. 31 marzo 2023, n. 36**
(Codice dei contratti pubblici), **art. 42**:

- **oggetto** e **tempi** della verifica in relazione al livello progettuale (c. 1);
- **ruolo del RUP** e **incompatibilità** della verifica (c. 2);
- **effetti** della verifica positiva (deposito sismico, denuncia al genio civile) (c. 3);
- **validazione** del progetto a base di gara (c. 4) e rinvio all'**Allegato I.7** (c. 5).

**Non è** uno strumento che esegue la verifica o redige il rapporto/atto di validazione: è un **supporto
documentale** che inquadra oggetto, tempi, soggetti ed effetti.

## Cosa fa

| Sotto-attività | Descrizione |
|---|---|
| `inquadra-verifica-progetto` | Inquadra oggetto e tempi della verifica per livello, il ruolo del RUP e le incompatibilità (art. 42 cc. 1-2) |
| `inquadra-validazione-effetti` | Inquadra gli effetti della verifica positiva (deposito sismico, Archivio OO.PP.) e la validazione a base di gara (art. 42 cc. 3-5) |

## Punti chiave (verificati sul testo)

- **Oggetto** (c. 1): rispondenza al **documento d'indirizzo (DIP)** + **conformità alla normativa**;
  verifica **durante lo sviluppo**, per livello (**PFTE**/esecutivo). Congiunto/PPP: PFTE **prima
  dell'affidamento**, esecutivo **prima dell'inizio lavori**.
- **RUP e incompatibilità** (c. 2): il RUP verifica o **segue** con **contraddittorio**; la verifica è
  **incompatibile** con progettazione, coordinamento sicurezza, **direzione lavori** e **collaudo**.
- **Effetti** (c. 3): la verifica positiva **assolve** deposito/autorizzazione **sismica** e **denuncia
  al genio civile**; deposito nell'**Archivio informatico nazionale delle opere pubbliche** (MIT).
- **Validazione** (c. 4): **atto formale** del **RUP** con gli esiti della verifica, riferito al
  **rapporto conclusivo** e alle **controdeduzioni** del progettista; **estremi nel bando/lettera
  d'invito**.
- **Contenuti/soggetti** (c. 5): **Allegato I.7** (contenuti, modalità e soggetti; correlati all'importo
  dei lavori); oneri **nelle risorse dell'opera**.

## Zona dei Campi Flegrei: regime speciale D.L. 205/2026 - stato al 15 novembre 2026

Per immobili e interventi nella **zona di intervento dei Campi Flegrei** (art. 1 c. 5: territorio dei comuni di Bacoli, Napoli e Pozzuoli ricompreso nella zona del Piano straordinario dell'art. 2 del D.L. 140/2023; per le funzioni degli artt. 12, 13 e 13-bis del D.L. 144/2026 anche il comune di Monte di Procida) si applica il regime speciale del **D.L. 11 novembre 2026, n. 205** "Piano straordinario per i Campi Flegrei nonche' ulteriori disposizioni urgenti di protezione civile" (GU SG n. 263 dell'11/11/2026, in vigore dal **12/11/2026**, art. 28). Fonte: https://www.gazzettaufficiale.it/eli/id/2026/11/11/26G00225/sg - testo in [`references/fonti/dl-205-2026-gu-263.md`](references/fonti/dl-205-2026-gu-263.md).

- **Art. 10 (Conferenza di servizi permanente)**: e' istituita la "Conferenza di servizi permanente per l'area dei Campi Flegrei", presieduta dal Commissario. La sua determinazione conclusiva **sostituisce a ogni effetto tutti i pareri, intese, concerti, nulla osta o altri atti di assenso** delle amministrazioni coinvolte e ha **effetto di variante agli strumenti urbanistici** vigenti. La Conferenza **approva, ai sensi dell'art. 38 del D.Lgs. 36/2023**, i progetti dei soggetti attuatori degli interventi sul patrimonio edilizio pubblico (c. 3 lett. b) e i progetti delle opere pubbliche e dei lavori su beni culturali di competenza del Commissario, del Ministero della cultura e del MIT (c. 3 lett. c).
- Il decreto non nomina la verifica e la validazione dell'art. 42: restano gli adempimenti del Codice; cambia la sede di approvazione del progetto, che per questi interventi e' la Conferenza di servizi permanente. Verificare con il RUP e gli atti del Commissario come si coordinano i passaggi.
- **Decreto-legge non ancora convertito**: il decreto "sara' presentato alle Camere per la conversione in legge" (art. 28); le disposizioni possono cambiare in sede di conversione. Ricontrollare questa sezione alla pubblicazione della legge di conversione in GU.
- **Ordinanze del Commissario**: sugli interventi relativi al patrimonio edilizio privato la Conferenza di servizi permanente si esprime "nelle modalita' e nei casi stabiliti con ordinanza del Commissario" (art. 10 c. 3 lett. d); le procedure per i lavori privati nella zona vanno quindi verificate sulle ordinanze commissariali vigenti.
- **Segnalalo all'utente** quando l'immobile o l'opera ricade nella zona. La skill non ricostruisce il regime speciale ne' il contenuto delle ordinanze: rinvia al testo del decreto e agli atti del Commissario.

## Fonti

- **D.Lgs. 31 marzo 2023, n. 36** (Codice dei contratti pubblici) - **art. 42** - testo vigente su
  Normattiva (indice pinnato a `!vig=2026-07-17`, codice 23G00044, idGruppo 5).
- **D.L. 11/11/2026 n. 205** (Campi Flegrei) - artt. 1, 10, 28; decreto-legge da convertire in legge.

Dettaglio in `references/sources.yaml`, `references/fonti/`, `references/estratti/`.

## Limiti

- **Non esegue** la verifica né redige il **rapporto di verifica** o l'**atto di validazione**.
- **Non riproduce** l'**Allegato I.7** (soglie di importo e soggetti verificatori) né gli **obblighi
  sismici** del DPR 380.
- **Non tratta** la **verifica di conformità/collaudo in esecuzione** (skill
  `collaudo-verifica-conformita-dlgs36`) né i **contenuti del PFTE** (skill `pfte-allegato-i7-checker`)
  se non nei richiami.

**La skill è un supporto documentale: non sostituisce il RUP, il soggetto verificatore o il progettista,
né la lettura dell'art. 42 del D.Lgs. 36/2023 e dell'Allegato I.7.**
