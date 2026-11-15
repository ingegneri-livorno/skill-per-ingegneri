# CHANGELOG - rup-responsabile-unico-progetto-dlgs36

Il formato e' basato su [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).
Versioning: [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.2.0-alpha] - 2026-11-15

### Added (closes #523)
- Fonte scaricata, hashata e letta (Regola zero): **GU Serie Generale n. 263 dell'11/11/2026** (PDF integrale del fascicolo), SHA256 12e7d5893462c1ec18f16a6a27c6666b540df2b157b4e82f288f0a64c337e8b3, contenente il **D.L. 11 novembre 2026, n. 205** "Piano straordinario per i Campi Flegrei" (cod. red. 26G00225, in vigore dal 12/11/2026, da convertire in legge). Trascrizione in `references/fonti/dl-205-2026-gu-263.md`.

### Changed
- `SKILL.md`: nuova sezione "Zona dei Campi Flegrei: regime speciale D.L. 205/2026 - stato al 15 novembre 2026" - art. 10: Conferenza di servizi permanente presieduta dal Commissario, che sostituisce pareri e atti di assenso, ha effetto di variante urbanistica e approva i progetti pubblici ai sensi dell'art. 38 D.Lgs. 36/2023 (c. 3 lett. b-c); avvertenza su decreto-legge in attesa di conversione e su ordinanze del Commissario (art. 10 c. 3 lett. d) per le procedure dei lavori privati. Nuovo `normative_refs`; version 0.1.0-alpha -> 0.2.0-alpha.
- `references/sources.yaml`: nuova fonte `dl-205-2026-gu-263`; `last_verified` -> 2026-11-15.
- `README.md`: fonte aggiunta all'elenco.

## [0.1.0-alpha] - 2026-07-17

### Added (closes #319)
- Prima versione della skill di supporto documentale all'inquadramento del
  Responsabile unico del progetto (RUP) nei contratti pubblici, art. 15 del D.Lgs.
  36/2023 (Codice dei contratti pubblici).
- Fonte scaricata, hashata e letta (Regola zero):
  - D.Lgs. 31/3/2023 n. 36 - testo multivigente su Normattiva, pagina indice pinnata
    `!vig=2026-07-17` SHA256:
    0e9a193836e379cb33cb6daf1a5a988c608eb9559d84b91a841d9ed9791a62af
    (riproducibile, doppio download; codice redazionale 23G00044, stesso indice
    delle altre skill D.Lgs. 36). Art. 15 (versione 2, idGruppo 2) letto via AJAX
    (caricaArticolo) e trascritto verbatim in
    `references/fonti/dlgs-36-2023-art15.md`: nomina (c. 1), soggetto/requisiti
    allegato I.2, obbligatorieta' e subentro ex lege (c. 2), nominativo nel bando
    (c. 3), unicita' e modelli organizzativi (c. 4), compiti (c. 5), struttura di
    supporto e risorse 1% (c. 6), formazione (c. 7), incompatibilita' nel contraente
    generale/PPP (c. 8), centrali di committenza (c. 9).
- Estratto operativo `references/estratti/rup-checklist.md` con nomina, requisiti,
  unicita'/modelli, compiti, struttura di supporto, formazione, incompatibilita' e
  centrali di committenza.
- Due task: `inquadra-nomina-rup.md` (nomina, soggetto, requisiti, unicita') e
  `verifica-compiti-incompatibilita.md` (compiti, struttura di supporto, formazione,
  divieto di cumulo, centrali di committenza).
- Due esempi: nomina del RUP con modello organizzativo (responsabili di procedimento
  per fase) e incompatibilita' nel contraente generale/PPP.

### Nota di source-grounding (#319)
La skill e' source-grounded sul **testo vigente dell'art. 15 del D.Lgs. 36/2023 letto
da Normattiva** (fonte ufficiale). L'**allegato I.2** (requisiti di professionalita'
ed elenco dei compiti del RUP), richiamato ai commi 2 e 5, e' **citato come rinvio e
non riprodotto**. E' citato l'**art. 37** (programmazione). Il testo tra doppi tondi
`(( ))` e l'indicazione del periodo soppresso (D.Lgs. 209/2024) sono riportati come
da fonte.

### Note di sviluppo
- Testo multivigente: ad ogni aggiornamento ri-pinnare la URL Normattiva e rileggere
  l'articolo se modificato.
- Validazione Livello 2 da effettuare con esperto di contratti pubblici/RUP.
- Possibili estensioni future: trascrizione mirata dell'allegato I.2 (requisiti e
  compiti del RUP) e raccordo con le skill sulle fasi (programmazione art. 37,
  subappalto art. 119, garanzie artt. 106/117, varianti art. 120, collaudo art. 116).
