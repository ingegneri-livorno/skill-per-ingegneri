---
name: autorizzazione-integrata-ambientale-dlgs152
description: "Supporto documentale all'Autorizzazione Integrata Ambientale (AIA/IPPC) secondo il D.Lgs. 3 aprile 2006, n. 152, Parte II, Titolo III-bis, come modificato dal D.Lgs. 197/2026 (recepimento IED2, in vigore dal 12/11/2026). Aiuta a inquadrare la domanda di AIA e i suoi contenuti, la procedura per il rilascio, il contenuto e le condizioni dell'AIA, il rinnovo e riesame e il rispetto delle condizioni con controlli e ispezioni di ISPRA e ARPA e provvedimenti in caso di inosservanza (art. 29-decies). Use when an engineer, plant operator, or environmental consultant must frame the Integrated Environmental Authorization procedure, its content based on BAT, its review, or the inspections under Italian D.Lgs. 152/2006 Title III-bis; it is a documentary aid and does NOT draft the application or the AIA, does NOT identify the applicable BAT, does NOT reproduce Annexes VIII/XII or the BREFs, and does NOT replace the operator, the competent authority, or ISPRA/ARPA."
license: MIT
area: ambiente-territorio-mobilita
title: "Autorizzazione Integrata Ambientale: procedura e controlli (D.Lgs 152/2006)"
summary: "Autorizzazione Integrata Ambientale (AIA/IPPC - D.Lgs 152/2006, Titolo III-bis): domanda (art. 29-ter), procedura (art. 29-quater), contenuto e VLE su BAT (art. 29-sexies), rinnovo e riesame (art. 29-octies), controlli e ispezioni ISPRA/ARPA (art. 29-decies). Non redige l'AIA."
normative_refs:
  - "D.Lgs. 3 aprile 2006, n. 152 - Parte II, Titolo III-bis, artt. 29-ter, 29-quater, 29-sexies, 29-octies, 29-decies"
  - "D.Lgs. 28 settembre 2026, n. 197 - recepimento Dir. (UE) 2024/1785 (IED2), modifiche al D.Lgs. 152/2006, in vigore dal 12/11/2026"
  - "Richiamati: art. 8-bis (Commissione AIA-IPPC), Allegati VIII/VIII-bis/XII, conclusioni sulle BAT/BREF, artt. 5, 6, 29-septies, 29-quattuordecies (sanzioni)"
version: 0.2.0-alpha
status: alpha
tags:
  - aia
  - ippc
  - dlgs-152-2006
  - dlgs-197-2026
  - ied2
  - autorizzazione-ambientale
  - bat
---

# Autorizzazione Integrata Ambientale (AIA): procedura e controlli (D.Lgs 152/2006)

## Quando usare questa skill

Usala quando un **ingegnere, gestore di installazione o consulente ambientale** deve inquadrare l'**Autorizzazione Integrata Ambientale (AIA/IPPC)** secondo il **D.Lgs. 3 aprile 2006, n. 152, Parte II, Titolo III-bis**, come modificato dal **D.Lgs. 28 settembre 2026, n. 197** (recepimento della Dir. (UE) 2024/1785, "IED2"):

- verificare il **campo di applicazione** (Allegati VIII e VIII-bis);
- comporre la **domanda** e i suoi contenuti;
- ricostruire la **procedura** di rilascio (conferenza di servizi, termini);
- inquadrare il **contenuto** dell'AIA (VLE e prestazioni basati sulle **BAT**, sistema di gestione ambientale), il **rinnovo/riesame** e i **controlli/ispezioni**.

Per gli impianti **non soggetti ad AIA** vedi `aua-dpr59-dossier` (AUA) e `scarichi-emissioni-dlgs152` (autorizzazioni singole residuali); per la **VIA** vedi `via-screening-sia-dlgs152`. Questa copre l'**AIA**.

## D.Lgs. 197/2026 (IED2): entrata in vigore e regime transitorio

Il D.Lgs. 197/2026 (GU SG n. 251 del 28-10-2026) **entra in vigore il 12/11/2026**. Prima di applicare una regola, stabilire **quale versione** del Titolo III-bis vale per l'installazione (art. 43 del decreto):

- installazioni già in funzione e autorizzate (attività dell'Allegato VIII al 4 agosto 2024): parte delle nuove regole (art. 29-sexies cc. 3-bis lett. a-d, 4-bis, 4-quater, 9-ter; art. 29-decies cc. 10-ter, 10-quater) si applica **dal riesame/aggiornamento** dell'AIA e comunque **entro il 1° settembre 2036**; fino ad allora vale il testo **vigente al 4 agosto 2024**;
- **BAT-AEPL** (art. 29-sexies c. 4-quinquies): per conclusioni sulle BAT pubblicate dopo il 1° luglio 2026, da subito per le nuove AIA, entro 4 anni per le altre;
- **nuove attività** dell'Allegato VIII: laminazione a freddo e finitura tessile **in funzione prima del 1° luglio 2026** -> dal 1° luglio 2030 (salvo art. 29-sexies cc. 4-quinquies e 9-bis.1); pirolisi, 2.3 b/b-bis, estrazione di minerali -> entro 4 anni dalle conclusioni sulle BAT e al più tardi entro il 1° settembre 2034 (esclusi art. 29-sexies cc. 4-quinquies e 9-bis.1), ma dalla data di autorizzazione se autorizzate per la prima volta dopo conclusioni sulle BAT pubblicate dopo il 1° luglio 2026;
- installazioni che **escono** dall'ambito: esercizio con l'AIA vigente fino al rinnovo e comunque fino a 12 mesi dall'entrata in vigore.

## Campo di applicazione (Allegati VIII e VIII-bis)

L'AIA si applica alle attività dell'**Allegato VIII** e dell'**Allegato VIII-bis** (art. 4 c. 4 lett. c). Il D.Lgs. 197/2026 **amplia l'Allegato VIII** (pirolisi; laminazione a freddo; forgiatura con presse > 30 MN; **fabbricazione di batterie** >= 15 000 Mg/anno di celle; **estrazione di minerali** su scala industriale; **elettrolisi dell'acqua per idrogeno** > 50 Mg/giorno al punto 6.6) e sposta gli **allevamenti di suini e pollame** nel nuovo **Allegato VIII-bis / Titolo III-ter** (soglie in UBA, regime di autorizzazione o registrazione definito dalle regioni). Nelle more delle procedure regionali restano in AIA gli allevamenti con più di 40 000 posti pollame, 2 000 posti suini da produzione di oltre 30 kg o 750 posti scrofe, e quelli coinsediati e tecnicamente connessi con attività dell'Allegato VIII. L'**Allegato X** è abrogato; l'**Allegato XII** (competenza statale) non è modificato.

## Domanda di AIA (art. 29-ter)

L'AIA è richiesta per **nuove installazioni**, **modifiche sostanziali** e **adeguamento** delle esistenti. La **domanda** contiene (c. 1, lett. a-m-bis): descrizione di installazione/attività, materie prime, energia e **acqua** (anche riutilizzata), **fonti ed entità delle emissioni** in ogni comparto (**odori** compresi) ed effetti anche **sulla salute umana**, **tecniche** per prevenire/ridurre le emissioni, misure sui **rifiuti** e di **controllo**, alternative esaminate, la **relazione di riferimento** per le **sostanze pericolose** e la **quietanza della tariffa istruttoria**.

**Completezza** (cc. 4-4-ter, D.Lgs. 197/2026): inoltro entro **10 giorni** alle amministrazioni ambientali, all'autorità sanitaria, al sindaco (e, per l'AIA statale, ai Ministeri interno, salute e imprese); osservazioni entro **20 giorni**; integrazioni chieste **una sola volta** entro **30 giorni dall'avvio** (termine >= 30 giorni, termini interrotti), pena il ritiro dell'istanza.

## Procedura per il rilascio (art. 29-quater)

- **Avvio** entro **30 giorni** dalla domanda; **pubblicazione** entro **15 giorni** dall'avvio (con pubblicazione in **fase precoce** di istanza e progetto di decisione); **osservazioni** entro **30 giorni**, periodo in cui i termini sono sospesi.
- **Conferenza di servizi decisoria** (L. 241/1990). Per l'AIA **statale** vi partecipa il **Ministero della salute** per la tutela della salute pubblica (c. 5-bis); la proposta **ISPRA** sul monitoraggio riceve il **parere dell'Istituto superiore di sanità** (c. 6); per le altre AIA, parere ARPA/APPA.
- L'AIA può prescrivere **approfondimenti o campagne di monitoraggio**, anche sanitari (c. 8-bis); abrogato il c. 7 (richiesta di riesame del sindaco).
- **Integrazioni** in conferenza entro un termine ≤ **90 giorni** (sospensione); **determinazione entro 150 giorni** dalla domanda, salve sospensioni e interruzioni; l'AIA **assorbe** le autorizzazioni di settore e si **coordina con la VIA** (istanza dopo il provvedimento di VIA o di non assoggettabilità).

## Commissione istruttoria AIA-IPPC (art. 8-bis)

Per le **AIA statali** l'istruttoria è curata dalla Commissione AIA-IPPC (art. 8-bis, sostituito dal D.Lgs. 197/2026): **23 esperti**, integrati **entro 3 mesi** con **5 componenti designati dal Ministero della salute** esperti di interazioni ambiente-salute; incarico di 4 anni rinnovabile una volta; regione, provincia e comune possono designare un esperto entro 15 giorni dall'avvio.

## Contenuto e condizioni dell'AIA (art. 29-sexies)

L'AIA include i **valori limite di emissione (VLE)** per gli inquinanti significativi (con riferimento all'allegato II del Reg. (UE) 2024/1244), **non meno rigorosi** della normativa vigente, riferiti alle **BAT** **senza obbligo** di una tecnica specifica, entro i **BAT-AEL** e attestati sui **valori più rigorosi** ottenibili stabilmente; con il D.Lgs. 197/2026 anche **valori limite di prestazione ambientale** e livelli nei **BAT-AEPL** (c. 4-quinquies). Il gestore adotta un **sistema di gestione ambientale** entro il **1° luglio 2030** con audit almeno triennale (per le installazioni già autorizzate verificare il coordinamento con l'art. 43 c. 2-4, che differisce al riesame l'art. 29-sexies c. 3-bis lett. c: punto da confermare con l'autorità competente) e, per le attività 1, 2, 3, 4, 6.1.b, 6.1.c dell'Allegato VIII, un **piano di trasformazione** entro il **30 giugno 2030**. Controlli su **acque sotterranee** almeno ogni **4 anni** e sul **suolo** ogni **9 anni**. **Deroghe** ai BAT-AEL solo su istanza del gestore e motivate; deroghe per **tecniche emergenti** fino a **30 mesi**.

## Rinnovo e riesame (art. 29-octies)

L'autorità **riesamina periodicamente** l'AIA: entro **4 anni** dalle **nuove conclusioni sulle BAT** sull'attività principale e comunque quando sono **trascorsi 10 anni** dal rilascio o dall'ultimo riesame sull'intera installazione; il **gestore** presenta le informazioni **entro 30-180 giorni** dall'avvio. Il D.Lgs. 197/2026 aggiunge trigger per norme di qualità nuove o stato dell'ambiente ricettore, per **rischi sanitari** sopravvenuti (c. 4 lett. c-bis) e per scarichi indiretti (c. 4-bis), e disciplina **piano di trasformazione** e **trasformazione industriale profonda** (proroghe fino a 8 anni, cc. 11-bis - 11-quater).

## Rispetto delle condizioni e controlli (art. 29-decies)

Il gestore **comunica** l'attuazione dell'AIA e svolge gli **autocontrolli**. **ISPRA** (impianti statali) o l'**autorità di controllo individuata dalla regione** con le **ARPA/APPA** eseguono **accertamenti** (anche sul sistema di gestione ambientale) e **ispezioni ordinarie** con **periodicità basata sul rischio** (non oltre **1 anno** per i rischi più elevati, **3 anni** per i meno elevati, **6 mesi** dopo una **grave inosservanza**). In caso di **inosservanza**: **diffida**, **diffida con sospensione senza indugio** per pericolo immediato, **sospensione** per violazioni persistenti pericolose o reiterate più di due volte in un anno e, nei casi gravi, **revoca** dell'AIA e **chiusura** dell'installazione.

## Cosa NON fa (limiti)

- **Non redige** la domanda né l'AIA e **non compila** la modulistica dell'autorità competente.
- **Non individua** le **BAT** applicabili né i **BAT-AEL/BAT-AEPL**: rinvia alle **conclusioni sulle BAT** (BREF).
- **Non riproduce** per intero gli **Allegati VIII/XII**: riporta solo le modifiche del D.Lgs. 197/2026 all'Allegato VIII e il nuovo Allegato VIII-bis; l'**assoggettabilità** va verificata sugli allegati.
- **Non tratta** nel dettaglio il **Titolo III-ter** (allevamenti) né le modifiche alle Parti Quarta e Quinta.
- **Non sostituisce** il **gestore**, l'**autorità competente** o **ISPRA/ARPA**; non tratta le **sanzioni** (art. 29-quattuordecies) se non come richiamo.

## Sotto-attività

| Task | Descrizione |
|---|---|
| [`inquadra-domanda-aia`](tasks/inquadra-domanda-aia.md) | Verifica l'assoggettabilità (All. VIII/VIII-bis) e il regime transitorio, compone i contenuti della domanda di AIA (art. 29-ter) e i passi della procedura (art. 29-quater) |
| [`verifica-condizioni-controlli`](tasks/verifica-condizioni-controlli.md) | Inquadra il contenuto/condizioni dell'AIA su BAT (art. 29-sexies), il riesame (art. 29-octies) e i controlli/inosservanze (art. 29-decies) |

## Riferimenti normativi

- **D.Lgs. 3 aprile 2006, n. 152** (Parte II, Titolo III-bis) - **art. 29-ter** (domanda), **art. 29-quater** (procedura), **art. 29-sexies** (contenuto/condizioni/BAT), **art. 29-octies** (rinnovo e riesame), **art. 29-decies** (rispetto delle condizioni, controlli e inosservanze).
- **D.Lgs. 28 settembre 2026, n. 197** (GU SG n. 251 del 28-10-2026, in vigore dal 12/11/2026) - recepimento della Dir. (UE) 2024/1785: modifiche agli artt. 4, 5, 6, 8-bis, 10, 29-ter, 29-quater, 29-sexies, 29-septies, 29-octies, 29-nonies, 29-decies, 29-terdecies (INCITE), Allegato VIII; nuovo Titolo III-ter e Allegato VIII-bis; abrogazione dell'Allegato X; regime transitorio (art. 43).
- **Richiamati** (non riprodotti): **Allegato XII**, **conclusioni sulle BAT/BREF**, artt. **5** (definizioni), **6** (c. 12-16), **29-bis**, **29-quinquies**, **29-septies** (BAT e norme di qualità), **29-nonies** (modifiche/variazione gestore), **29-quattuordecies** (sanzioni).

Dettaglio in `references/sources.yaml`, `references/fonti/dlgs-152-2006-aia-titolo3bis.md` (testo previgente), `references/fonti/dlgs-197-2026-ied2.md` (novelle IED2), `references/estratti/aia-checklist.md`.

## Avvertenza

Skill di **supporto documentale**: la **redazione della domanda/AIA**, l'**individuazione delle BAT** e la gestione del procedimento e dei controlli restano responsabilità del **gestore**, dell'**autorità competente** e di **ISPRA/ARPA**, sul testo vigente del Titolo III-bis del D.Lgs. 152/2006 come modificato dal D.Lgs. 197/2026. La skill **non sostituisce** tali soggetti né la lettura degli articoli e degli allegati richiamati.
