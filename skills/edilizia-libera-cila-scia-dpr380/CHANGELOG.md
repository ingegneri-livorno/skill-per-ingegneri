# CHANGELOG - edilizia-libera-cila-scia-dpr380

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

### Added (closes #325)
- Prima versione della skill di supporto documentale ai regimi del titolo edilizio
  diversi dal permesso di costruire (edilizia libera, CILA, SCIA, SCIA in alternativa al
  PdC), Titolo II del DPR 380/2001.
- Fonte scaricata, hashata e letta (Regola zero):
  - D.P.R. 6/6/2001 n. 380 - testo su Normattiva, pagina indice pinnata `!vig=2026-07-17`
    SHA256: bac3f7b170cfd122936873c835b3f728e7880d058bd98ad45f55b94ba89a632f
    (riproducibile, doppio download; codice redazionale 001G0429, stesso indice delle
    altre skill DPR 380). Artt. 6 (attività edilizia libera), 6-bis (CILA), 22 (SCIA) e 23
    (SCIA in alternativa al permesso di costruire) letti via AJAX (caricaArticolo, idGruppo
    2 per 6/6-bis, idGruppo 6 per 22/23) e trascritti verbatim in
    `references/fonti/dpr-380-2001-6-6bis-22-23.md` (incluse lettere/commi abrogati e
    aggiornamenti 29, 66, 69).
- Estratto operativo `references/estratti/titoli-edilizi-checklist.md` con edilizia libera,
  CILA, SCIA, SCIA alternativa e una sintesi decisionale.
- Due task: `scegli-titolo-edilizio.md` (scelta del regime dalla categoria art. 3) e
  `imposta-scia-alternativa.md` (adempimenti SCIA/SCIA alternativa: relazione, termini,
  contributo, efficacia, collaudo).
- Due esempi: CILA vs SCIA per manutenzione straordinaria (discrimine parti strutturali);
  edilizia libera (serra mobile, vasca acque meteoriche) e SCIA alternativa al PdC in
  attuazione di piano attuativo.

### Nota di source-grounding (#325)
La skill e' source-grounded sul **testo vigente degli artt. 6, 6-bis, 22, 23 del DPR
380/2001 letto da Normattiva** (fonte ufficiale). La **qualificazione dell'intervento**
(art. 3) e il **permesso di costruire** (art. 10, 20) sono coperti da skill dedicate
(`definizioni-interventi-edilizi-dpr380`, `permesso-costruire-dpr380`) e qui citati come
rinvio. Il **glossario dell'edilizia libera** (DM 2/3/2018) e la **modulistica unificata**
(skill `modulistica-edilizia-unificata`) non sono riprodotti. Gli artt. 16, 37, 44 e
l'art. 19 della L. 241/1990 sono citati. Il testo tra doppi tondi `(( ))` e le note di
abrogazione sono riportati come da fonte.

### Note di sviluppo
- Testo multivigente: ad ogni aggiornamento ri-pinnare la URL Normattiva e rileggere gli
  articoli modificati (il DPR 380 è oggetto di frequenti correttivi, es. D.Lgs. 190/2024,
  D.Lgs. 178/2025).
- Validazione Livello 2 da effettuare con tecnico abilitato/esperto edilizia.
- Possibili estensioni future: raccordo con la disciplina sanzionatoria (artt. 37, 44,
  skill `vigilanza-sanzioni-abusi-edilizi-dpr380`) e con la modulistica regionale.
