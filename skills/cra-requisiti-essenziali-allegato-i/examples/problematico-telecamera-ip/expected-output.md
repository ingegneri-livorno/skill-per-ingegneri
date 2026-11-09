# Output atteso - telecamera IP

## Precondizioni

- **Chi e' il fabbricante.** Un importatore che immette sul mercato il prodotto **con il proprio nome o marchio** e' ritenuto fabbricante ed e' soggetto agli obblighi degli artt. 13 e 14 (art. 21; vedi anche art. 3, punto 13). Gli obblighi dell'art. 13 ricadono quindi sul **cliente**, non solo sul produttore originale. "CRA ready" dichiarato dal fornitore non e' un'evidenza: servono valutazione dei rischi, documentazione tecnica e prove (art. 13, par. 4 e 12; allegato VII).
- Ambito e classificazione non accertati: eseguire prima `cra-classificazione-pde`.
- Immissione prevista giugno 2028: allegato I e art. 13 si applicano integralmente (art. 71, par. 2).

## Parte II "non applicabile": non ammissibile con questa motivazione

La parte II non e' filtrata dalla valutazione dei rischi: la formula "ove applicabile" riferita al rischio riguarda solo la parte I, punto 2 (allegato I, parte I, punto 2, alinea; art. 13, par. 3, ultimo periodo). Una non applicabilita' richiede una chiara giustificazione (art. 13, par. 4) e deve poggiare sulla formulazione del singolo punto; il prezzo del prodotto e l'assenza di sviluppo interno non sono criteri previsti dal testo. Il cliente, come fabbricante, risponde dei processi della parte II (art. 6, lett. b; art. 13, par. 8). [pratica, non norma] In concreto questo richiede accordi con il produttore originale che coprano SBOM, CVD, correzioni e aggiornamenti.

## Valutazione dei rischi

**Mancante.** Senza di essa nessuna lettera della parte I, punto 2, puo' essere dichiarata non applicabile (art. 13, par. 3-4) e manca l'elemento dell'allegato VII, punto 3.

## Parte I

| Requisito | Stato | Rilievo |
|---|---|---|
| 2 a) | mancante | nessun controllo delle vulnerabilita' sfruttabili note prima della messa a disposizione |
| 2 b) | mancante | credenziale `admin/admin` comune a tutti gli esemplari e telnet attivo: configurazione non sicura per impostazione predefinita |
| 2 c) | mancante | nessun aggiornamento automatico ne' notifica; correzioni solo a pagamento |
| 2 d) | mancante | password comune; nessuna segnalazione di accessi non autorizzati descritta |
| 2 e) | mancante | interfaccia web in HTTP: dati in transito non protetti, nessuna giustificazione |
| 2 j) | mancante | telnet espone una superficie di attacco non necessaria |
| 2 g) e l) | mancante | log di uso inviati al cloud senza giustificazione rispetto alla finalita' prevista (lett. g, minimizzazione) e senza meccanismo di disattivazione per l'utilizzatore (lett. l) |
| 2 m) | mancante | il reset non rimuove tutti i dati (SD, associazione cloud) |
| 2 f), h), i), k) | da verificare | dati non forniti |

## Parte II e art. 13

| Punto | Stato | Rilievo |
|---|---|---|
| 1) | mancante | un PDF del 2026 non e' una SBOM in formato leggibile da dispositivo automatico ne' aggiornata |
| 2) | mancante | correzioni non separate dalle funzioni e non tempestive |
| 3) | mancante | nessuna prova periodica |
| 4) | mancante | nessuna divulgazione delle vulnerabilita' risolte |
| 5) | mancante | nessuna politica CVD |
| 6) | mancante | nessun indirizzo di contatto per le segnalazioni |
| 7) | parziale | distribuzione manuale dal sito; sicurezza del canale da verificare |
| 8) | mancante | aggiornamenti di sicurezza a pagamento: il testo li vuole gratuiti |

**Periodo di assistenza**: 2 anni non rispetta il minimo di cinque anni (art. 13, par. 8, terzo comma) e non riflette la durata d'uso indicata di 5-7 anni (art. 13, par. 8, secondo comma). Anche cinque anni potrebbero non bastare se la durata d'uso prevista e' piu' lunga: il periodo va fissato in base a essa, con cinque anni come minimo. La garanzia legale non e' un criterio previsto dal testo. Mancano la motivazione nella documentazione tecnica (allegato VII, punto 4), la conservazione degli aggiornamenti per dieci anni (par. 9) e la data di fine assistenza al momento dell'acquisto (par. 19).

**Componenti di terzi**: dovuta diligenza non documentata (art. 13, par. 5).

## Informazioni all'utilizzatore

Mancano almeno: punto di contatto unico che consenta di scegliere il mezzo di comunicazione (il solo chatbot non basta, art. 13, par. 17), politica CVD (allegato II, punto 2), data di fine assistenza (allegato II, punto 7), istruzioni per disattivare gli aggiornamenti automatici e per l'eliminazione sicura dei dati (punto 8, lett. d ed e). Lingua da verificare: il testo chiede una lingua facilmente comprensibile dagli utilizzatori (art. 13, par. 18).

## Lacune in ordine di priorita'

1. Configurazione di fabbrica (lett. b, d, j): credenziale univoca o impostata al primo avvio, telnet disattivato.
2. Aggiornamenti di sicurezza gratuiti, separati, notificati, automatici di default (parte I lett. c; parte II punti 2, 7, 8).
3. Periodo di assistenza che rifletta la durata d'uso prevista (5-7 anni), con minimo di cinque anni, motivato e comunicato all'acquisto.
4. [pratica, non norma] Accordo col produttore originale che copra SBOM, CVD, correzioni e disponibilita' degli aggiornamenti per tutto il periodo.
5. Valutazione dei rischi e documentazione tecnica.
6. Istruzioni conformi all'allegato II.

## Esposizione sanzionatoria

La non conformita' all'allegato I e all'art. 13 rientra nel massimale piu' alto dell'art. 64, par. 2 (15 000 000 EUR o 2,5% del fatturato mondiale annuo, se superiore). Le norme sanzionatorie sono fissate dagli Stati membri (art. 64, par. 1): la disciplina italiana non e' fra le fonti lette.

## Rinvio

Gap analysis di supporto. Il cliente, come fabbricante, resta responsabile della conformita'. Il rapporto col produttore originale ha profili contrattuali e legali da verificare con un consulente.
