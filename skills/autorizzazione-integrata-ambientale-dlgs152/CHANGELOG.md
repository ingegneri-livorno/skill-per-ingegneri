# CHANGELOG - autorizzazione-integrata-ambientale-dlgs152

Il formato e' basato su [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).
Versioning: [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.2.0-alpha] - 2026-11-01

### Changed (closes #517)
- Aggiornamento al **D.Lgs. 28 settembre 2026, n. 197** (GU SG n. 251 del 28-10-2026, codice 26G00213, **in vigore dal 12/11/2026**), recepimento della Dir. (UE) 2024/1785 (IED2), che modifica il D.Lgs. 152/2006 (Capo I, artt. 1-42).
- Nuova fonte scaricata, hashata e letta (Regola zero): fascicolo PDF GU SG n. 251 del 28-10-2026, SHA256 d4fd3721ccdf315a77119215ce1a976fe4b052238e71100b6f5948230fa2fe52; trascrizione verbatim degli articoli usati in `references/fonti/dlgs-197-2026-ied2.md`.
- `SKILL.md`: nuove sezioni su entrata in vigore e regime transitorio (art. 43), campo di applicazione (Allegato VIII ampliato, Allegato VIII-bis/Titolo III-ter, abrogazione Allegato X), Commissione AIA-IPPC (art. 8-bis: 23 esperti + 5 del Ministero della salute); aggiornate domanda (art. 29-ter: acqua, odori, salute umana, tariffa; inoltro 10 gg, osservazioni 20 gg, integrazioni una sola volta), procedura (art. 29-quater: conferenza decisoria, Ministero della salute e parere ISS per l'AIA statale, abrogazione c. 7), contenuto (art. 29-sexies: BAT-AEPL, SGA, piano di trasformazione, controlli 4/9 anni, deroghe), riesame (art. 29-octies: nuovi trigger, trasformazione industriale profonda), controlli (art. 29-decies: autorità di controllo regionale, sospensione b-bis), INCITE (art. 29-terdecies).
- Aggiornati estratto, task, esempi, `AGENTS.md`, `README.md`, `agents/openai.yaml`; `normative_refs` e tag nel frontmatter.

### Fixed
- Fonte `dlgs-152-2006-aia-titolo3bis`: la pagina indice Normattiva pinnata restituisce ora SHA256 6652cbbcfa814b819ef2601b8de1e8059bfc2fdc2f241ec2c83a2a3bdc495d31 (prima c2175fe5...); articoli riscaricati e confrontati con la trascrizione, testo dei commi invariato. Hash aggiornato con nota di riverifica.

### Note
- `references/fonti/dlgs-152-2006-aia-titolo3bis.md` resta il testo previgente (vig. 2026-07-17): da riallineare al consolidato Normattiva dopo il 12/11/2026.

## [0.1.0-alpha] - 2026-07-17

### Added (closes #289)
- Prima versione della skill di supporto all'**Autorizzazione Integrata Ambientale (AIA/IPPC)**, ai
  sensi del **D.Lgs. 3 aprile 2006, n. 152, Parte II, Titolo III-bis** (artt. 29-ter, 29-quater,
  29-sexies, 29-octies, 29-decies), nell'area `ambiente-territorio-mobilita`.
- Fonte scaricata, hashata e letta (Regola zero):
  - **D.Lgs. 3 aprile 2006, n. 152** - indice Normattiva pinnato `!vig=2026-07-17`
    SHA256: c2175fe5c9313db1087d444b07e71d727154140d579ffcf6357ababa5d57b45c
    (codice 006G0171). Artt. 29-ter/quater/sexies/octies/decies (idGruppo 9) via `caricaArticolo`.
  - Trascrizione verbatim in `references/fonti/dlgs-152-2006-aia-titolo3bis.md`.
- Estratto operativo `references/estratti/aia-checklist.md`.
- Due task: `inquadra-domanda-aia.md` e `verifica-condizioni-controlli.md`.
- Due esempi: assoggettabilità, domanda e procedura (artt. 29-ter, 29-quater); controlli e
  inosservanze (art. 29-decies).

### Contenuto ancorato al testo
- Art. 29-ter domanda (contenuti a-m, relazione di riferimento, completezza 30 gg); art. 29-quater
  procedura (avvio 30 gg, pubblicazione 15 gg, osservazioni 30 gg, conferenza di servizi, integrazioni
  ≤ 90 gg, determinazione 150 gg, coordinamento VIA); art. 29-sexies contenuto/condizioni (VLE su BAT
  senza obbligo di tecnica specifica, BAT-AEL, monitoraggio, deroghe); art. 29-octies rinnovo/riesame
  (nuove conclusioni sulle BAT; 10 anni; gestore 30-180 gg); art. 29-decies controlli (ISPRA/ARPA;
  ispezioni 1/3 anni, 6 mesi dopo grave inosservanza; inosservanze: diffida/sospensione/revoca-chiusura).

### Scope e limiti
- Non redige la domanda/AIA, non individua le BAT, non riproduce gli Allegati VIII/XII (attività IPPC)
  né i BREF, non tratta le sanzioni (art. 29-quattuordecies). Distinta da AUA (`aua-dpr59-dossier`),
  autorizzazioni singole (`scarichi-emissioni-dlgs152`) e VIA (`via-screening-sia-dlgs152`).

### Note di sviluppo
- Normattiva: ad ogni aggiornamento riscaricare l'indice del D.Lgs. 152/2006 pinnato (nuovo hash) e
  rileggere gli articoli del Titolo III-bis.
- Validazione Livello 2 con tecnico ambientale / autorità competente o ARPA.
