# CHANGELOG - rsia-audit-stradale-dlgs35

Tutte le modifiche significative alla skill sono documentate qui.

Il formato e' basato su [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
e questa skill aderisce a [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.2.0-alpha] - 2026-10-25

### Changed (closes #514)
- Recepito il D.M. MIT 11 settembre 2026 sui dispositivi di sicurezza stradale per i motociclisti (DSM) (GU SG n. 243 del 19/10/2026, in vigore centottanta giorni dopo la pubblicazione, art. 7 c. 3), che da quella data abroga il D.M. 1 aprile 2019 prot. n. 121 (art. 7 c. 2), come riferimento tecnico:
  - `tasks/draft-rsa.md`, Allegato II punto 2 lett. f): verifiche su ambito >= 70 km/h (art. 1 c. 1), zone da proteggere (art. 4 c. 2), estensione (art. 4 c. 5), allegato progettuale (art. 4 c. 1), mancata installazione e deroga (art. 4 cc. 3, 6), conformita' UNI CEN/TS 17342 o previgente TS 1317-8 (artt. 2, 3, 5 c. 4), scelta del decreto applicabile: D.M. 2019 fino all'entrata in vigore del D.M. 2026 e, dopo, per i lavori con affidamento in corso o PFTE approvato (art. 7 cc. 1, 3);
  - `tasks/draft-nsa.md`, Allegato III componente 6: valutazione del rischio dell'ente sulle barriere in esercizio nelle zone dell'art. 4 c. 2 (art. 5 cc. 1-2).
- Scarto rispetto alla scheda #514: il decreto non contiene un elenco di tipologie approvate (requisiti prestazionali UNI CEN/TS 17342 e dichiarazione del fabbricante, art. 2) ne' requisiti di manutenzione periodica dei DSM (solo la deroga dell'art. 4 c. 6); non cita RSA, NSA o ispezioni del D.Lgs 35/2011, richiamato solo nel preambolo.

### Added
- Fonti `dm-mit-11-9-2026-dsm-gu243` e `dm-mit-1-4-2019-dsm-gu114` in `references/sources.yaml` (SHA256 dei PDF GU), trascrizioni `references/fonti/dm-mit-11-9-2026-dsm.md` e `references/fonti/dm-mit-1-4-2019-dsm.md`, estratto `references/estratti/dm-mit-11-9-2026-dsm.md` (con sezione sul quale decreto applicare e sul regime previgente).

## [0.1.0-alpha] - 2026-05-15

### Added
- Prima versione alpha della skill, copertura delle quattro procedure del D.Lgs 35/2011 modificato dal D.Lgs 213/2021.
- `SKILL.md` con frontmatter dual-agent (Claude Code + Codex), descrizione, disclaimer, processo generale e rinvii a `tasks/`.
- Cinque task files: `check-ambito-applicazione.md`, `draft-viss.md`, `draft-rsa.md`, `draft-nsa.md`, `verifica-requisiti-controllore.md`.
- Fonti normative: `references/sources.yaml` (D.Lgs 35/2011, D.Lgs 213/2021, Dir. 2008/96/CE - tre fonti scaricate e verificate via SHA256; Dir. (UE) 2019/1936 come riferimento strutturale).
- Estratti testuali per articolo, comma e allegato in `references/estratti/dlgs-35-2011.md`, `references/estratti/dlgs-213-2021.md`, `references/estratti/dir-2008-96-ce.md`.
- Esempi: `01-rsa-pfte-conforme` (caso conforme: autostrada TEN-T 18 km, controllore qualificato, galleria correttamente esclusa) e `02-rsa-controllore-non-idoneo` (caso problematico: incompatibilita' del controllore per partecipazione pregressa alla progettazione preliminare, mancanza dei requisiti formali, regime transitorio non applicabile).
- `AGENTS.md` di skill con convenzioni di dominio (articoli chiave, anti-pattern: niente citazione del vecchio art. 5 o vecchio Allegato III sostituiti dal D.Lgs 213/2021).

### Note di sviluppo
- Skill non ancora validata da dominio terzo. Validazione di Livello 1 effettuata dall'autore (Claude Opus 4.7).
- Da considerare draft finche' non passa validazione di Livello 2 (vedi `methodology/validazione.md`).
- Validatore di Livello 2 da identificare: controllore della sicurezza stradale iscritto all'elenco MIMS.
- Direttiva (UE) 2019/1936 inserita come riferimento strutturale solo: i contenuti sostanziali sono applicati attraverso il D.Lgs 213/2021 di recepimento, che e' la fonte vincolante nell'ordinamento italiano.
