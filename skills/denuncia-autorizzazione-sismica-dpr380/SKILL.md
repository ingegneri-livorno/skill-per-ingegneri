---
name: denuncia-autorizzazione-sismica-dpr380
description: "Supporto documentale agli adempimenti per le costruzioni in zone sismiche secondo il DPR 380/2001 (Testo unico edilizia), Parte II, Capo IV. Aiuta a inquadrare la denuncia dei lavori e la presentazione del progetto, l'autorizzazione per l'inizio dei lavori e la disciplina degli interventi strutturali. Use when a technician must frame the seismic works notice, the prior authorization and the classification of structural interventions in seismic zones under the Italian Testo unico edilizia; it is a documentary aid, does not draft the notice or the structural design, does not perform calculations and does not replace the regional technical office or the SUE."
license: MIT
area: strutture-geotecnica
title: "Denuncia lavori e autorizzazione sismica (DPR 380/2001 artt. 93, 94, 94-bis)"
summary: "Inquadra gli adempimenti per le costruzioni in zone sismiche (DPR 380/2001): denuncia lavori e deposito del progetto asseverato (art. 93), autorizzazione preventiva dell'ufficio regionale (art. 94), classificazione degli interventi per rilevanza e zona sismica (art. 94-bis)."
normative_refs:
  - "D.P.R. 6/6/2001 n. 380 - artt. 93 (denuncia lavori e deposito progetto) e 94 (autorizzazione per l'inizio dei lavori)"
  - "D.P.R. 6/6/2001 n. 380 - art. 94-bis (disciplina degli interventi strutturali in zone sismiche)"
  - "D.L. 11/11/2026 n. 205 (GU n. 263 dell'11/11/2026, vigente dal 12/11/2026, da convertire) - artt. 18-19: Campi Flegrei, programmi del Commissario di riparazione e prevenzione sismica"
version: 0.2.0-alpha
status: alpha
tags:
  - dpr-380-2001
  - zone-sismiche
  - denuncia-lavori
  - autorizzazione-sismica
  - interventi-strutturali
  - strutture
---

# Denuncia lavori e autorizzazione sismica (DPR 380/2001 artt. 93, 94, 94-bis)

## Quando usare questa skill

Usala quando devi **inquadrare gli adempimenti** per le **costruzioni in zone sismiche** e
ancorarli al **DPR 380/2001, Parte II, Capo IV**:

- **denuncia dei lavori e deposito del progetto** - **art. 93**: nelle **zone sismiche**
  (art. 83), chi intende procedere a costruzioni/riparazioni/sopraelevazioni da' **preavviso
  scritto** allo **sportello unico**, che ne trasmette copia al **competente ufficio tecnico
  della regione**; **deposito del progetto** (doppio esemplare, firmato da tecnico abilitato
  e dal DL); **contenuto minimo** e **asseverazione** del progettista (rispetto delle NTC,
  coerenza strutture/architettonico, prescrizioni sismiche urbanistiche); il preavviso vale
  anche come **denuncia ex art. 65**; **registro comunale** delle denunce;
- **autorizzazione per l'inizio dei lavori** - **art. 94**: nelle **localita' sismiche**
  (escluse quelle a **bassa sismicita'** indicate nei decreti ex art. 83) non si possono
  **iniziare i lavori senza preventiva autorizzazione** del competente ufficio tecnico
  regionale; **rilascio entro 30 giorni**; **silenzio assenso** (c. 2-bis) con attestazione
  SUE; **ricorso** al presidente della giunta regionale; **direzione lavori** da tecnico
  abilitato;
- **disciplina degli interventi strutturali** - **art. 94-bis**: classifica gli interventi
  in **"rilevanti"** (a), **"di minore rilevanza"** (b) e **"privi di rilevanza"** (c) per la
  pubblica incolumita', in funzione della **zona sismica** (1/2/3/4) e del tipo di
  intervento; per gli interventi **rilevanti** serve l'**autorizzazione** ex art. 94; per gli
  altri **non** si applica l'autorizzazione preventiva (deroga), salvo **controlli a
  campione** regionali; restano ferme le procedure degli **artt. 65 e 67 c. 1**.

**Non e' una skill di calcolo/redazione**: non redige la denuncia/istanza ne' il progetto
strutturale, non esegue calcoli e non sostituisce l'ufficio tecnico regionale/SUE.

## Cosa NON fa (limiti)

- Non **redige** la denuncia/istanza, l'asseverazione ne' il **progetto strutturale**.
- Non **esegue calcoli** strutturali/sismici (NTC, DM 17/1/2018): rinvio alle skill NTC.
- Non riproduce le **linee guida MIT** (DM 30/4/2018) ne' le **elencazioni/procedure
  regionali** di dettaglio: rinvio.
- Non tratta la **denuncia delle opere in c.a./acciaio** (art. 65): skill
  `denuncia-opere-strutturali-l1086`.
- Non individua la **classificazione sismica** del sito (zona 1-4, art. 83): dato di fatto da
  verificare presso la regione/comune.

## Sotto-attivita'

| Task | Descrizione |
|---|---|
| [`inquadra-denuncia-autorizzazione`](tasks/inquadra-denuncia-autorizzazione.md) | Imposta il preavviso/denuncia e il deposito del progetto (art. 93) e verifica se serve l'autorizzazione preventiva (art. 94) |
| [`classifica-intervento-sismico`](tasks/classifica-intervento-sismico.md) | Classifica l'intervento come rilevante, di minore rilevanza o privo di rilevanza (art. 94-bis) e ne deduce il regime (autorizzazione vs deposito) |

## Zona dei Campi Flegrei: regime speciale D.L. 205/2026 - stato al 15 novembre 2026

Per immobili e interventi nella **zona di intervento dei Campi Flegrei** (art. 1 c. 5: territorio dei comuni di Bacoli, Napoli e Pozzuoli ricompreso nella zona del Piano straordinario dell'art. 2 del D.L. 140/2023; per le funzioni degli artt. 12, 13 e 13-bis del D.L. 144/2026 anche il comune di Monte di Procida) si applica il regime speciale del **D.L. 11 novembre 2026, n. 205** "Piano straordinario per i Campi Flegrei nonche' ulteriori disposizioni urgenti di protezione civile" (GU SG n. 263 dell'11/11/2026, in vigore dal **12/11/2026**, art. 28). Fonte: https://www.gazzettaufficiale.it/eli/id/2026/11/11/26G00225/sg - testo in [`references/fonti/dl-205-2026-gu-263.md`](references/fonti/dl-205-2026-gu-263.md).

- **Art. 18 (programma pluriennale del Commissario)**: il Commissario predispone un **programma pluriennale**, aggiornabile annualmente, di interventi di **riparazione e riqualificazione sismica** degli edifici di proprieta' pubblica, delle infrastrutture di trasporto, di mitigazione del rischio da crollo dei costoni rocciosi, dei centri operativi comunali di protezione civile e delle aree di attesa e di raccolta, e degli altri servizi essenziali danneggiati dagli eventi sismici del fenomeno bradisismico; priorita' a edifici scolastici e universitari, servizi pubblici essenziali, edilizia residenziale pubblica ed edifici che ospitano minori, detenuti o persone con disabilita'. Il programma e' approvato con decreto del Ministro per la protezione civile e le politiche del mare, previa deliberazione del Consiglio dei ministri (c. 2).
- **Art. 18 c. 4 (demolizione e ricostruzione altrove, solo per gli interventi del programma pubblico del c. 1)**: se il costo di riparazione e riqualificazione sismica e' **pari o equivalente al costo di demolizione e ricostruzione**, si provvede, ove possibile e in via preferenziale, alla **demolizione** e alla **ricostruzione in altra area** individuata dal Commissario fuori dalla zona di intervento e comunque non esposta al rischio bradisismico.
- **Art. 19 (prevenzione sismica)**: i programmi di intervento dell'art. 9-ter c. 2 lett. a) nn. 1 e 2 del **D.L. 76/2024** possono essere predisposti dal Commissario anche a valere sul fondo dell'art. 5 c. 1 lett. b) del decreto e, annualmente, **confluiscono in un unico programma di prevenzione strutturale**, pubblicato dal Commissario sul proprio sito istituzionale.
- Le parti trascritte del decreto non modificano gli artt. 93, 94 e 94-bis del D.P.R. 380/2001. I progetti dei soggetti attuatori sul patrimonio edilizio pubblico e quelli delle opere pubbliche di competenza del Commissario, del Ministero della cultura e del MIT sono pero' approvati dalla Conferenza di servizi permanente (art. 10 c. 3 lett. b-c), la cui determinazione sostituisce gli atti di assenso delle amministrazioni coinvolte. Verificare caso per caso come cio' si coordina con il deposito e l'autorizzazione sismica.
- **Decreto-legge non ancora convertito**: il decreto "sara' presentato alle Camere per la conversione in legge" (art. 28); le disposizioni possono cambiare in sede di conversione. Ricontrollare questa sezione alla pubblicazione della legge di conversione in GU.
- **Ordinanze del Commissario**: sugli interventi relativi al patrimonio edilizio privato la Conferenza di servizi permanente si esprime "nelle modalita' e nei casi stabiliti con ordinanza del Commissario" (art. 10 c. 3 lett. d); le procedure per i lavori privati nella zona vanno quindi verificate sulle ordinanze commissariali vigenti.
- **Segnalalo all'utente** quando l'immobile o l'opera ricade nella zona. La skill non ricostruisce il regime speciale ne' il contenuto delle ordinanze: rinvia al testo del decreto e agli atti del Commissario.

## Riferimenti normativi

- **D.P.R. 6 giugno 2001, n. 380** (Testo unico edilizia) - Parte II, Capo IV - artt. **93**
  (denuncia lavori e deposito progetto), **94** (autorizzazione per l'inizio dei lavori),
  **94-bis** (disciplina degli interventi strutturali); richiamati gli artt. **52**, **65**,
  **67**, **83** (classificazione sismica), il **DM 17/1/2018** (NTC) e le **linee guida MIT
  (DM 30/4/2018)** e le disposizioni regionali (rinvio).
- **D.L. 11/11/2026 n. 205** (Campi Flegrei) - artt. 1, 10, 18, 19, 28; decreto-legge da convertire in legge.

Dettaglio in `references/sources.yaml`,
`references/fonti/dpr-380-2001-93-94-94bis.md`,
`references/estratti/sismica-checklist.md`.

## Avvertenza

Skill di **supporto documentale**: la classificazione dell'intervento, la redazione della
denuncia/istanza e del progetto strutturale, i calcoli e il rilascio dell'autorizzazione
restano in capo al **progettista/direttore dei lavori**, all'**ufficio tecnico regionale** e
al **SUE**. **Non sostituisce** questi soggetti ne' la lettura degli artt. 93, 94, 94-bis
del DPR 380/2001, delle NTC e delle disposizioni regionali.
