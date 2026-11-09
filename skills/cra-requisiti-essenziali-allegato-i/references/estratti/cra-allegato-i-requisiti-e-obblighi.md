# Estratto: requisiti essenziali dell'allegato I e obblighi del fabbricante (Reg. UE 2024/2847)

Parafrasi operativa di `../fonti/reg-ue-2024-2847-cra-requisiti-essenziali.md`. Ogni affermazione cita articolo, paragrafo, punto e lettera della fonte. Dove questo estratto aggiunge un suggerimento tecnico che non viene dal testo, lo marca come **[pratica, non norma]**.

## A. Quando si applica

- Il Regolamento si applica **dall'11 dicembre 2027** (art. 71, par. 2, primo comma). Requisiti essenziali (allegato I) e obblighi del fabbricante (art. 13) ricadono in questa data.
- Fanno eccezione l'**art. 14** (segnalazione), applicabile dall'**11 settembre 2026**, e il **capo IV** (artt. 35-51, organismi notificati), applicabile dall'**11 giugno 2026** (art. 71, par. 2, secondo comma). L'art. 14 e' coperto da `cra-segnalazione-art14`.
- I requisiti essenziali, compresi quelli di gestione delle vulnerabilita', si applicano a **ogni singolo prodotto** al momento della **sua** immissione sul mercato, che sia fabbricato come unita' singola o in serie (considerando 38). Il considerando aggiunge che ogni esemplare di un tipo dovrebbe aver ricevuto tutte le patch e gli aggiornamenti di sicurezza disponibili al momento dell'immissione.
- I prodotti **immessi sul mercato prima dell'11 dicembre 2027** sono soggetti ai requisiti solo se, da quella data, subiscono una **modifica sostanziale** (art. 69, par. 2). La protezione riguarda gli esemplari gia' immessi prima di quella data, non il modello: ogni esemplare dello stesso modello immesso dall'11 dicembre 2027 deve essere conforme (considerando 38). L'art. 14 si applica anche agli esemplari gia' immessi (art. 69, par. 3).
- "Modifica sostanziale": modifica successiva all'immissione che incide sulla conformita' all'allegato I, parte I, o cambia la finalita' prevista per cui il prodotto e' stato valutato (art. 3, punto 30).
- "Immissione sul mercato" e' la **prima** messa a disposizione nel mercato dell'Unione (art. 3, punto 21); "messa a disposizione" e' la fornitura, onerosa o gratuita, nel corso di un'attivita' commerciale (art. 3, punto 22).

- **Chi ha gli obblighi**: il "fabbricante" e' anche chi fa progettare o fabbricare il prodotto e lo commercializza con il proprio nome o marchio (art. 3, punto 13). Un **importatore o distributore** e' ritenuto fabbricante, con gli obblighi degli artt. 13 e 14, quando immette sul mercato il prodotto **con il proprio nome o marchio** o vi apporta una **modifica sostanziale** (art. 21).

Conseguenza operativa: la gap analysis serve per ogni prodotto di cui anche un solo esemplare sara' immesso sul mercato dall'11 dicembre 2027, compresi i modelli gia' in vendita. Fanno eccezione solo gli esemplari immessi prima di quella data e non modificati in modo sostanziale.

## B. Struttura dell'obbligo

L'art. 6 pone **due condizioni cumulative** per la messa a disposizione:

1. il **prodotto** soddisfa l'allegato I, **parte I** (requisiti sulle proprieta' del prodotto), a condizione che sia correttamente installato, mantenuto, usato secondo finalita' prevista o in condizioni ragionevolmente prevedibili e, se applicabile, aggiornato (art. 6, lett. a);
2. i **processi del fabbricante** sono conformi all'allegato I, **parte II** (gestione delle vulnerabilita') (art. 6, lett. b).

L'art. 13, par. 1, ripete la prima condizione come obbligo del fabbricante all'atto dell'immissione; l'art. 13, par. 8, la seconda per tutto il periodo di assistenza.

## C. La valutazione dei rischi decide l'applicabilita' (art. 13, par. 2-4)

- Il fabbricante **effettua** una valutazione dei rischi di cibersicurezza e ne tiene conto in pianificazione, progettazione, sviluppo, produzione, consegna e manutenzione (art. 13, par. 2).
- La valutazione e' **documentata** e aggiornata, se del caso, durante il periodo di assistenza (art. 13, par. 3).
- Contenuto minimo (art. 13, par. 3): analisi dei rischi basata su **finalita' prevista**, **uso ragionevolmente prevedibile**, **condizioni d'uso** (ambiente operativo, attivi da proteggere) e **durata di utilizzo prevista**. Deve indicare:
  - **se, e come**, si applicano i requisiti dell'allegato I, parte I, **punto 2** (lettere a-m);
  - **come** il fabbricante applica la parte I, **punto 1**, e i requisiti di gestione delle vulnerabilita' della **parte II**.
- La valutazione entra nella **documentazione tecnica** (art. 13, par. 4; allegato VII, punto 3).
- Se un requisito essenziale **non e' applicabile**, la documentazione tecnica contiene una **chiara giustificazione** (art. 13, par. 4, ultimo periodo).
- Per prodotti soggetti anche ad altri atti dell'Unione (art. 12), la valutazione puo' far parte della valutazione dei rischi prevista da quegli atti (art. 13, par. 4, secondo periodo). L'art. 12 non e' trascritto in questa skill.

**Asimmetria da non perdere.** La formula "sulla base della valutazione dei rischi ... e ove applicabile" introduce **solo** la parte I, punto 2 (allegato I, parte I, punto 2, alinea). Per la parte I, punto 1, e per la parte II la valutazione dei rischi indica le **modalita'** di applicazione, non decide se applicarle (art. 13, par. 3, ultimo periodo). Questo non rende la parte II applicabile in ogni dettaglio: l'art. 13, par. 4, chiede una chiara giustificazione per **qualsiasi** requisito essenziale non applicabile, l'allegato VII, punto 6, parla di requisiti "applicabili" delle parti I e II, e alcuni punti della parte II contengono condizioni proprie (punto 2: "ove tecnicamente fattibile"; punto 7: "ove applicabile"; art. 13, par. 10, per le versioni successive di software). Una non applicabilita' nella parte II deve quindi poggiare sulla **formulazione del singolo punto** e sulle caratteristiche del prodotto, mai su criteri estranei al testo come il prezzo o l'assenza di sviluppo interno.

Definizioni che reggono l'analisi: "rischio di cibersicurezza" come combinazione di entita' della perdita e probabilita' dell'incidente (art. 3, punto 37); "rischio significativo" (punto 38); "finalita' prevista" (punto 23); "uso ragionevolmente prevedibile" (punto 24); "uso improprio ragionevolmente prevedibile" (punto 25).

## D. Allegato I, parte I - requisiti sulle proprieta' del prodotto

**Punto 1** (sempre): progettato, sviluppato e prodotto per un livello adeguato di cibersicurezza **in base ai rischi**.

**Punto 2** (sulla base della valutazione dei rischi e ove applicabile). Il prodotto:

| Lett. | Cosa chiede il testo | Dettagli letterali da verificare |
|---|---|---|
| a) | messo a disposizione **senza vulnerabilita' sfruttabili note** | "sfruttabile" = utilizzabile efficacemente da un avversario in condizioni operative pratiche (art. 3, punto 41) |
| b) | **configurazione sicura per impostazione predefinita** | possibilita' di **ripristinare lo stato originale**; eccezione solo per accordo con utilizzatore commerciale su prodotto su misura |
| c) | vulnerabilita' affrontabili con **aggiornamenti di sicurezza** | se del caso **automatici**, entro tempo adeguato, **attivi per impostazione predefinita**, con **meccanismo di disattivazione chiaro e facile**, **notifica** degli aggiornamenti disponibili e possibilita' di **rinviarli temporaneamente** |
| d) | protezione dall'**accesso non autorizzato** | meccanismi di controllo (autenticazione, gestione identita' o accessi, elenco non esaustivo) e **segnalazione** degli accessi non autorizzati |
| e) | **riservatezza** dei dati conservati, trasmessi o trattati | ad esempio crittografia a riposo e in transito con meccanismi **all'avanguardia** |
| f) | **integrita'** di dati, comandi, programmi e configurazione | contro manipolazioni non autorizzate e **segnalazione delle corruzioni** |
| g) | **minimizzazione dei dati** | solo dati adeguati, pertinenti e limitati alla finalita' prevista |
| h) | **disponibilita'** delle funzioni essenziali e di base | anche dopo un incidente; resilienza e attenuazione contro denial of service |
| i) | ridurre al minimo l'impatto **su altri dispositivi o reti** | disponibilita' dei servizi forniti da altri |
| j) | **limitare le superfici di attacco** | comprese le interfacce esterne |
| k) | ridurre l'impatto degli incidenti con **tecniche di attenuazione dello sfruttamento** | |
| l) | **registrazione e monitoraggio** delle attivita' interne pertinenti | accesso o modifica di dati, servizi, funzioni; con **meccanismo di disattivazione per l'utilizzatore** |
| m) | **rimozione sicura e permanente** di tutti i dati e impostazioni | e, se i dati sono trasferibili ad altri prodotti, trasferimento sicuro |

Il testo non fissa algoritmi, lunghezze di chiave, tempi di patch o soglie numeriche per nessuna lettera. Ogni parametro concreto viene da norme tecniche o dalla valutazione dei rischi, non dall'allegato I.

## E. Allegato I, parte II - gestione delle vulnerabilita' (processi del fabbricante)

| Punto | Cosa chiede il testo | Dettagli letterali |
|---|---|---|
| 1) | identificare e documentare vulnerabilita' e componenti; **SBOM** | formato **di uso comune e leggibile da dispositivo automatico**, con **almeno le dipendenze di primo livello** |
| 2) | affrontare e correggere **tempestivamente**, anche con aggiornamenti | ove tecnicamente fattibile, aggiornamenti di sicurezza **separati** da quelli di funzionalita' |
| 3) | **prove e riesami** di sicurezza efficaci e **periodici** | |
| 4) | dopo l'aggiornamento, **divulgazione pubblica** delle vulnerabilita' risolte | descrizione, identificazione del prodotto, impatto, gravita', istruzioni per correggere; ritardo ammesso in casi debitamente giustificati finche' gli utilizzatori possono applicare la patch |
| 5) | **politica di divulgazione coordinata** (CVD) | messa in atto **e applicata** |
| 6) | facilitare la condivisione di informazioni sulle vulnerabilita', anche dei componenti di terzi | **indirizzo di contatto** per le segnalazioni |
| 7) | **distribuzione sicura** degli aggiornamenti | correzione tempestiva e, ove applicabile, **automatica** |
| 8) | aggiornamenti di sicurezza diffusi **tempestivamente e gratuitamente** | con **messaggi di avviso** sulle misure da adottare; eccezione solo per accordo con utilizzatore commerciale su prodotto su misura |

"Distinta base del software": registro formale con dettagli e relazioni della catena di approvvigionamento dei componenti software (art. 3, punto 39). La Commissione **puo'** specificare formato ed elementi con atto di esecuzione (art. 13, par. 24): questa skill non ha verificato se sia stato adottato.

[pratica, non norma] Formati SBOM di uso comune sono, per esempio, SPDX e CycloneDX. Il testo non li nomina.

## F. Altri obblighi dell'art. 13 che si verificano insieme all'allegato I

- **Componenti di terzi** (par. 5): dovuta diligenza nell'integrare componenti di terzi, **anche open source** non messi a disposizione nell'ambito di un'attivita' commerciale.
- **Vulnerabilita' in un componente** (par. 6): segnalarla a chi fabbrica o mantiene il componente, correggerla secondo la parte II, e condividere codice o documentazione della correzione col manutentore, se del caso in formato leggibile da dispositivo automatico.
- **Documentazione sistematica** degli aspetti di cibersicurezza, comprese le vulnerabilita' note e le informazioni di terzi; aggiornamento della valutazione dei rischi se del caso (par. 7).
- **Periodo di assistenza** (par. 8):
  - riflette la **durata di utilizzo prevista** (aspettative degli utilizzatori, natura e finalita' del prodotto, diritto dell'Unione sulla durata di vita);
  - puo' tener conto di prodotti analoghi di altri fabbricanti, disponibilita' dell'ambiente operativo, periodi di assistenza dei componenti di terzi, orientamenti ADCO e Commissione;
  - **almeno cinque anni**; se l'uso previsto e' inferiore a cinque anni, pari alla durata di utilizzo prevista;
  - le informazioni usate per determinarlo vanno nella documentazione tecnica (anche allegato VII, punto 4);
  - la Commissione puo' fissare minimi per categorie con atto delegato (non verificato da questa skill).
- **Disponibilita' degli aggiornamenti** (par. 9): ciascun aggiornamento di sicurezza resta disponibile **almeno dieci anni** dal rilascio o per il restante periodo di assistenza, se superiore.
- **Versioni successive di software** (par. 10): la parte II, punto 2, puo' essere garantita solo sull'ultima versione se gli utilizzatori delle versioni precedenti vi hanno **accesso gratuito** e **senza costi aggiuntivi** di adeguamento hardware e software.
- **Archivi pubblici di versioni precedenti** (par. 11): ammessi, con informazione chiara sui rischi del software privo di assistenza.
- **Fine del periodo di assistenza** (par. 19): data finale (almeno **mese e anno**) indicata chiaramente **al momento dell'acquisto**; notifica agli utilizzatori a fine assistenza, ove tecnicamente fattibile.
- **Misure correttive** (par. 21): se il prodotto o i processi non sono conformi all'allegato I, misure correttive immediate, ritiro o richiamo.

## G. Informazioni e istruzioni per l'utilizzatore (art. 13, par. 15-18 e 20; allegato II)

- Identificazione del prodotto: numero di tipo, lotto o serie o altro elemento, o sull'imballaggio o documento di accompagnamento (par. 15).
- Nome o marchio, indirizzo postale, e-mail o altro contatto digitale, sito web se disponibile (par. 16; allegato II, punto 1).
- **Punto di contatto unico**, facilmente identificabile, che lasci scegliere il mezzo di comunicazione senza limitarsi a strumenti automatizzati (par. 17; allegato II, punto 2, insieme alla politica CVD).
- Lingua facilmente comprensibile; informazioni chiare e leggibili; disponibili **almeno dieci anni** o per il periodo di assistenza se superiore, anche online (par. 18).
- Copia della dichiarazione di conformita' UE o dichiarazione semplificata con indirizzo Internet di quella completa (par. 20; allegato II, punto 6).
- Contenuto minimo dell'allegato II: punti 1-9, fra cui finalita' prevista e proprieta' di sicurezza (punto 4), rischi prevedibili anche da uso improprio (punto 5), tipo di assistenza e **data finale del periodo di assistenza** (punto 7), istruzioni su messa in servizio sicura, effetti delle modifiche, installazione degli aggiornamenti, smantellamento ed eliminazione sicura dei dati, disattivazione degli aggiornamenti automatici, informazioni per l'integratore (punto 8, lett. a-f), dove trovare la SBOM se il fabbricante decide di renderla disponibile (punto 9).

Nota: la SBOM va **redatta** sempre (parte II, punto 1), ma la sua **messa a disposizione dell'utilizzatore** e' una scelta del fabbricante (allegato II, punto 9). All'autorita' di vigilanza va fornita su richiesta motivata (allegato VII, punto 8).

## H. Dove confluiscono le evidenze: documentazione tecnica (art. 31; allegato VII)

- Redatta **prima** dell'immissione sul mercato e aggiornata almeno per il periodo di assistenza (art. 31, par. 2).
- Conservata con la dichiarazione UE **almeno dieci anni** dall'immissione o per il periodo di assistenza, se superiore (art. 13, par. 13).
- Elementi dell'allegato VII che si alimentano con la gap analysis di questa skill:
  - punto 2, lett. b): processi di gestione delle vulnerabilita' (SBOM, politica CVD, prova dell'indirizzo di contatto, soluzioni per la distribuzione sicura degli aggiornamenti);
  - punto 3: valutazione dei rischi, comprese le modalita' di applicazione della parte I;
  - punto 4: informazioni per il periodo di assistenza;
  - punto 5: norme armonizzate, specifiche comuni o sistemi di certificazione applicati; **in loro assenza, descrizione delle soluzioni adottate** per le parti I e II;
  - punto 6: **relazioni delle prove** di conformita' alle parti I e II.

## I. Presunzione di conformita' (art. 27, par. 1 e 8)

- Conformita' a **norme armonizzate** i cui riferimenti sono **pubblicati nella GU UE** = presunzione di conformita' ai requisiti dell'allegato I da esse coperti (par. 1).
- Stessa presunzione per certificati o dichiarazioni UE nell'ambito di un **sistema europeo di certificazione** ex Reg. (UE) 2019/881, nella misura in cui coprono i requisiti (par. 8).
- Questa skill **non conosce** quali norme armonizzate siano state pubblicate in GU UE: va verificato alla data della valutazione. Senza norme applicate, l'allegato VII, punto 5, chiede la descrizione delle soluzioni adottate.

## J. Sanzioni (art. 64, par. 1-4)

- Le norme sanzionatorie sono fissate dagli **Stati membri** (par. 1).
- Non conformita' all'**allegato I** e agli obblighi degli **artt. 13 e 14**: fino a **15 000 000 EUR** o, per le imprese, fino al **2,5%** del fatturato mondiale annuo dell'esercizio precedente, se superiore (par. 2).
- Non conformita' fra l'altro all'art. 31, par. 1-4 (documentazione tecnica): fino a 10 000 000 EUR o 2% (par. 3).
- Informazioni inesatte, incomplete o fuorvianti ad autorita' o organismi notificati: fino a 5 000 000 EUR o 1% (par. 4).

I parametri di commisurazione (par. 5) e i paragrafi successivi non sono trascritti. Le norme sanzionatorie italiane non sono fra le fonti lette.

## K. Cosa la fonte letta non dice (non inventarlo)

- **Nessuna soglia numerica tecnica**: tempi massimi di patch, algoritmi, lunghezze di chiave, livelli CVSS.
- **Quali norme armonizzate** coprono quali requisiti, e se siano state pubblicate.
- **Formato SBOM obbligatorio**: dipende da un eventuale atto di esecuzione (art. 13, par. 24) non letto.
- **Minimi di periodo di assistenza per categoria**: dipendono da eventuali atti delegati (art. 13, par. 8) non letti.
- **Regole nazionali italiane** (autorita', procedure, sanzioni): nessun atto nazionale di adeguamento e' fra le fonti lette.
- **Ambito di applicazione ed esclusioni** (art. 2) e **classificazione** (artt. 7-8): vedi `cra-classificazione-pde`.
