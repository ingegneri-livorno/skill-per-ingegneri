# AGENTS.md - terre-rocce-scavo-dpr120

> Convenzioni di dominio per agent che lavorano su questa skill. Per le
> convenzioni globali del repo vedi `../../AGENTS.md`.

## Dominio

Supporto documentale alla **gestione delle terre e rocce da scavo**: qualificazione come
**sottoprodotto** (anziche' rifiuto), **esclusione dalla disciplina rifiuti** (riutilizzo nel
sito), gestione nei cantieri di **piccole** e **grandi** dimensioni. Fonte: **D.P.R. 120/2017**,
coordinato con la **Parte IV del D.Lgs. 152/2006**. Target: ingegneri, consulenti ambientali,
imprese, direzione lavori.

**E' una skill documentale**: inquadra qualificazione e procedure; **non riproduce i valori CSC**
ne' gli Allegati tecnici, non esegue campionamento/analisi e non sostituisce l'ARPA.

## Nota sull'area e sulla complementarita'

Area **ambiente-territorio-mobilita**. Complementare a `trasporto-rifiuti-fir-dlgs152` (rifiuti/
FIR) e `bonifica-siti-contaminati-dlgs152` (bonifica): questa copre la **gestione delle terre da
scavo** (sottoprodotto/riutilizzo).

## Fonti autoritative

Catalogata in `references/sources.yaml`:

- **dpr-120-2017**: D.P.R. 13 giugno 2017, n. 120, indice Normattiva pinnato `!vig=2026-07-16`
  (hash `67cee768...`, codice 17G00135). Artt. 1, 2, 4, 20, 21, 24 (testo vigente) via
  `caricaArticolo`, trascritti verbatim.

- **dl-177-2026-gu234**: D.L. 8 ottobre 2026, n. 177, GU SG n. 234 dell'8/10/2026 (hash `a9cf0cd5...`).
  Solo art. 4, c. 1, lett. b (nuovo art. 185-ter D.Lgs. 152/2006) e art. 6. Decreto-legge da convertire:
  non modifica il D.P.R. 120/2017.

Trascrizioni in `references/fonti/`; estratti in `references/estratti/`.

## Punti chiave (verificati sul testo)

- **Sottoprodotto** (art. 4, ex art. 184-bis D.Lgs. 152/2006): 4 requisiti (generazione in
  un'opera; utilizzo conforme a **piano/dichiarazione**; idoneita' senza trattamenti; requisiti
  ambientali).
- **Dimensione cantiere** (art. 2): **piccole <= 6.000 mc** (dichiarazione, artt. 20-21); **grandi
  > 6.000 mc** (piano di utilizzo, artt. 9 e ss.; VIA/AIA).
- **Piccoli cantieri** (artt. 20-21): requisiti ambientali (**CSC** colonne A/B, Tab. 1, All. 5,
  Parte IV, D.Lgs. 152/2006) + **dichiarazione di utilizzo** (allegato 6, **15 gg** prima, Comune +
  ARPA, utilizzo entro **1 anno**, DAU finale).
- **Utilizzo nel sito** (art. 24): terre **escluse dai rifiuti** (art. 185 D.Lgs. 152/2006) se non
  contaminate (allegato 4); amianto naturale solo nel sito con controllo ARPA/ASL.

- **Art. 185-ter D.Lgs. 152/2006** (D.L. 177/2026): deposito di CER 17.05.04/17.05.03* elevato a 4.000 mc
  (max 800 mc pericolosi); cantieri puntuali <= 20 mc: riutilizzo diretto in sito senza caratterizzazione,
  con esclusioni (c. 3). Non citare i limiti precedenti dell'art. 185-bis: non sono nelle fonti.

## Convenzioni specifiche

### Cosa NON fare
- Non **riprodurre i valori CSC** (D.Lgs. 152/2006, Allegato 5) ne' gli **Allegati tecnici** del
  DPR (campionamento/analisi, modulistica): rinviare agli atti. Non inventare soglie o esiti.
- Non **eseguire** campionamento/analisi ne' redigere il piano/la dichiarazione.

### Cosa fare
- Qualificare le terre (sottoprodotto/escluse/rifiuto), determinare la dimensione del cantiere e
  impostare la dichiarazione (piccoli cantieri) o rinviare al piano di utilizzo (grandi).

## Aggiornamento delle fonti

Controllare la legge di conversione del D.L. 177/2026 (art. 4, c. 1, lett. b). Normattiva: riscaricare l'indice del D.P.R. 120/2017 pinnato a nuovo `!vig=` (nuovo hash) e
rileggere gli articoli; verificare gli aggiornamenti delle CSC (D.Lgs. 152/2006) e degli allegati.

## Validatori

- Non ancora assegnato (Livello 2 con professionista ambientale / ARPA).

## Stato attuale

- Versione: 0.2.0-alpha (closes #259, #508)
- Task files: 2 (`qualifica-terre-scavo.md`, `gestisci-dichiarazione-piccoli-cantieri.md`)
- Esempi: 3 (piccolo cantiere - dichiarazione di utilizzo; riutilizzo nel sito di produzione; cantiere puntuale <= 20 mc)
