# CHANGELOG - permesso-costruire-dpr380

Il formato e' basato su [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).
Versioning: [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.2.0-alpha] - 2026-11-15

### Added (closes #523)
- Fonte scaricata, hashata e letta (Regola zero): **GU Serie Generale n. 263 dell'11/11/2026** (PDF integrale del fascicolo), SHA256 12e7d5893462c1ec18f16a6a27c6666b540df2b157b4e82f288f0a64c337e8b3, contenente il **D.L. 11 novembre 2026, n. 205** "Piano straordinario per i Campi Flegrei" (cod. red. 26G00225, in vigore dal 12/11/2026, da convertire in legge). Trascrizione in `references/fonti/dl-205-2026-gu-263.md`.

### Changed
- `SKILL.md`: nuova sezione "Zona dei Campi Flegrei: regime speciale D.L. 205/2026 - stato al 15 novembre 2026" - art. 9: nella zona di intervento gli strumenti urbanistici comunali prevedono consumo di suolo da nuova costruzione o ristrutturazione edilizia (art. 3 c. 1 lett. d-e DPR 380) solo in casi eccezionali e previa dimostrazione dell'insostenibilita' tecnica ed economica di riqualificare o rigenerare aree gia' edificate; art. 13: per gli interventi realizzati prima del 1/8/2026 sugli immobili oggetto di contributo, art. 1-sexies D.L. 55/2018, PdC e SCIA in sanatoria entro 60 giorni, una sola richiesta di integrazioni entro 15 giorni, condoni pendenti definiti con priorita' entro 90 giorni; avvertenza su decreto-legge in attesa di conversione e su ordinanze del Commissario (art. 10 c. 3 lett. d) per le procedure dei lavori privati. Nuovo `normative_refs`; version 0.1.0-alpha -> 0.2.0-alpha.
- `SKILL.md`: sezione Campi Flegrei estesa all'**art. 12** (domanda di contributo con la richiesta del titolo; il Comune rilascia il titolo ex art. 20 o verifica SCIA artt. 22-23; progetto unitario e stato legittimo riferito all'edificio; contributo solo con titolo, sanatoria o casi dell'art. 13); il punto sulle ordinanze ora distingue cio' che il decreto dispone direttamente (artt. 12-13) da cio' che e' rinviato alle ordinanze.
- `references/fonti/dl-205-2026-gu-263.md`: aggiunto l'art. 12 trascritto integralmente (identico in tutte le skill che citano il decreto).
- `references/sources.yaml`: nuova fonte `dl-205-2026-gu-263`; `last_verified` -> 2026-11-15.
- `README.md`: fonte aggiunta all'elenco.

## [0.1.0-alpha] - 2026-07-17

### Added (closes #303)
- Prima versione della skill di supporto al regime del **permesso di costruire**
  (caratteristiche, presupposti, procedimento, efficacia e decadenza), ai sensi del
  **D.P.R. 380/2001, artt. 11, 12, 15, 20**, nell'area `edilizia-urbanistica-catasto`.
- Fonte scaricata, hashata e letta (Regola zero):
  - **D.P.R. 6/6/2001 n. 380** - indice Normattiva pinnato `!vig=2026-07-17`
    SHA256: bac3f7b170cfd122936873c835b3f728e7880d058bd98ad45f55b94ba89a632f
    (codice 001G0429). Artt. 11, 12, 15 (idGruppo 3), 20 (idGruppo 5),
    flagTipoArticolo 0, via `caricaArticolo`.
  - Trascrizione verbatim in `references/fonti/dpr-380-2001-permesso.md`.
- Estratto operativo `references/estratti/permesso-costruire-checklist.md`.
- Due task: `inquadra-presupposti-caratteristiche.md` e
  `verifica-procedimento-termini-decadenza.md`.
- Due esempi: presupposti e caratteristiche del titolo (artt. 11-12); termini,
  silenzio-assenso e decadenza (artt. 20, 15).

### Contenuto ancorato al testo
- Art. 11 caratteristiche (legittimazione, trasferibilita', irrevocabilita',
  onerosita' art. 16, diritti dei terzi); art. 12 presupposti (conformita'
  urbanistica, urbanizzazione primaria esistente/prevista/impegno, misure di
  salvaguardia); art. 15 efficacia temporale (inizio 1 anno, ultimazione 3 anni),
  decadenza, proroga, nuovo permesso per la parte non ultimata, decadenza per
  contrastanti previsioni; art. 20 procedimento (SUE, asseverazione, responsabile,
  termini 60/30 gg, interruzione/sospensione, conferenza di servizi, silenzio-assenso
  e vincoli, sanzioni per false attestazioni).

### Scope e limiti
- Non decide il titolo (PdC vs SCIA/CILA - art. 10), non redige domanda/asseverazione,
  non calcola il contributo (art. 16), non tratta agibilita' (art. 24) ne'
  vigilanza/sanzioni (artt. 27 ss.), non sostituisce il progettista, il SUE o il
  Comune. Artt. 10, 13, 16, 22, 24 e la L. 241/1990 citati e non trascritti.

### Note di sviluppo
- Normattiva: ad ogni aggiornamento riscaricare l'indice del DPR 380/2001 pinnato
  (nuovo hash) e rileggere gli artt. 11, 12, 15, 20 (testo tra `(( ))`, es. Salva Casa
  DL 69/2024 conv. L. 105/2024).
- Validazione Livello 2 con tecnico SUE / esperto di diritto urbanistico.
