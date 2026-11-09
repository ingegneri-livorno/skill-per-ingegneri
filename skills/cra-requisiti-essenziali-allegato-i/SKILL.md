---
name: cra-requisiti-essenziali-allegato-i
description: |-
  Gap analysis di un prodotto con elementi digitali (PDE) rispetto ai requisiti essenziali di cibersicurezza dell'allegato I del Regolamento (UE) 2024/2847 (Cyber Resilience Act) e agli obblighi del fabbricante dell'art. 13: valutazione dei rischi, requisiti di prodotto (parte I, lettere a-m), processi di gestione delle vulnerabilita' (parte II, SBOM, CVD, aggiornamenti), periodo di assistenza, informazioni all'utilizzatore (allegato II). Use when an engineer, product security engineer or compliance manager designing or maintaining hardware or software sold in the EU must check what the CRA requires of the product and of the manufacturer's processes before 11 December 2027, find the gaps, and know which evidence goes into the Annex VII technical documentation. Does not classify the product or pick the conformity assessment module (use cra-classificazione-pde) and does not handle art. 14 incident reporting (use cra-segnalazione-art14).
license: MIT
area: software-dati-cybersecurity
title: "CRA - Requisiti essenziali (allegato I) e obblighi del fabbricante"
summary: "Gap analysis di un prodotto con elementi digitali rispetto ai requisiti essenziali dell'allegato I del CRA (Reg. UE 2024/2847) e agli obblighi dell'art. 13: valutazione dei rischi, requisiti di prodotto, gestione vulnerabilita', SBOM, periodo di assistenza, istruzioni."
normative_refs:
  - "Reg. UE 2024/2847 (Cyber Resilience Act) allegato I parti I e II"
  - "Reg. UE 2024/2847 artt. 6, 13, 21, 27, 31, 64, 69, 71"
  - "Reg. UE 2024/2847 allegati II e VII"
version: 0.1.0-alpha
status: alpha
tags:
  - cra
  - reg-ue-2024-2847
  - cyber
  - security-by-design
  - sbom
  - vulnerability-management
---

# CRA - Requisiti essenziali di cibersicurezza (allegato I) e obblighi del fabbricante

## Quando usare questa skill

Quando un **fabbricante di un prodotto con elementi digitali (PDE)** - in pratica l'ingegnere di prodotto, firmware o software, il security engineer, il responsabile tecnico o il compliance manager - deve capire **cosa il CRA chiede al prodotto e ai suoi processi** e **dove sono le lacune**, prima dell'**11 dicembre 2027**, data da cui si applicano i requisiti essenziali e l'art. 13 (art. 71, par. 2).

Casi tipici:

- si progetta un prodotto connesso (dispositivo IoT, gateway, app, software installabile, firmware) che sara' immesso sul mercato UE dopo l'11 dicembre 2027 e serve una **gap analysis** sui requisiti dell'allegato I;
- serve impostare la **valutazione dei rischi di cibersicurezza** dell'art. 13, che decide quali requisiti della parte I si applicano e come;
- serve verificare i **processi di gestione delle vulnerabilita'** (SBOM, politica CVD, aggiornamenti di sicurezza, periodo di assistenza);
- serve controllare le **informazioni e istruzioni per l'utilizzatore** dell'allegato II.

Quando **non** usarla:

- Verificare se il prodotto rientra nel CRA, classificarlo e scegliere il modulo di valutazione della conformita': usa `cra-classificazione-pde`.
- Gestire una vulnerabilita' attivamente sfruttata o un incidente grave (art. 14, gia' applicabile dall'11 settembre 2026): usa `cra-segnalazione-art14`.
- Obblighi dell'organizzazione ai sensi della normativa NIS2: usa `nis2-self-assessment`. Questa skill riguarda il **prodotto** e i processi del fabbricante che lo riguardano.
- Progettazione di dettaglio dei controlli (scelta di algoritmi, architettura di autenticazione, penetration test): la skill dice cosa il testo richiede e quali evidenze servono, non progetta la soluzione.

## Avvertenza

Questa skill e' uno strumento di supporto alla verifica di documenti tecnici e processi. **Non sostituisce il giudizio del professionista che firma la valutazione ne' quello del fabbricante, che resta l'unico responsabile della dichiarazione di conformita' UE.** L'utilizzo improprio degli output e' responsabilita' esclusiva dell'utente. La skill non produce documenti pronti alla firma, non rilascia attestazioni di conformita' e non sostituisce le prove richieste dall'allegato VII, punto 6.

Tre limiti di contesto da ricordare a ogni uso:

1. **Norme armonizzate**: la skill non sa quali siano pubblicate in GU UE alla data d'uso. Verificarlo prima di contare sulla presunzione di conformita' dell'art. 27.
2. **Atti della Commissione** su formato SBOM (art. 13, par. 24) e periodi minimi di assistenza per categoria (art. 13, par. 8): non letti.
3. **Disciplina italiana**: le norme sanzionatorie sono fissate dagli Stati membri (art. 64, par. 1). Nessun atto nazionale di adeguamento al CRA e' fra le fonti lette.

## Sotto-attivita' disponibili

In base alla richiesta dell'utente, carica il file appropriato da `tasks/`:

- **Impostare la valutazione dei rischi di cibersicurezza** (art. 13, par. 2-4): quando l'utente deve redigerla o verificarla, o non sa quali requisiti della parte I si applicano, leggere `tasks/imposta-valutazione-rischi.md`.
- **Gap analysis sui requisiti di prodotto** (allegato I, parte I): quando l'utente descrive il prodotto e chiede cosa manca, leggere `tasks/gap-analysis-parte-i.md`.
- **Gap analysis sui processi di gestione delle vulnerabilita'** (allegato I, parte II; art. 13, par. 5-11 e 19): SBOM, CVD, aggiornamenti, periodo di assistenza; leggere `tasks/gap-analysis-parte-ii.md`.
- **Verificare informazioni e istruzioni per l'utilizzatore** (allegato II; art. 13, par. 15-20): leggere `tasks/check-informazioni-utilizzatore.md`.

Per una gap analysis completa esegui i task nell'ordine: valutazione dei rischi, parte I, parte II, informazioni utilizzatore. Se la richiesta non e' chiara, chiedi all'utente quale sotto-attivita' desidera.

## Processo generale

1. Verifica le **precondizioni**: il prodotto e' un PDE in ambito CRA e il richiedente e' il fabbricante, anche come importatore o distributore che usa il proprio marchio (art. 3, punti 1 e 13; art. 21)? Se l'ambito non e' accertato, rinvia a `cra-classificazione-pde` prima di continuare.
2. Verifica le **date**: i requisiti si applicano a ogni singolo esemplare immesso sul mercato dall'11 dicembre 2027, anche se il modello era gia' in vendita prima (considerando 38). Gli esemplari immessi prima di quella data sono soggetti solo in caso di modifica sostanziale successiva (art. 69, par. 2). Non concludere che un modello lanciato prima del 2027 sia esente.
3. Carica il task e raccogli gli input. Non assumere caratteristiche del prodotto che l'utente non ha descritto: chiedile.
4. Per ogni requisito registra uno stato fra **soddisfatto / parziale / mancante / non applicabile (con giustificazione) / da verificare**, la citazione esatta (allegato, parte, punto, lettera) e l'evidenza che finira' nell'allegato VII.
5. Distingui sempre cio' che il testo **impone**, cio' che e' **condizionato** ("ove applicabile", "se del caso", "ove tecnicamente fattibile") e cio' su cui il testo **tace**.
6. Chiudi con l'elenco delle lacune in ordine di priorita' e il rinvio al professionista e al fabbricante.

## Regola di prudenza sulla non applicabilita'

Solo i requisiti della **parte I, punto 2** sono subordinati alla valutazione dei rischi ("ove applicabile"). Per la parte I, punto 1, e per la parte II la valutazione dei rischi ne indica le modalita', non l'applicabilita' (art. 13, par. 3). Qualsiasi requisito non applicabile richiede comunque una chiara giustificazione nella documentazione tecnica (art. 13, par. 4). La skill quindi:

- per la parte II non usa la valutazione dei rischi come filtro: accetta "non applicabile" solo se poggia sulla formulazione del singolo punto (per esempio "ove applicabile" nel punto 7, "ove tecnicamente fattibile" nel punto 2) e ha la giustificazione dell'art. 13, par. 4; mai su prezzo, dimensione del fabbricante o assenza di sviluppo interno;
- accetta "non applicabile" per una lettera della parte I, punto 2, solo con una giustificazione legata alla valutazione dei rischi, da riportare nella documentazione tecnica (art. 13, par. 4);
- in caso di dubbio classifica il requisito come **da verificare**, non come soddisfatto.

## Fonti normative

- **Reg. (UE) 2024/2847 (CRA)**: considerando 38, art. 3 (punti 1, 2, 6, 13, 20-25, 30, 37-41, 48), art. 6, **art. 13** (integrale), art. 21, art. 27 (par. 1 e 8), art. 31, art. 64 (par. 1-4), art. 69, art. 71, **allegato I** (parti I e II), **allegato II**, allegato VII.

Trascrizione verbatim in `references/fonti/reg-ue-2024-2847-cra-requisiti-essenziali.md`, estratto operativo in `references/estratti/cra-allegato-i-requisiti-e-obblighi.md`, riferimenti con SHA256 in `references/sources.yaml`.

## Limiti

Cosa questa skill NON fa:

- Non verifica l'ambito di applicazione ne' classifica il prodotto (usa `cra-classificazione-pde`).
- Non sceglie ne' esegue la procedura di valutazione della conformita' e non redige la dichiarazione di conformita' UE.
- Non fissa parametri tecnici (algoritmi, tempi di patch, soglie CVSS): il testo non li contiene.
- Non indica quali norme armonizzate applicare ne' se siano pubblicate.
- Non copre gli obblighi propri di importatori, distributori e gestori di software open source (artt. 18-20 e 22-26, non letti); dell'art. 21 usa solo la regola che li rende fabbricanti.
- Non copre la segnalazione dell'art. 14 (usa `cra-segnalazione-art14`).
- Non tratta il rapporto con il regolamento sull'IA per i sistemi ad alto rischio (art. 12, non letto).
- Non applica atti nazionali italiani di adeguamento al CRA: nessuno e' fra le fonti lette.
