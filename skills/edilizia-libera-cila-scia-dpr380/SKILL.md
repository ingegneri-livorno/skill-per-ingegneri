---
name: edilizia-libera-cila-scia-dpr380
description: "Supporto documentale ai regimi del titolo edilizio diversi dal permesso di costruire secondo il DPR 380/2001 (Testo unico edilizia), Titolo II. Aiuta a inquadrare l'attivita' edilizia libera, la CILA, la SCIA e la SCIA in alternativa al permesso di costruire. Use when a technician, designer or citizen must frame which building title applies (free building activity, CILA, SCIA or SCIA alternative to the building permit) under the Italian Testo unico edilizia; it is a documentary aid, does not qualify the specific intervention, does not draft the CILA/SCIA and does not replace the SUE/municipality or regional rules."
license: MIT
area: edilizia-urbanistica-catasto
title: "Edilizia libera, CILA e SCIA (DPR 380/2001 artt. 6, 6-bis, 22, 23)"
summary: "Inquadra i regimi del titolo edilizio diversi dal permesso di costruire (DPR 380/2001): edilizia libera senza titolo (art. 6), CILA asseverata residuale (art. 6-bis), SCIA ex art. 19 L. 241/1990 (art. 22), SCIA in alternativa al PdC con preavviso di 30 giorni (art. 23)."
normative_refs:
  - "D.P.R. 6/6/2001 n. 380 - artt. 6 (attivita' edilizia libera) e 6-bis (CILA)"
  - "D.P.R. 6/6/2001 n. 380 - artt. 22 (SCIA) e 23 (SCIA in alternativa al permesso di costruire)"
  - "D.L. 11/11/2026 n. 205 (GU n. 263, vigente dal 12/11/2026, da convertire) - art. 9: Campi Flegrei, piani comunali: consumo di suolo per nuove costruzioni/ristrutturazioni solo in casi eccezionali"
version: 0.2.0-alpha
status: alpha
tags:
  - dpr-380-2001
  - edilizia
  - titolo-edilizio
  - cila
  - scia
  - edilizia-libera
---

# Edilizia libera, CILA e SCIA (DPR 380/2001 artt. 6, 6-bis, 22, 23)

## Quando usare questa skill

Usala quando devi **inquadrare quale titolo edilizio** si applica a un intervento,
diverso dal **permesso di costruire**, ancorandolo al **DPR 380/2001, Titolo II**:

- **attivita' edilizia libera** - **art. 6**: interventi eseguibili **senza alcun titolo
  abilitativo** (manutenzione ordinaria, eliminazione di **barriere architettoniche** senza
  ascensori esterni/alterazione sagoma, **VEPA**, **tende/pergole**, opere temporanee di
  ricerca geognostica, movimenti di terra agricoli, serre mobili stagionali, **opere
  stagionali fino a 180 giorni**, pavimentazioni/finiture di spazi esterni, aree ludiche,
  vasche per acque meteoriche), **fatte salve** le normative di settore (sismica, sicurezza,
  antincendio, igiene, energia, idrogeologico, beni culturali/paesaggio);
- **CILA** - **art. 6-bis**: gli interventi **non riconducibili** agli artt. 6, 10 e 22 sono
  realizzabili previa **comunicazione di inizio lavori asseverata** da un tecnico abilitato
  (conformita' urbanistica, compatibilita' sismica/energetica, **nessun interessamento delle
  parti strutturali**); **sanzione 1.000 euro** (ridotta di due terzi se spontanea);
- **SCIA** - **art. 22**: **segnalazione certificata di inizio attivita'** (ex **art. 19 L.
  241/1990**) per manutenzione straordinaria e restauro/risanamento **su parti strutturali**,
  **ristrutturazione** diversa da quella "pesante" (art. 10 c. 1 lett. c), **varianti** a
  permessi di costruire;
- **SCIA in alternativa al permesso di costruire** - **art. 23**: **ristrutturazione
  "pesante"** (art. 10 c. 1 lett. c) e **nuova costruzione/ristrutturazione urbanistica** in
  attuazione di **piani attuativi**/strumenti generali con precise disposizioni
  plano-volumetriche; **relazione del progettista** e **termine di 30 giorni** prima
  dell'inizio dei lavori; **contributo di costruzione** (art. 16); efficacia **3 anni**.

**Non e' una skill di qualificazione/redazione**: non decide in concreto la categoria
dell'intervento (art. 3), non redige la CILA/SCIA e non sostituisce il SUE/Comune.

## Cosa NON fa (limiti)

- Non **qualifica in concreto** l'intervento (categoria ex art. 3): rinvio a
  `definizioni-interventi-edilizi-dpr380`.
- Non tratta il **permesso di costruire** (art. 10, 20): skill
  `permesso-costruire-dpr380`.
- Non riproduce il **glossario dell'edilizia libera** (DM 2/3/2018) ne' la **modulistica
  unificata** (skill `modulistica-edilizia-unificata`).
- Non **redige** la CILA/SCIA, l'asseverazione o la relazione del progettista.
- Non tratta le **discipline regionali** (che possono ampliare/ridurre gli ambiti) ne' i
  **vincoli** (paesaggio, sismica): rinvio.

## Sotto-attivita'

| Task | Descrizione |
|---|---|
| [`scegli-titolo-edilizio`](tasks/scegli-titolo-edilizio.md) | Inquadra il regime applicabile (edilizia libera art. 6, CILA art. 6-bis, SCIA art. 22, SCIA alternativa art. 23) a partire dalla categoria dell'intervento (art. 3) |
| [`imposta-scia-alternativa`](tasks/imposta-scia-alternativa.md) | Imposta gli adempimenti della SCIA (art. 22) e della SCIA in alternativa al PdC (art. 23): relazione, termini, contributo, efficacia |

## Zona dei Campi Flegrei: regime speciale D.L. 205/2026 - stato al 15 novembre 2026

Per immobili e interventi nella **zona di intervento dei Campi Flegrei** (art. 1 c. 5: territorio dei comuni di Bacoli, Napoli e Pozzuoli ricompreso nella zona del Piano straordinario dell'art. 2 del D.L. 140/2023; per le funzioni degli artt. 12, 13 e 13-bis del D.L. 144/2026 anche il comune di Monte di Procida) si applica il regime speciale del **D.L. 11 novembre 2026, n. 205** "Piano straordinario per i Campi Flegrei nonche' ulteriori disposizioni urgenti di protezione civile" (GU SG n. 263 dell'11/11/2026, in vigore dal **12/11/2026**, art. 28). Fonte: https://www.gazzettaufficiale.it/eli/id/2026/11/11/26G00225/sg - testo in [`references/fonti/dl-205-2026-gu-263.md`](references/fonti/dl-205-2026-gu-263.md).

- **Art. 9 (consumo del suolo)**: nella zona gli strumenti urbanistici comunali prevedono consumo di suolo per interventi di **nuova costruzione** o di **ristrutturazione edilizia** (D.P.R. 380/2001 art. 3 c. 1 lett. d ed e) **"soltanto in casi eccezionali"**: per riduzione del rischio, adeguamento funzionale e igienico-sanitario degli immobili esistenti, protezione civile, mobilita', fornitura di servizi essenziali, da motivare adeguatamente, ed **esclusivamente** se e' dimostrata l'**insostenibilita' tecnica ed economica di riqualificare o rigenerare aree gia' edificate** (modalita' da definire con ordinanza del Commissario) e la compatibilita' con la pianificazione di protezione civile. La norma si rivolge agli strumenti urbanistici, non al singolo titolo: per gli interventi di ristrutturazione edilizia in SCIA (art. 22) o in SCIA alternativa al permesso di costruire (art. 23) verificare lo strumento urbanistico vigente e le ordinanze del Commissario.
- **Art. 13 (semplificazione procedimentale)**: per gli **interventi edilizi realizzati prima del 1/8/2026** sugli immobili oggetto dei contributi per la riduzione della vulnerabilita' sismica e per il ripristino, il pronto ripristino e la riqualificazione sismica elencati al c. 1 si applica, in quanto compatibile, l'**art. 1-sexies del D.L. 55/2018**. Le richieste di **permesso di costruire in sanatoria** e le **SCIA in sanatoria** presentate ai sensi del c. 1, anche contestualmente alla domanda di contributo, sono concluse dal Comune **entro 60 giorni** (c. 2); il Comune puo' chiedere **una sola volta**, entro 15 giorni, le integrazioni strettamente necessarie, con sospensione dei termini fino alla ricezione e comunque per non oltre 30 giorni (c. 3). Le **istanze di condono** non ancora definite sono definite **con priorita' entro 90 giorni** dalla comunicazione della domanda di contributo (c. 4). La concessione del contributo e' subordinata alla positiva conclusione della sanatoria o del condono (c. 6); restano ferme le norme antisismiche e le altre discipline di settore (c. 5) e la conformita' alle norme tecniche sismiche sia alla realizzazione sia al rilascio del titolo in sanatoria (c. 8).
- **Decreto-legge non ancora convertito**: il decreto "sara' presentato alle Camere per la conversione in legge" (art. 28); le disposizioni possono cambiare in sede di conversione. Ricontrollare questa sezione alla pubblicazione della legge di conversione in GU.
- **Ordinanze del Commissario**: sugli interventi relativi al patrimonio edilizio privato la Conferenza di servizi permanente si esprime "nelle modalita' e nei casi stabiliti con ordinanza del Commissario" (art. 10 c. 3 lett. d); le procedure per i lavori privati nella zona vanno quindi verificate sulle ordinanze commissariali vigenti.
- **Segnalalo all'utente** quando l'immobile o l'opera ricade nella zona. La skill non ricostruisce il regime speciale ne' il contenuto delle ordinanze: rinvia al testo del decreto e agli atti del Commissario.

## Riferimenti normativi

- **D.P.R. 6 giugno 2001, n. 380** (Testo unico edilizia) - Titolo II - artt. **6**
  (edilizia libera), **6-bis** (CILA), **22** (SCIA), **23** (SCIA in alternativa al
  permesso di costruire); richiamati gli artt. **3** (definizioni), **10** (PdC), **16**
  (contributo), **37** e **44** (sanzioni) e l'**art. 19 della L. 241/1990**.
- **D.L. 11/11/2026 n. 205** (Campi Flegrei) - artt. 1, 9, 10, 13, 28; decreto-legge da convertire in legge.

Dettaglio in `references/sources.yaml`,
`references/fonti/dpr-380-2001-6-6bis-22-23.md`,
`references/estratti/titoli-edilizi-checklist.md`.

## Avvertenza

Skill di **supporto documentale**: la qualificazione dell'intervento, la scelta del
titolo in concreto, la redazione della CILA/SCIA e delle asseverazioni e il rispetto
delle discipline regionali e dei vincoli restano in capo al **tecnico abilitato** e al
**SUE/Comune**. **Non sostituisce** il tecnico abilitato ne' il SUE/Comune, ne' la
lettura degli artt. 6, 6-bis, 22, 23 del DPR 380/2001.
