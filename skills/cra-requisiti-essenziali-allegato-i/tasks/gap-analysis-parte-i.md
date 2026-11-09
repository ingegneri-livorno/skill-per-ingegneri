# Task: gap analysis sui requisiti di prodotto (allegato I, parte I)

## Obiettivo

Verificare, requisito per requisito, se il prodotto soddisfa l'allegato I, parte I, e quali evidenze servono nella documentazione tecnica. Presuppone una matrice di applicabilita' (vedi `imposta-valutazione-rischi.md`); se non esiste, costruiscila prima o segnala che ogni "non applicabile" resta da verificare.

## Input richiesti

1. Descrizione tecnica del prodotto: interfacce esterne (rete, radio, USB, porte di debug, API, servizi cloud), sistema operativo e componenti principali, modello di autenticazione, dati trattati.
2. Configurazione di fabbrica (credenziali, servizi attivi, porte aperte, funzioni abilitate).
3. Meccanismo di aggiornamento: come arrivano gli aggiornamenti, se sono automatici, se l'utente puo' disattivarli o rinviarli.
4. Stato delle vulnerabilita' note alla data di immissione (scansioni, SBOM confrontata con database di vulnerabilita').
5. Matrice di applicabilita' della valutazione dei rischi, se esiste.
6. Prove gia' svolte (test, review, penetration test) e relativi rapporti.

## Fonti

- `../references/estratti/cra-allegato-i-requisiti-e-obblighi.md`, sezioni C, D, H, I.
- `../references/fonti/reg-ue-2024-2847-cra-requisiti-essenziali.md`: allegato I, parte I; art. 6, lett. a); art. 13, par. 1, 3, 4; art. 3, punto 41; allegato VII, punti 3, 5, 6; art. 27.

## Procedura

### 1. Parte I, punto 1

Verifica che la documentazione dica **come** il livello di cibersicurezza e' stato commisurato ai rischi. Non e' un controllo tecnico ma di coerenza: le scelte delle lettere a)-m) devono discendere dalla valutazione dei rischi.

### 2. Parte I, punto 2 - una lettera alla volta

Per ogni lettera applicabile, confronta il prodotto con le parole del testo (tabella in sezione D dell'estratto). Punti di controllo letterali che vengono spesso persi:

- **a)** "vulnerabilita' **sfruttabili note**" alla **messa a disposizione**: serve un controllo delle vulnerabilita' note sui componenti alla data di rilascio. [pratica, non norma] Una vulnerabilita' nota che si ritiene non sfruttabile nel contesto (art. 3, punto 41) conviene motivarla per iscritto. Il considerando 38 indica che ogni esemplare dovrebbe aver ricevuto le patch disponibili al momento dell'immissione.
- **b)** configurazione sicura **per impostazione predefinita** e **ripristino dello stato originale**. Credenziali predefinite uguali per tutti gli esemplari, servizi di debug attivi o porte inutili aperte di fabbrica sono rilievi da discutere su questa lettera e sulla j). L'eccezione vale solo per accordo con un **utilizzatore commerciale** su un **prodotto su misura**.
- **c)** cinque elementi distinti: aggiornamenti di sicurezza possibili; se del caso **automatici**; **attivi per impostazione predefinita**; **disattivazione chiara e facile**; **notifica** e **rinvio temporaneo**. Registra lo stato di ciascuno.
- **d)** due elementi: controllo degli accessi **e segnalazione** degli accessi non autorizzati.
- **e)** riservatezza "ad esempio" con crittografia a riposo e in transito con meccanismi **all'avanguardia**: il testo e' esemplificativo, ma la scelta di non cifrare va motivata nella valutazione dei rischi.
- **f)** integrita' anche di **comandi, programmi e configurazione**, e **segnalazione delle corruzioni** (per esempio verifica della firma del firmware all'avvio e all'aggiornamento: [pratica, non norma]).
- **g)** minimizzazione **rispetto alla finalita' prevista**: elenca i dati raccolti e la funzione che li giustifica.
- **h)** disponibilita' delle funzioni **essenziali e di base**, anche **dopo un incidente**.
- **i)** impatto **su altri dispositivi o reti** (per esempio uso del prodotto in una botnet o traffico non limitato: [pratica, non norma]).
- **j)** superficie di attacco, **comprese le interfacce esterne**: elenca ogni interfaccia e perche' esiste.
- **k)** tecniche di **attenuazione dello sfruttamento**.
- **l)** registrazione e monitoraggio delle attivita' interne pertinenti **con meccanismo di disattivazione per l'utilizzatore**.
- **m)** rimozione **sicura, agevole e permanente** di **tutti** i dati e impostazioni; trasferimento sicuro se i dati sono trasferibili.

### 3. Evidenze e presunzione di conformita'

Per ogni lettera indica l'evidenza da inserire nella documentazione tecnica (allegato VII, punto 6: relazioni delle prove). Se il fabbricante applica norme armonizzate, chiedi quali e verifica che i riferimenti siano **pubblicati in GU UE** (art. 27, par. 1): la skill non conosce l'elenco. Se non ne applica, l'allegato VII, punto 5, richiede la **descrizione delle soluzioni adottate** per ciascun requisito.

### 4. Condizioni dell'art. 6, lett. a)

La conformita' della parte I e' valutata assumendo installazione corretta, manutenzione adeguata, uso conforme o ragionevolmente prevedibile e aggiornamenti installati. Queste condizioni rendono indispensabili le istruzioni dell'allegato II (vedi `check-informazioni-utilizzatore.md`).

## Output

Tabella con una riga per lettera:

| Requisito | Applicabile | Stato | Cosa manca | Evidenza per allegato VII |
|---|---|---|---|---|

Stati ammessi: soddisfatto / parziale / mancante / non applicabile (giustificato) / da verificare. Seguono le lacune in ordine di priorita' e il rinvio al fabbricante.

[pratica, non norma] Priorita' suggerita: prima cio' che il testo vieta alla messa a disposizione (lett. a e b), poi la capacita' di correggere sul campo (lett. c e f), poi il resto.

## Limiti

- Non esegue test, scansioni o penetration test: ne legge i risultati.
- Non indica algoritmi, lunghezze di chiave o soglie: il testo non li contiene.
- Non decide se una norma armonizzata copre un requisito.
