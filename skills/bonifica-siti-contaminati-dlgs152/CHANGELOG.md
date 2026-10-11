# CHANGELOG - bonifica-siti-contaminati-dlgs152

Il formato e' basato su [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).
Versioning: [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.2.0-alpha] - 2026-10-11

### Changed (closes #507)
- Recepito il D.L. 8/10/2026 n. 177 (GU SG n. 234 dell'8/10/2026, in vigore dal
  9/10/2026, da convertire in legge), art. 5:
  - art. 244 c. 3: ordinanza della provincia entro 150 giorni dalla comunicazione
    del c. 1; nuovo c. 4-ter: la regione assegna alla provincia fino a 30 giorni,
    poi adotta l'ordinanza con il supporto SNPA;
  - art. 252 c. 3 (aree marine dei SIN) e All. 5 Tab. 2 METALLI (soppresse la
    decima e la sedicesima riga): segnalati come richiami, la skill non riproduce
    i valori CSC;
  - art. 5 c. 2: semplificazioni siti orfani (art. 6 c. 1 D.L. 153/2024) estese
    agli interventi di bonifica finanziati dai Fondi ex L. 178/2020 art. 1 c. 177
    e L. 147/2013 art. 1 c. 6;
  - art. 4 c. 1 lett. b: art. 185-ter c. 3 (terre e rocce da siti in bonifica).
- Scarto rispetto alla scheda #507: il testo non usa "perentorio" ne' "FSC" e non
  detta norme transitorie; il D.L. non modifica gli artt. 242, 245, 250.

### Added
- Fonti `dl-177-2026-gu234` e `dl-153-2024-gu244` in `references/sources.yaml`
  (SHA256 dei PDF GU) e trascrizioni `references/fonti/dl-177-2026.md`,
  `references/fonti/dl-153-2024-art6.md`.

## [0.1.0-alpha] - 2026-07-14

### Added (closes #62)
- Prima versione della skill di supporto documentale alla procedura di bonifica
  dei siti contaminati (Parte quarta Titolo V del D.Lgs. 152/2006).
- Fonte scaricata, hashata e letta (Regola zero):
  - D.Lgs. 3/4/2006 n. 152 - testo multivigente su Normattiva, pagina indice
    pinnata `!vig=2026-07-14` SHA256:
    af54f5e0c6fa3d0a6d3dc5cf6d33ece0be7969be086dd93a24980e11b053b9fe
    (riproducibile, doppio download; pattern della skill aua-dpr59-dossier).
    Articoli 240 (v. 2, definizioni CSC/CSR), 242 (v. 11, procedure operative),
    244 (v. 3, ordinanze PA), 249 (aree ridotte) e 257 (v. 2, sanzioni) letti via
    AJAX (caricaArticolo) e trascritti verbatim in
    `references/fonti/dlgs-152-2006.md`.
- Estratto operativo `references/estratti/bonifica-siti-checklist.md` con
  definizioni, procedura, termini, attori, iniziativa PA e sanzioni.
- Due task: `diagnosi-procedura.md` (step dell'art. 242, termini e attori) e
  `checklist-adempimenti.md` (completezza e sanzioni art. 257).
- Due esempi: sversamento con indagine sotto CSC (chiusura con
  autocertificazione) e superamento CSC in area dismessa (procedura piena).

### Nota di source-grounding (#62)
La scheda #62 citava il D.Lgs. 152/06 Tit. V tramite `bosettiegatti` (host non
ufficiale) e le linee guida ISPRA. La skill e' source-grounded sul **testo
vigente del D.Lgs. 152/2006 letto da Normattiva** (fonte ufficiale, TUA
fortemente emendato), con la pagina indice pinnata a data di vigenza per hash
riproducibile e la trascrizione verbatim degli artt. 240, 242, 244, 249, 257
(versioni vigenti). I **valori CSC** (Allegato 5), i **criteri di analisi di
rischio** (Allegato 1), il **piano di caratterizzazione** (Allegato 2) e le
**procedure semplificate** (Allegato 4) non sono riprodotti: il perimetro
distingue cio' che e' negli articoli (definizioni, procedura, termini, attori,
sanzioni) da cio' che richiede la lettura degli allegati e l'analisi tecnica.

### Note di sviluppo
- Testo multivigente: ad ogni aggiornamento ri-pinnare la URL Normattiva e
  rileggere gli articoli modificati (usare le versioni piu' alte: art. 242 v. 11,
  art. 244 v. 3, art. 240/257 v. 2 al 2026-07-14).
- Validazione Livello 2 da effettuare con tecnico ambientale/geologo.
- Possibili estensioni future: trattazione dei SIN (art. 252), degli oneri reali
  e privilegi (artt. 250, 253) e trascrizione mirata dell'Allegato 4 (procedure
  semplificate per aree di ridotte dimensioni).
