---
name: via-screening-sia-dlgs152
description: "Supporto documentale alla Valutazione di Impatto Ambientale (VIA) ai sensi della Parte Seconda del D.Lgs. 152/2006 (testo vigente) e del DM 30/03/2015. Copre due fasi: (1) la verifica di assoggettabilita' a VIA (screening, art. 19) con la procedura e i termini perentori, la checklist dei contenuti dello Studio Preliminare Ambientale (Allegato IV-bis) e i criteri di decisione (Allegato V), incluse le linee guida per lo screening di competenza regionale (DM 30/03/2015, meccanismi di adeguamento delle soglie); (2) la struttura e la checklist di completezza dei contenuti dello Studio di Impatto Ambientale - SIA (Allegato VII, art. 22). Use when an Italian engineer or environmental consultant needs to plan the VIA screening procedure, check a Studio Preliminare Ambientale or a SIA for completeness against the current D.Lgs. 152/2006 requirements; it is a documentary aid and does not decide assoggettabilita' nor replace the authority or the signing professional."
license: MIT
area: ambiente-territorio-mobilita
title: "VIA - screening (art. 19) e SIA (Allegato VII) D.Lgs. 152/2006"
summary: "Supporto documentale VIA (D.Lgs. 152/2006 + DM 30/03/2015): procedura e termini della verifica di assoggettabilita' (art. 19), checklist dello Studio Preliminare Ambientale (All. IV-bis) e dei criteri (All. V), struttura/checklist del SIA (All. VII); non decide l'esito"
normative_refs:
  - "D.Lgs. 3/4/2006 n. 152 Parte Seconda - artt. 19, 22 + Allegati IV-bis, V, VII (testo vigente)"
  - "D.L. 8/10/2026 n. 177 art. 1 (modifiche artt. 8, 25, 27 D.Lgs. 152/2006; soggetto a conversione)"
  - "DM 30/03/2015 (linee guida verifica assoggettabilita' competenza regionale)"
version: 0.2.0-alpha
status: alpha
tags:
  - via
  - dlgs-152-2006
  - valutazione-impatto-ambientale
  - screening-assoggettabilita
  - studio-impatto-ambientale
---

# VIA - screening (art. 19) e SIA (Allegato VII) D.Lgs. 152/2006

## Quando usare questa skill

Usala quando devi, nell'ambito della Valutazione di Impatto Ambientale (VIA):

- pianificare la **verifica di assoggettabilita' a VIA** (screening) di un
  progetto: procedura, termini perentori, documenti (art. 19);
- verificare la **completezza dello Studio Preliminare Ambientale** rispetto
  all'Allegato IV-bis e ai criteri dell'Allegato V;
- impostare o verificare la **struttura dello Studio di Impatto Ambientale
  (SIA)** rispetto all'Allegato VII (i 12 punti dell'art. 22);
- orientarti sui **criteri e soglie per lo screening di competenza regionale**
  (DM 30/03/2015) e i meccanismi di adeguamento regionale.

Target: ingegneri ambientali, consulenti ambientali, proponenti e tecnici che
predispongono la documentazione VIA.

## Avvertenza

Questa skill e' un **supporto documentale**. **Non decide l'assoggettabilita' a
VIA** (competenza dell'autorita' competente), **non stabilisce se un progetto
specifico rientri negli allegati II-bis/IV** (per questo servono gli elenchi con
le soglie e le norme regionali) e **non sostituisce** i tecnici che redigono e
firmano lo Studio Preliminare Ambientale o il SIA. Fornisce procedura, termini e
checklist di completezza tratti dal testo vigente delle norme.

## Novita' normativa: D.L. 177/2026 (in vigore dal 9/10/2026, soggetto a conversione)

Il D.L. 8/10/2026 n. 177 (GU n. 234 dell'8/10/2026) all'art. 1 c. 1 modifica
l'art. 8 c. 2-bis D.Lgs. 152/2006: la **verifica di assoggettabilita' a VIA**
dei progetti di competenza statale rientranti nell'ambito della Commissione
Tecnica PNRR-PNIEC (PNRR, fondo complementare, progetti attuativi PNIEC
dell'allegato I-bis, progetti idrici dell'allegato II) e' esplicitamente tra le
procedure di tale Commissione, che opera anche con le modalita' dell'art. 19.
**L'art. 19 e l'art. 22 non sono modificati**: procedura, termini e contenuti
restano quelli descritti. Sull'autorizzazione paesaggistica il decreto aggiunge
solo una clausola di coordinamento all'art. 27 c. 2 lett. d) (VIA statale,
rinvio all'art. 25 c. 2-quinquies, primo periodo): nessuna modifica per lo
screening. E' un decreto-legge soggetto a conversione: verificare l'esito in GU.
Dettaglio: `references/estratti/via-screening-sia-checklist.md` sez. F.

## Sotto-attivita' disponibili

- **Screening / verifica di assoggettabilita'**: pianificare il procedimento
  (art. 19) e verificare lo Studio Preliminare Ambientale (All. IV-bis + criteri
  All. V) -> `tasks/screening-verifica-assoggettabilita.md`
- **Checklist SIA**: verificare la struttura/completezza di uno Studio di Impatto
  Ambientale rispetto ai 12 punti dell'Allegato VII ->
  `tasks/checklist-sia.md`

Se la richiesta non e' chiara, chiedi all'utente quale sotto-attivita' desidera.

## Processo generale

1. Identifica la sotto-attivita'.
2. Carica il file `tasks/<task-scelto>.md`.
3. Richiedi gli input necessari (tipo di progetto, competenza statale/regionale,
   documento da verificare, ecc.).
4. Applica la procedura/checklist **citando l'articolo o l'allegato preciso**
   (art. 19, All. IV-bis, All. V, All. VII, DM 30/03/2015).
5. Distingui cio' che e' **cogente** (D.Lgs. 152/2006, DM) da cio' che dipende
   dalle **norme regionali** di adeguamento.
6. Chiudi con il rinvio all'autorita' competente e ai tecnici firmatari.

## Fonti normative

Riferimenti completi in `references/sources.yaml`. Trascrizioni verificate in
`references/fonti/`, estratto operativo in `references/estratti/`:

- `fonti/dlgs-152-2006-via.md` - D.Lgs. 152/2006 art. 19, All. IV-bis, V, VII e,
  in coda, testo ante-decreto degli artt. 8, 25, 27 modificati dal D.L. 177/2026
  (testo vigente da Normattiva, pagina indice pinnata `!vig=2026-07-14`)
- `fonti/dm-30-03-2015-via.md` - DM 30/03/2015 (linee guida screening regionale)
- `fonti/dl-177-2026.md` - D.L. 177/2026 art. 1 e art. 6 (GU n. 234/2026)
- `estratti/via-screening-sia-checklist.md` - checklist operative

## Limiti

Cosa questa skill NON fa:
- non contiene gli elenchi integrali dei progetti (allegati II-bis e IV) con le
  soglie dimensionali: per stabilire se un progetto rientri nello screening,
  consultare gli allegati alla Parte Seconda e il DM 30/03/2015 + norme regionali;
- non copre la procedura di VIA vera e propria (artt. 23-27), il PAUR (art.
  27-bis), la VAS (artt. 11-18) ne' la VIA statale (Commissione art. 8; per le
  sole modifiche del D.L. 177/2026 vedi sezione "Novita' normativa");
- non decide l'assoggettabilita' ne' redige gli studi: fornisce procedura e
  checklist di completezza.
