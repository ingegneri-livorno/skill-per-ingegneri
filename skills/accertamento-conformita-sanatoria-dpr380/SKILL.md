---
name: accertamento-conformita-sanatoria-dpr380
description: "Supporto documentale al progettista (geometra, architetto, ingegnere) e al tecnico incaricato per l'accertamento di conformita' (permesso di costruire o SCIA in sanatoria) degli interventi edilizi abusivi, ai sensi del D.P.R. 6 giugno 2001, n. 380 (Testo unico edilizia), Titolo IV, artt. 36, 36-bis e 37, come modificati dal decreto-legge 69/2024 (salva-casa) convertito dalla legge 105/2024. Use when a surveyor, architect, or engineer must frame the building compliance assessment (permit or SCIA in condono/sanatoria) for unlawful works under D.P.R. 380/2001 as amended by the 2024 salva-casa reform; it is a documentary aid and does NOT draft the application or the compliance statement, does NOT classify the abuse or compute the oblation or venal value, does NOT cover the condono under special laws, and does NOT replace the designer, the one-stop building desk, or the competent authorities."
license: MIT
area: edilizia-urbanistica-catasto
title: "Accertamento di conformita' / sanatoria edilizia - salva-casa (DPR 380/2001)"
summary: "Inquadra l'accertamento di conformita' (sanatoria edilizia) del DPR 380/2001 dopo il salva-casa: doppia conformita' piena per assenza titolo/totale difformita' (36), attenuata per parziale difformita'/variazioni essenziali con silenzio-assenso 45 gg (36-bis), sanzione SCIA (37)."
normative_refs:
  - "D.P.R. 6 giugno 2001, n. 380 (Testo unico edilizia) - artt. 36 (assenza titolo/totale difformita'), 36-bis (parziale difformita'/variazioni essenziali - salva-casa) e 37 (assenza/difformita' SCIA)"
  - "Rinvio: D.L. 69/2024 conv. L. 105/2024 (salva-casa, introduce l'art. 36-bis); artt. 31-34, 34-bis, 9-bis, 44 DPR 380; art. 167 D.Lgs. 42/2004; leggi condono (non trattate)"
  - "D.L. 11/11/2026 n. 205 (GU n. 263 dell'11/11/2026, vigente dal 12/11/2026, da convertire) - art. 13: Campi Flegrei, sanatorie in 60 gg e condoni in 90"
version: 0.2.0-alpha
status: alpha
tags:
  - accertamento-conformita
  - sanatoria-edilizia
  - salva-casa
  - dpr-380-2001
  - doppia-conformita
---

# Accertamento di conformità / sanatoria edilizia - salva-casa (DPR 380/2001 artt. 36, 36-bis, 37)

## Quando usare questa skill

Usala quando un **progettista** (geometra/architetto/ingegnere) o un **tecnico incaricato** deve
**inquadrare** l'**accertamento di conformità** (permesso di costruire o SCIA **in sanatoria**) di un
intervento edilizio abusivo, secondo il **D.P.R. 6 giugno 2001, n. 380** (Testo unico edilizia),
**Titolo IV, artt. 36, 36-bis e 37**, come modificati dal **DL 69/2024 ("salva-casa"), conv. L.
105/2024**:

- capire **quale articolo** si applica in base al tipo di abuso;
- **art. 36** (assenza di titolo / totale difformità): doppia conformità piena;
- **art. 36-bis** (parziale difformità / variazioni essenziali): doppia conformità attenuata;
- **art. 37** (assenza/difformità dalla SCIA): sanzione e rinvio all'art. 36-bis.

**Non è** uno strumento che redige la domanda o la dichiarazione di conformità, né qualifica l'abuso o
calcola l'oblazione: è un **supporto documentale** che inquadra presupposti, termini ed effetti.

## Cosa fa

| Sotto-attività | Descrizione |
|---|---|
| `inquadra-articolo-doppia-conformita` | Stabilisce quale articolo si applica (36/36-bis/37) e quale doppia conformità è richiesta in base alla qualificazione dell'abuso |
| `inquadra-procedura-oblazione-termini` | Inquadra dichiarazione del professionista, oblazione, profili sismici/paesaggistici, termini ed esito (art. 36-bis; art. 37) |

## Punti chiave (verificati sul testo)

- **Art. 36** (assenza titolo/totale difformità): **doppia conformità piena** (realizzazione **e**
  domanda) (c. 1); oblazione = **contributo doppio** (c. 2); **60 giorni**, **silenzio-rifiuto** (c. 3).
- **Art. 36-bis** (parziale difformità/variazioni essenziali, **salva-casa**): **doppia conformità
  attenuata** (urbanistica alla **domanda** + requisiti edilizi alla **realizzazione**) (c. 1);
  **dichiarazione del professionista abilitato** e prova dell'**epoca** (art. 9-bis c. 1-bis) (c. 3);
  **sismica** (c. 3-bis) e **paesaggistica** (cc. 4, 5-bis); **oblazione** (c. 5: doppio contributo
  **+20%** o doppio valore venale, **1.032-10.328** / **516-5.164 euro**); **45 giorni**,
  **silenzio-assenso** (c. 6).
- **Art. 37** (assenza/difformità SCIA): sanzione **triplo** dell'aumento del valore venale, **min 1.032
  euro** (c. 1); vincolati (cc. 2-3); rinvio all'accertamento **art. 36-bis** (c. 6).

## Zona dei Campi Flegrei: regime speciale D.L. 205/2026 - stato al 15 novembre 2026

Per immobili e interventi nella **zona di intervento dei Campi Flegrei** (art. 1 c. 5: territorio dei comuni di Bacoli, Napoli e Pozzuoli ricompreso nella zona del Piano straordinario dell'art. 2 del D.L. 140/2023; per le funzioni degli artt. 12, 13 e 13-bis del D.L. 144/2026 anche il comune di Monte di Procida) si applica il regime speciale del **D.L. 11 novembre 2026, n. 205** "Piano straordinario per i Campi Flegrei nonche' ulteriori disposizioni urgenti di protezione civile" (GU SG n. 263 dell'11/11/2026, in vigore dal **12/11/2026**, art. 28). Fonte: https://www.gazzettaufficiale.it/eli/id/2026/11/11/26G00225/sg - testo in [`references/fonti/dl-205-2026-gu-263.md`](references/fonti/dl-205-2026-gu-263.md).

- **Art. 13 (sanatorie e condoni sugli immobili oggetto di contributo)**: per gli **interventi edilizi realizzati prima del 1/8/2026** sugli immobili oggetto dei contributi per la riduzione della vulnerabilita' sismica e per il ripristino, il pronto ripristino e la riqualificazione sismica elencati al c. 1 si applica, in quanto compatibile, l'**art. 1-sexies del D.L. 55/2018** (c. 1). Le richieste di **permesso di costruire in sanatoria** e le **SCIA in sanatoria** presentate ai sensi del c. 1, anche contestualmente alla domanda di contributo, sono concluse dal Comune **con provvedimento espresso entro 60 giorni** (c. 2); il Comune puo' chiedere **una sola volta**, entro 15 giorni, le integrazioni strettamente necessarie, con sospensione dei termini fino alla ricezione e comunque per non oltre 30 giorni (c. 3). Le **istanze di condono** (L. 47/1985, L. 724/1994, D.L. 269/2003) non ancora definite sono definite **con priorita' entro 90 giorni** dalla comunicazione della domanda di contributo (c. 4). Restano ferme le norme antisismiche, di sicurezza, antincendio, igienico-sanitarie, energetiche, idrogeologiche e il D.Lgs. 42/2004 (c. 5). Sanzioni, oblazioni e oneri della sanatoria o del condono **restano a carico dell'interessato** e non sono ammessi a contributo (c. 7). Resta ferma, **ove di maggiore favore**, la disciplina del D.L. 69/2024 (salva-casa); l'intervento deve essere conforme alle norme tecniche per le costruzioni in zona sismica **sia al momento della realizzazione sia al rilascio del titolo in sanatoria** (c. 8).
- **Rapporto con il contributo**: la pendenza della sanatoria o del condono non preclude la domanda di contributo, ma la concessione e' subordinata alla loro positiva conclusione (art. 13 c. 6); il contributo spetta solo se l'immobile e' munito del titolo e conforme ad esso, o di titolo in sanatoria conseguito alla data della domanda, o nei casi dell'art. 13 (art. 12 c. 8).
- **Rapporto con gli artt. 36 e 36-bis**: il testo trascritto del decreto non modifica gli artt. 36, 36-bis e 37 del D.P.R. 380/2001; per questi casi fissa un termine di 60 giorni con provvedimento espresso e fa salva la disciplina del salva-casa ove piu' favorevole. Il testo trascritto non dice come l'art. 13 c. 2 si coordina con il silenzio-rifiuto dell'art. 36 c. 3 e con il silenzio-assenso dell'art. 36-bis c. 6: verificarlo con il Comune e con gli atti del Commissario.
- **Ordinanze del Commissario**: il Commissario puo' assegnare con ordinanza alla propria struttura di supporto, in tutto o in parte, l'istruttoria dei procedimenti edilizi dell'art. 13 (c. 6).
- **Decreto-legge non ancora convertito**: il decreto "sara' presentato alle Camere per la conversione in legge" (art. 28); le disposizioni possono cambiare in sede di conversione. Ricontrollare questa sezione alla pubblicazione della legge di conversione in GU.
- **Segnalalo all'utente** quando l'immobile ricade nella zona. La skill non tratta il condono ne' l'art. 1-sexies del D.L. 55/2018 (non trascritto): rinvia al testo del decreto e agli atti del Commissario.

## Fonti

- **D.P.R. 6 giugno 2001, n. 380** (Testo unico edilizia) - **artt. 36, 36-bis, 37** - testo vigente su
  Normattiva (indice pinnato a `!vig=2026-07-17`, codice 001G0429, idGruppo 9).
- **D.L. 11/11/2026 n. 205** (Campi Flegrei) - artt. 1, 12, 13, 28; decreto-legge da convertire in legge.

Dettaglio in `references/sources.yaml`, `references/fonti/`, `references/estratti/`.

## Limiti

- **Non redige** la domanda di sanatoria né la **dichiarazione di conformità** del professionista.
- **Non qualifica** l'abuso (assenza/totale/parziale/variazione essenziale) al posto del tecnico; **non
  calcola** l'oblazione né il **valore venale**.
- **Non tratta** il **condono** (leggi speciali: L. 47/1985 capo IV, L. 724/1994, L. 326/2003) né lo
  **stato legittimo** (art. 9-bis) se non nei richiami.

**La skill è un supporto documentale: non sostituisce il progettista, lo sportello unico per l'edilizia
o gli enti competenti, né la lettura degli artt. 36-37 del D.P.R. 380/2001 e delle norme del salva-casa.**
