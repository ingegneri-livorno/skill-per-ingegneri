# CHANGELOG - accertamento-conformita-sanatoria-dpr380

Il formato e' basato su [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).
Versioning: [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.2.0-alpha] - 2026-11-15

### Added (refs #523)
- Fonte scaricata, hashata e letta (Regola zero): **GU Serie Generale n. 263 dell'11/11/2026** (PDF integrale del fascicolo), SHA256 12e7d5893462c1ec18f16a6a27c6666b540df2b157b4e82f288f0a64c337e8b3, contenente il **D.L. 11 novembre 2026, n. 205** "Piano straordinario per i Campi Flegrei" (cod. red. 26G00225, in vigore dal 12/11/2026, da convertire in legge). Trascrizione in `references/fonti/dl-205-2026-gu-263.md` (identica a quella delle altre skill che citano il decreto).

### Changed
- `SKILL.md`: nuova sezione "Zona dei Campi Flegrei: regime speciale D.L. 205/2026 - stato al 15 novembre 2026" - art. 13: per gli interventi realizzati prima del 1/8/2026 sugli immobili oggetto di contributo, art. 1-sexies D.L. 55/2018, PdC e SCIA in sanatoria con provvedimento espresso entro 60 giorni, una sola richiesta di integrazioni entro 15 giorni, condoni pendenti entro 90 giorni, oneri a carico dell'interessato, salva-casa fatto salvo ove piu' favorevole, conformita' sismica alla realizzazione e al rilascio; art. 12 c. 8 e art. 13 c. 6 sul rapporto con il contributo. Nuovo `normative_refs`; version 0.1.0-alpha -> 0.2.0-alpha.
- `references/sources.yaml`: nuova fonte `dl-205-2026-gu-263`; `last_verified` -> 2026-11-15.
- `README.md`: fonte aggiunta all'elenco.

## [0.1.0-alpha] - 2026-07-17

### Added (closes #364)
- Prima versione della skill di supporto al **progettista** e al **tecnico incaricato** per
  l'**accertamento di conformita' / sanatoria edilizia**, ai sensi del **D.P.R. 6 giugno 2001, n. 380,
  Titolo IV, artt. 36, 36-bis e 37** (salva-casa 2024), nell'area `edilizia-urbanistica-catasto`.
- Fonte scaricata, hashata e letta (Regola zero):
  - **DPR 380/2001** - indice Normattiva pinnato `!vig=2026-07-17` SHA256:
    bac3f7b170cfd122936873c835b3f728e7880d058bd98ad45f55b94ba89a632f (codice 001G0429, idGruppo 9).
    Art. 36 (idSottoArticolo 1, v6), 36-bis (idSottoArticolo 2, v2), 37 (v5) via `caricaArticolo` (AKN).
  - Trascrizione verbatim in `references/fonti/dpr-380-2001-36-36bis-37.md`.
- Estratto operativo `references/estratti/accertamento-conformita-checklist.md` con tabella articolo/
  doppia conformita'.
- Due task: `inquadra-articolo-doppia-conformita.md` e `inquadra-procedura-oblazione-termini.md`.
- Due esempi: veranda in parziale difformita' (art. 36-bis, doppia conformita' attenuata); ampliamento in
  assenza di titolo (art. 36, doppia conformita' piena e non ammissibilita' se non conforme all'epoca).

### Contenuto ancorato al testo
- Art. 36 - assenza di titolo/totale difformita', doppia conformita' piena, oblazione contributo doppio,
  60 giorni silenzio-rifiuto; art. 36-bis (introdotto dal salva-casa) - parziale difformita'/variazioni
  essenziali, doppia conformita' attenuata, dichiarazione del professionista abilitato e prova
  dell'epoca (art. 9-bis c. 1-bis), profili sismici (3-bis) e paesaggistici (4, 5-bis, art. 167 D.Lgs.
  42/2004), oblazione (5), 45 giorni silenzio-assenso (6); art. 37 - assenza/difformita' dalla SCIA con
  sanzione pari al triplo dell'aumento del valore venale (min 1.032 euro) e rinvio all'accertamento
  dell'art. 36-bis.

### Scope e limiti
- Non redige la domanda ne' la dichiarazione di conformita', non qualifica in concreto l'abuso, non
  calcola l'oblazione ne' il valore venale, non tratta il condono (leggi speciali). Non sostituisce il
  progettista, lo sportello unico per l'edilizia ne' gli enti competenti.

### Note di sviluppo
- Distinta da `vigilanza-sanzioni-abusi-edilizi-dpr380` (che esclude la sanatoria). Modifiche dal DL
  69/2024 conv. L. 105/2024 (salva-casa): rileggere periodicamente artt. 36/36-bis/37 sull'indice
  pinnato aggiornato. Validazione Livello 2 con tecnico edilizio/esperto di sanatorie.
