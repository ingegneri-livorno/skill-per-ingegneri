# Task: verificare informazioni e istruzioni per l'utilizzatore (allegato II; art. 13, par. 15-20)

## Obiettivo

Verificare che il prodotto sia accompagnato dalle informazioni e istruzioni richieste dall'allegato II e dagli obblighi di identificazione e contatto dell'art. 13. Le istruzioni sono anche cio' che rende operanti le condizioni dell'art. 6, lett. a) (installazione corretta, manutenzione, aggiornamenti installati).

## Input richiesti

1. Le istruzioni per l'utente e le informazioni di accompagnamento (manuale, foglio di avvertenze, pagina web), in bozza o definitive.
2. Etichetta e imballaggio: identificazione del prodotto e del fabbricante.
3. Dove e come e' indicata la data di fine del periodo di assistenza al momento dell'acquisto.
4. Lingue in cui le informazioni sono fornite.
5. Se il prodotto e' destinato a essere integrato in altri prodotti.
6. Se il fabbricante rende disponibile la SBOM all'utilizzatore.

## Fonti

- `../references/estratti/cra-allegato-i-requisiti-e-obblighi.md`, sezione G.
- `../references/fonti/reg-ue-2024-2847-cra-requisiti-essenziali.md`: allegato II; art. 13, par. 15, 16, 17, 18, 19, 20; art. 6, lett. a).

## Procedura

### 1. Checklist allegato II (contenuto minimo)

| Punto | Elemento | Presente? | Dove |
|---|---|---|---|
| 1 | Nome o marchio del fabbricante, indirizzo postale, e-mail o altro contatto digitale, sito web se disponibile | | |
| 2 | Punto di contatto unico per segnalare e ricevere informazioni sulle vulnerabilita' **e** dove trovare la politica CVD | | |
| 3 | Nome, tipo e informazioni per l'identificazione univoca | | |
| 4 | Finalita' prevista, ambiente di sicurezza, funzionalita' essenziali, proprieta' di sicurezza | | |
| 5 | Circostanze note o prevedibili, anche di uso improprio, che possono comportare rischi significativi | | |
| 6 | Se del caso, indirizzo Internet della dichiarazione di conformita' UE | | |
| 7 | Tipo di assistenza di sicurezza e **data finale del periodo di assistenza** | | |
| 8 a) | Misure per l'uso sicuro alla prima messa in servizio e per tutta la durata | | |
| 8 b) | Come le modifiche al prodotto possono influire sulla sicurezza dei dati | | |
| 8 c) | Come installare gli aggiornamenti di sicurezza | | |
| 8 d) | Smantellamento sicuro ed eliminazione sicura dei dati | | |
| 8 e) | Come disattivare l'installazione automatica degli aggiornamenti (allegato I, parte I, punto 2, lett. c) | | |
| 8 f) | Se destinato all'integrazione: informazioni per l'integratore su allegato I e allegato VII | | |
| 9 | Se la SBOM e' resa disponibile: dove trovarla | | |

Il punto 8 ammette **istruzioni dettagliate oppure un indirizzo Internet** che vi rimandi.

### 2. Obblighi di forma e durata (art. 13)

- Identificazione del prodotto (numero di tipo, lotto o serie) sul prodotto o, se non possibile, su imballaggio o documento (par. 15).
- Dati del fabbricante sul prodotto, imballaggio o documento, e anche nelle istruzioni (par. 16).
- Punto di contatto unico **facilmente identificabile**, che consenta di **scegliere il mezzo** di comunicazione senza limitarsi a strumenti automatizzati (par. 17). Un solo chatbot non basta.
- Istruzioni in lingua facilmente comprensibile, chiare e leggibili, in forma cartacea o elettronica (par. 18).
- Disponibili **almeno dieci anni** dall'immissione o per il periodo di assistenza se superiore; se online, accessibili e disponibili per lo stesso periodo (par. 18).
- Data di fine assistenza (almeno **mese e anno**) chiara **al momento dell'acquisto** (par. 19).
- Copia della dichiarazione di conformita' UE o dichiarazione semplificata con l'indirizzo Internet esatto di quella completa (par. 20).

### 3. Coerenza con le altre parti

- La data del punto 7 coincide con il periodo di assistenza fissato in `gap-analysis-parte-ii.md`?
- Il punto 8 e) descrive davvero il meccanismo di disattivazione verificato in `gap-analysis-parte-i.md` (lett. c)?
- Le proprieta' di sicurezza del punto 4 corrispondono a quelle documentate nella valutazione dei rischi?

## Output

1. Checklist allegato II compilata.
2. Elenco degli obblighi di forma e durata con stato.
3. Incoerenze fra istruzioni, valutazione dei rischi e periodo di assistenza.
4. Lacune in ordine di priorita' e rinvio al fabbricante.

## Limiti

- Non redige il manuale: indica cosa deve contenere.
- Non verifica i requisiti linguistici nazionali, che il testo affida a una "lingua facilmente comprensibile dagli utilizzatori e dalle autorita' di vigilanza del mercato" senza indicarla.
- Non verifica il contenuto della dichiarazione di conformita' UE (art. 28, allegato V, non letti).
