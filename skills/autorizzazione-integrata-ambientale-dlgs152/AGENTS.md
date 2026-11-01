# AGENTS.md - autorizzazione-integrata-ambientale-dlgs152

> Convenzioni di dominio per agent che lavorano su questa skill. Per le
> convenzioni globali del repo vedi `../../AGENTS.md`.

## Dominio

Supporto documentale all'**Autorizzazione Integrata Ambientale (AIA/IPPC)**: domanda, procedura di
rilascio, contenuto e condizioni (VLE su BAT), rinnovo/riesame, rispetto delle condizioni e
controlli/ispezioni, secondo il **D.Lgs. 3 aprile 2006, n. 152, Parte II, Titolo III-bis** (artt.
29-ter, 29-quater, 29-sexies, 29-octies, 29-decies), come modificato dal **D.Lgs. 28 settembre 2026, n. 197** (recepimento IED2, in vigore dal 12/11/2026). Target: ingegneri, gestori di installazioni, consulenti ambientali.

**È una skill documentale**: inquadra procedura/contenuto/controlli; **non redige** la domanda/AIA,
**non individua** le BAT, non sostituisce il gestore, l'autorità competente o ISPRA/ARPA.

## Nota sull'area e complementarità

Area **ambiente-territorio-mobilita**. Complementare e distinta da `aua-dpr59-dossier` (AUA, impianti
**non** soggetti ad AIA), `scarichi-emissioni-dlgs152` (autorizzazioni singole residuali) e
`via-screening-sia-dlgs152` (VIA): questa copre l'**AIA** (impianti IPPC).

## Fonti autoritative

Catalogata in `references/sources.yaml`:

- **dlgs-152-2006-aia-titolo3bis**: D.Lgs. 3 aprile 2006, n. 152, pagina indice Normattiva pinnata a
  `!vig=2026-07-17` (hash `6652cbbc...`, riverificato 2026-11-01; codice 006G0171). Artt. 29-ter, 29-quater, 29-sexies,
  29-octies, 29-decies (idGruppo 9) caricati via `caricaArticolo` e trascritti verbatim. Testo **previgente** al D.Lgs. 197/2026.
- **dlgs-197-2026-ied2**: D.Lgs. 28 settembre 2026, n. 197, fascicolo PDF della GU SG n. 251 del 28-10-2026 (hash `d4fd3721...`; codice 26G00213). Articoli rilevanti trascritti verbatim in `references/fonti/dlgs-197-2026-ied2.md`.

Trascrizioni in `references/fonti/dlgs-152-2006-aia-titolo3bis.md` e `references/fonti/dlgs-197-2026-ied2.md`; estratto operativo in
`references/estratti/aia-checklist.md`.

## Punti chiave (verificati sul testo)

- **D.Lgs. 197/2026**: in vigore dal **12/11/2026**; regime transitorio all'art. 43 (per le installazioni già autorizzate parte delle novità si applica dal riesame, al più tardi 1° settembre 2036). Marcare sempre se una regola è pre- o post-D.Lgs. 197/2026.
- **Commissione AIA-IPPC** (art. 8-bis): 23 esperti + 5 designati dal Ministero della salute entro 3 mesi.
- **Campo di applicazione**: Allegato VIII ampliato; allevamenti nell'Allegato VIII-bis / Titolo III-ter; Allegato X abrogato.

- **Domanda** (art. 29-ter): contenuti a-m-bis; relazione di riferimento per sostanze pericolose;
  inoltro 10 gg, osservazioni amministrazioni 20 gg, integrazioni una sola volta entro 30 gg dall'avvio.
- **Procedura** (art. 29-quater): avvio 30 gg, pubblicazione 15 gg, osservazioni 30 gg, conferenza di
  servizi decisoria (AIA statale: Ministero della salute, parere ISS), integrazioni ≤ 90 gg, determinazione entro **150 gg**; coordinamento con la VIA.
- **Contenuto** (art. 29-sexies): VLE su **BAT** (senza obbligo di tecnica specifica), entro i
  **BAT-AEL** (e **BAT-AEPL** per conclusioni post 1° luglio 2026); SGA entro 1° luglio 2030; piano di trasformazione entro 30 giugno 2030; acque sotterranee 4 anni, suolo 9 anni; deroghe su istanza del gestore.
- **Riesame** (art. 29-octies): su nuove conclusioni sulle BAT; **10 anni** dal rilascio/ultimo
  riesame; gestore 30-180 gg; nuovi trigger sanitari (c. 4 lett. c-bis); trasformazione industriale profonda fino a 8 anni.
- **Controlli** (art. 29-decies): ISPRA/ARPA; ispezioni 1/3 anni, 6 mesi dopo grave inosservanza;
  inosservanze → diffida/sospensione (anche per violazioni reiterate più di 2 volte in un anno)/revoca-chiusura.

## Convenzioni specifiche

### Cosa NON fare
- Non **redigere** la domanda/AIA né individuare le **BAT** applicabili.
- Non **riprodurre** gli **Allegati VIII/XII** (attività IPPC/soglie) né i BREF.
- Non inventare **termini** (usare quelli dell'estratto, tratti dalle due fonti) e non applicare le novità del D.Lgs. 197/2026 senza verificare l'art. 43.

### Cosa fare
- **Verificare** l'assoggettabilità (rinvio All. VIII/XII), **comporre** contenuti/timeline della
  domanda, **inquadrare** contenuto/riesame/controlli.

## Aggiornamento delle fonti

Normattiva: riscaricare l'indice del D.Lgs. 152/2006 pinnato a nuovo `!vig=` (nuovo hash) e rileggere
gli artt. 29-ter/quater/sexies/octies/decies (testo tra `(( ))`). Dopo il 12/11/2026 sostituire la trascrizione previgente con il testo consolidato che include il D.Lgs. 197/2026.

## Validatori

- Non ancora assegnato (Livello 2 con tecnico ambientale / autorità competente o ARPA).

## Stato attuale

- Versione: 0.2.0-alpha
- Task files: 2 (`inquadra-domanda-aia.md`, `verifica-condizioni-controlli.md`)
- Esempi: 2 (domanda e procedura; controlli e inosservanze art. 29-decies)
