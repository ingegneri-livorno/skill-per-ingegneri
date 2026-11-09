# Fonte: Regolamento (UE) 2024/2847 (Cyber Resilience Act) - requisiti essenziali e obblighi del fabbricante

## Provenienza

- Atto: **Regolamento (UE) 2024/2847** del Parlamento europeo e del Consiglio del 23 ottobre 2024 relativo a requisiti orizzontali di cibersicurezza per i prodotti con elementi digitali (regolamento sulla cibersicurezza, "Cyber Resilience Act").
- CELEX `32024R2847`, ELI <http://data.europa.eu/eli/reg/2024/2847/oj>.
- Rappresentazione scaricata: **XHTML in lingua italiana** dal repository CELLAR dell'Ufficio delle pubblicazioni UE, <http://publications.europa.eu/resource/celex/32024R2847>, con `Accept: application/xhtml+xml` e `Accept-Language: ita` (743.211 byte). I due header sono dichiarati in `sources.yaml` nei campi `accept` e `accept_language`.
- Binario locale (non committato): `not_in_repo/reg-ue-2024-2847-cra-cellar.xhtml`.
- Accessed: 2026-11-09.

## Identificazione

| Campo | Valore |
|---|---|
| `id` in `sources.yaml` | `reg-ue-2024-2847-cra-requisiti-essenziali` |
| SHA256 del binario | `c545dfacd04be16112595c2de51b35c6d6d0329b565b393de581c77b63659f5b` |
| Versione/edizione | Testo pubblicato in GU UE L del 20 novembre 2024 (versione di pubblicazione, non consolidata), come servito da CELLAR il 2026-11-09 |
| Data di trascrizione | 2026-11-09 |

Lo stesso binario, con lo stesso hash, e' gia' la fonte di `cra-segnalazione-art14` (scaricato il 2026-08-25): il testo servito da CELLAR non e' cambiato fra le due date.

## Perimetro di questa trascrizione

**Inclusi (verbatim)**: considerando 38; art. 3, punti 1, 2, 6, 13, 20, 21, 22, 23, 24, 25, 30, 37, 38, 39, 40, 41, 48; art. 6 (integrale); art. 13 (integrale); art. 21 (integrale); art. 27, paragrafi 1 e 8; art. 31 (integrale); art. 64, paragrafi da 1 a 4; art. 69 (integrale); art. 71 (integrale); allegati I, II e VII (integrali).

**Volutamente esclusi**: considerando diversi dal 38; art. 2 (ambito di applicazione ed esclusioni) e artt. 7-8 con allegati III-IV (classificazione), coperti da `cra-classificazione-pde`; art. 12 (sistemi di IA ad alto rischio); art. 14 e seguenti (segnalazione), coperti da `cra-segnalazione-art14`; artt. 18-20 e 22-26 (altri operatori economici e gestori open source); art. 28 e allegato V-VI (dichiarazione di conformita'); art. 32 e allegato VIII (procedure di valutazione della conformita'); capi IV-VII salvo gli articoli elencati sopra. Dentro gli articoli trascritti in parte l'omissione e' segnalata in linea con un marcatore `[... non trascritti]`.

Il criterio del perimetro e' che sia trascritto **verbatim** cio' che la skill cita: i requisiti essenziali (allegato I), gli obblighi del fabbricante che li reggono (art. 13) e i casi in cui importatori e distributori ne assumono gli obblighi (art. 21), le informazioni all'utilizzatore (allegato II), il contenuto della documentazione tecnica in cui confluiscono le evidenze (art. 31, allegato VII), la presunzione di conformita' (art. 27), le date (artt. 69, 71) e i massimali sanzionatori (art. 64).

Il testo tra fence e' riportato con la tipografia originale della fonte (virgolette caporali, apostrofi tipografici, accenti), estratto in modo meccanico dall'XHTML: i marcatori di elenco (`1)`, `a)`, `1.`) sono riuniti sulla stessa riga del testo che introducono. La prosa di contorno di questo file usa caratteri da tastiera standard.

## Considerando 38

Unico considerando trascritto: chiarisce che i requisiti si applicano a ogni singola unita' al momento della sua immissione sul mercato.

```
(38)

Per garantire che i prodotti con elementi digitali, quando sono immessi sul mercato, non presentino rischi di cibersicurezza per le persone e le organizzazioni, è opportuno stabilire requisiti essenziali di cibersicurezza per tali prodotti. Tali requisiti essenziali di cibersicurezza, compresi i requisiti in materia di gestione delle vulnerabilità, si applicano a ogni singolo prodotto con elementi digitali al momento dell’immissione sul mercato, indipendentemente dal fatto che il prodotto con elementi digitali sia fabbricato come unità singola o in serie. Ad esempio, per un tipo di prodotto, ogni singolo prodotto con elementi digitali dovrebbe aver ricevuto tutte le patch o gli aggiornamenti di sicurezza disponibili per affrontare le questioni di sicurezza pertinenti al momento dell’immissione sul mercato. Qualora i prodotti con elementi digitali vengano successivamente modificati, da mezzi fisici o digitali, in un modo non previsto dal fabbricante nella valutazione dei rischi iniziale e che potrebbe implicare il fatto che essi non rispettino più i requisiti essenziali di cibersicurezza pertinenti, la modifica dovrebbe essere considerata sostanziale. Ad esempio le riparazioni potrebbero essere assimilate a interventi di manutenzione purché non modifichino un prodotto con elementi digitali già immesso sul mercato in maniera tale da poter influire sulla sua conformità ai requisiti applicabili o da modificare la finalità prevista per la quale il prodotto è stato valutato.
```

## Articolo 3 - Definizioni (punti citati dalla skill)

Trascritti solo i punti usati dalla skill; la numerazione e' quella del testo.

```
Articolo 3

Definizioni

Ai fini del presente regolamento si applicano le definizioni seguenti:

1) «prodotto con elementi digitali»: qualsiasi prodotto software o hardware e le relative soluzioni di elaborazione dati da remoto, compresi i componenti software o hardware immesso sul mercato separatamente;

2) «elaborazione dati da remoto»: qualsiasi elaborazione dati a distanza per la quale il software è stato progettato e sviluppato dal fabbricante o sotto la sua responsabilità e la cui assenza impedirebbe al prodotto con elementi digitali di svolgere una delle sue funzioni;

[... punti non trascritti]

6) «componente»: il software o l’hardware destinato a essere integrato in un sistema di informazione elettronico;

[... punti non trascritti]

13) «fabbricante»: una persona fisica o giuridica che sviluppa o fabbrica prodotti con elementi digitali o che fa progettare, sviluppare o fabbricare prodotti con elementi digitali e li commercializza con il proprio nome o marchio, a titolo oneroso, di monetizzazione o gratuito;

[... punti non trascritti]

20) «periodo di assistenza»: il periodo durante il quale un fabbricante garantisce che le vulnerabilità di un prodotto con elementi digitali siano gestite in modo efficace e conformemente ai requisiti essenziali di cibersicurezza di cui all’allegato I, parte II;

21) «immissione sul mercato»: la prima messa a disposizione di un prodotto con elementi digitali sul mercato dell’Unione;

22) «messa a disposizione sul mercato»: la fornitura, a titolo oneroso o gratuito, di un prodotto con elementi digitali perché sia distribuito o usato sul mercato dell’Unione nel corso di un’attività commerciale;

23) «finalità prevista»: l’uso di un prodotto con elementi digitali previsto dal fabbricante, compresi il contesto e le condizioni d’uso specifici, come dettagliati nelle informazioni comunicate dal fabbricante nelle istruzioni per l’uso, nel materiale promozionale o di vendita e nelle dichiarazioni, nonché nella documentazione tecnica;

24) «uso ragionevolmente prevedibile»: un uso che non corrisponde necessariamente alla finalità prevista dal fabbricante nelle istruzioni per l’uso, nel materiale promozionale o di vendita e nelle dichiarazioni, nonché nella documentazione tecnica, ma che è probabile possa derivare da un comportamento umano o da operazioni o interazioni tecniche ragionevolmente prevedibili;

25) «uso improprio ragionevolmente prevedibile»: l’uso di un prodotto con elementi digitali in un modo non conforme alla sua finalità prevista, ma che può derivare da un comportamento umano o da un’interazione con altri sistemi ragionevolmente prevedibili;

[... punti non trascritti]

30) «modifica sostanziale»: una modifica del prodotto con elementi digitali a seguito della sua immissione sul mercato che incide sulla conformità del prodotto con elementi digitali ai requisiti essenziali di cibersicurezza di cui all’allegato I, parte I, o che comporta una modifica della finalità prevista per la quale il prodotto con elementi digitali è stato valutato;

[... punti non trascritti]

37) «rischio di cibersicurezza»: la potenziale perdita o perturbazione causata da un incidente da esprimersi come combinazione dell’entità di tale perdita o perturbazione e della probabilità che si verifichi l’incidente;

38) «rischio di cibersicurezza significativo»: un rischio di cibersicurezza che, in base alle sue caratteristiche tecniche, si può presumere abbia una probabilità elevata di provocare un incidente che potrebbe avere un impatto negativo grave, causando anche notevoli perdite o perturbazioni materiali o non materiali;

39) «distinta base del software»: un registro formale contenente i dettagli e le relazioni della catena di approvvigionamento dei componenti inclusi negli elementi software di un prodotto con elementi digitali;

40) «vulnerabilità»: un punto debole, una suscettibilità o un difetto di prodotti TIC o servizi TIC che può essere sfruttato da una minaccia informatica;

41) «vulnerabilità sfruttabile»: una vulnerabilità che può essere utilizzata efficacemente da un avversario in condizioni operative pratiche;

[... punti non trascritti]

48) «software libero e open source»: un software il cui codice sorgente è condiviso apertamente e che è messo a disposizione nell’ambito di una licenza gratuita e open source che prevede tutti i diritti per renderlo liberamente accessibile, utilizzabile, modificabile e ridistribuibile;

[... punti non trascritti]
```

## Articolo 6 - Requisiti per i prodotti con elementi digitali (integrale)

```
Articolo 6

Requisiti per i prodotti con elementi digitali

I prodotti con elementi digitali sono messi a disposizione sul mercato soltanto se:

a) soddisfano i requisiti essenziali di cibersicurezza di cui all’allegato I, parte I, a condizione che siano correttamente installati, siano oggetto di un’adeguata manutenzione e siano utilizzati conformemente alla loro finalità prevista o in condizioni ragionevolmente prevedibili e, se applicabile, siano stati installati i necessari aggiornamenti di sicurezza, e

b) i processi messi in atto dal fabbricante sono conformi ai requisiti essenziali di cibersicurezza di cui all’allegato I, parte II.
```

## Articolo 13 - Obblighi dei fabbricanti (integrale)

```
Articolo 13

Obblighi dei fabbricanti

1. All’atto dell’immissione sul mercato di un prodotto con elementi digitali, i fabbricanti assicurano che esso sia stato progettato, sviluppato e prodotto conformemente ai requisiti essenziali di cibersicurezza di cui all’allegato I, parte I.

2. Ai fini della conformità al paragrafo 1, i fabbricanti effettuano una valutazione dei rischi di cibersicurezza associati a un prodotto con elementi digitali e tengono conto dei risultati di tale valutazione durante le fasi di pianificazione, progettazione, sviluppo, produzione, consegna e manutenzione del prodotto con elementi digitali, allo scopo di ridurre al minimo i rischi di cibersicurezza, prevenire gli incidenti e ridurne al minimo il loro impatto, anche in relazione alla salute e alla sicurezza degli utilizzatori.

3. La valutazione dei rischi di cibersicurezza è documentata e aggiornata, se del caso, durante un periodo di assistenza da determinare conformemente al paragrafo 8 del presente articolo. Tale valutazione comprende almeno un’analisi dei rischi di cibersicurezza basata sulla finalità prevista e sull’uso ragionevolmente prevedibile del prodotto con elementi digitali, nonché sulle sue condizioni d’uso, quali l’ambiente operativo o gli attivi da proteggere, tenendo conto della durata di utilizzo del prodotto prevista. La valutazione dei rischi di cibersicurezza indica se, ed eventualmente in che modo, i requisiti di sicurezza di cui all’allegato I, parte I, punto 2, sono applicabili al pertinente prodotto con elementi digitali e le modalità di attuazione di tali requisiti sulla base della valutazione dei rischi di cibersicurezza. Indica inoltre le modalità con cui il fabbricante intende applicare l’allegato I, parte I, punto 1, e i requisiti di gestione delle vulnerabilità di cui all’allegato I, parte II.

4. All’atto dell’immissione sul mercato di un prodotto con elementi digitali, il fabbricante include la valutazione dei rischi di cibersicurezza di cui al paragrafo 3 del presente articolo nella documentazione tecnica richiesta a norma dell’articolo 31 e dell’allegato VII. Per i prodotti con elementi digitali di cui all’articolo 12, che sono soggetti anche ad altri atti giuridici dell’Unione, la valutazione dei rischi di cibersicurezza può far parte della valutazione dei rischi prevista da tali atti giuridici dell’Unione. Se alcuni requisiti essenziali di cibersicurezza non sono applicabili al prodotto con elementi digitali, il fabbricante fornisce una chiara giustificazione in tal senso nella suddetta documentazione tecnica.

5. Ai fini dell’adempimento dell’obbligo di cui al paragrafo 1, i fabbricanti esercitano la dovuta diligenza quando integrano componenti provenienti da terzi affinché tali componenti non compromettano la cibersicurezza del prodotto con elementi digitali, anche quando integrano componenti di software liberi e open source che non sono stati messi a disposizione sul mercato nel corso di un’attività commerciale.

6. Quando è individuata una vulnerabilità in un componente, compreso un componente open source, integrato nel prodotto con elementi digitali, i fabbricanti la segnalano alla persona o al soggetto che si occupa della fabbricazione o della manutenzione del componente e affrontano e correggono la vulnerabilità conformemente ai requisiti di gestione delle vulnerabilità di cui all’allegato I, parte II. Qualora abbiano sviluppato una modifica del software o dell’hardware per affrontare la vulnerabilità di tale componente, i fabbricanti condividono il codice o la documentazione pertinenti con la persona o il soggetto che si occupa della fabbricazione o della manutenzione del componente, se del caso in un formato leggibile da un dispositivo automatico.

7. I fabbricanti documentano sistematicamente, in modo proporzionato alla natura e ai rischi di cibersicurezza, gli aspetti pertinenti di cibersicurezza relativi al prodotto con elementi digitali, comprese le vulnerabilità di cui vengono a conoscenza e qualsiasi informazione pertinente fornita da terzi e, se del caso, aggiornano la valutazione dei rischi di cibersicurezza del prodotto.

8. All’atto dell’immissione sul mercato di un prodotto con elementi digitali e per la durata del periodo di assistenza, i fabbricanti garantiscono che le vulnerabilità di tale prodotto, compresi i suoi componenti, siano gestite in modo efficace e in conformità dei requisiti essenziali di cibersicurezza di cui all’allegato I, parte II.

I fabbricanti determinano il periodo di assistenza in modo che rifletta la durata di utilizzo prevista del prodotto, tenendo conto, in particolare, delle ragionevoli aspettative degli utilizzatori, della natura del prodotto, compresa la sua finalità prevista, nonché del pertinente diritto dell’Unione che determina la durata di vita dei prodotti con elementi digitali. Nel determinare il periodo di assistenza, i fabbricanti possono tenere conto anche dei periodi di assistenza dei prodotti con elementi digitali che offrono funzionalità analoghe immessi sul mercato da altri fabbricanti, della disponibilità dell’ambiente operativo, dei periodi di assistenza dei componenti integrati che forniscono funzioni essenziali e che provengono da terzi, nonché degli orientamenti pertinenti forniti dall’apposito gruppo di cooperazione amministrativa (ADCO) istituito a norma dell’articolo 52, paragrafo 15, e dalla Commissione. Le questioni da prendere in considerazione per determinare il periodo di assistenza sono prese in considerazione in modo da garantire la proporzionalità.

Fatto salvo il secondo comma, il periodo di assistenza è di almeno cinque anni. Se si prevede che il prodotto con elementi digitali sarà utilizzato per meno di cinque anni, il periodo di assistenza corrisponde alla durata di utilizzo prevista.

Tenendo conto delle raccomandazioni dell’ADCO di cui all’articolo 52, paragrafo 16, la Commissione può adottare atti delegati conformemente all’articolo 61 al fine di integrare il presente regolamento specificando il periodo minimo di assistenza per determinate categorie di prodotti qualora i dati di vigilanza del mercato suggeriscano l’inadeguatezza dei periodi di assistenza.

I fabbricanti includono nella documentazione tecnica di cui all’allegato VII le informazioni prese in considerazione per determinare il periodo di assistenza di un prodotto con elementi digitali.

I fabbricanti dispongono di politiche e procedure adeguate, comprese politiche di divulgazione coordinata delle vulnerabilità, di cui all’allegato I, parte II, punto 5, per trattare e correggere potenziali vulnerabilità del prodotto con elementi digitali segnalate da fonti interne o esterne.

9. I fabbricanti garantiscono che ciascun aggiornamento di sicurezza di cui all’allegato I, parte II, punto 8, che è stato messo a disposizione degli utilizzatori durante il periodo di assistenza, rimanga disponibile dopo il rilascio per un minimo di dieci anni o per il restante periodo di assistenza, se quest’ultimo è superiore.

10. Il fabbricante che abbia immesso sul mercato versioni successive sostanzialmente modificate di un software può garantire la conformità al requisito essenziale di cibersicurezza di cui all’allegato I, parte II, punto 2, solo per l’ultima versione immessa sul mercato, a condizione che gli utilizzatori delle versioni precedentemente immesse sul mercato abbiano accesso gratuito all’ultima versione immessa sul mercato e non debbano sostenere costi aggiuntivi per adeguare l’ambiente hardware e software in cui utilizzano la versione originale del prodotto.

11. I fabbricanti possono tenere archivi pubblici di software per migliorare l’accesso degli utilizzatori alle versioni precedenti. In questi casi, gli utilizzatori sono informati in modo chiaro e facilmente accessibile dei rischi associati all’uso di software privi di assistenza.

12. Prima di immettere un prodotto con elementi digitali sul mercato, i fabbricanti redigono la documentazione tecnica di cui all’articolo 31.

Essi seguono o fanno eseguire le procedure di valutazione della conformità prescelte di cui all’articolo 32.

Se tale procedura di valutazione della conformità dimostra la conformità del prodotto con elementi digitali ai requisiti essenziali di cibersicurezza di cui all’allegato I, parte I, e dei processi messi in atto dal fabbricante ai requisiti essenziali di cibersicurezza di cui all’allegato I, parte II, i fabbricanti redigono la dichiarazione di conformità UE conformemente all’articolo 28 e appongono la marcatura CE conformemente all’articolo 30.

13. I fabbricanti tengono la documentazione tecnica e la dichiarazione di conformità UE a disposizione delle autorità di vigilanza del mercato per un periodo di almeno dieci anni dalla data di immissione sul mercato del prodotto con elementi digitali o per il periodo di assistenza, se quest’ultimo è superiore.

14. I fabbricanti si assicurano che siano predisposte le procedure necessarie affinché i prodotti con elementi digitali fabbricati nell’ambito di una produzione in serie rimangano conformi al presente regolamento. I fabbricanti tengono adeguatamente conto delle modifiche del processo di sviluppo e di produzione o della progettazione o delle caratteristiche del prodotto con elementi digitali, nonché delle modifiche delle norme armonizzate, dei sistemi europei di certificazione della cibersicurezza o delle specifiche comuni di cui all’articolo 27 con riferimento alle quali è dichiarata la conformità del prodotto con elementi digitali o mediante applicazione delle quali tale conformità è verificata.

15. I fabbricanti garantiscono che i loro prodotti con elementi digitali rechino un numero di tipo, di lotto o di serie o qualsiasi altro elemento che ne consenta l’identificazione, oppure, qualora ciò non sia possibile, che tali informazioni siano fornite sull’imballaggio o in un documento di accompagnamento del prodotto con elementi digitali.

16. I fabbricanti indicano il loro nome, la loro denominazione commerciale registrata o il loro marchio registrato, l’indirizzo postale, l’indirizzo di posta elettronica o altri dati di contatto digitale nonché, se disponibile, il sito web presso cui possono essere contattati, sul prodotto con elementi digitali, sull’imballaggio o in un documento di accompagnamento del prodotto con elementi digitali. Tali informazioni sono incluse anche nelle informazioni e nelle istruzioni per l’utilizzatore di cui all’allegato II. I dati di recapito sono redatti in una lingua facilmente comprensibile dagli utilizzatori e dalle autorità di vigilanza del mercato.

17. Ai fini del presente regolamento, i fabbricanti designano un punto di contatto unico che consenta agli utilizzatori di comunicare direttamente e rapidamente con loro, anche per facilitare la segnalazione di vulnerabilità del prodotto con elementi digitali.

I fabbricanti garantiscono che il punto di contatto unico sia facilmente identificabile dagli utilizzatori. Essi includono inoltre il punto di contatto unico nelle informazioni e istruzioni per l’utilizzatore di cui all’allegato II.

Il punto di contatto unico consente agli utilizzatori di scegliere i mezzi di comunicazione preferiti, senza limitarli agli strumenti automatizzati.

18. I fabbricanti provvedono affinché i prodotti con elementi digitali siano accompagnati dalle informazioni e dalle istruzioni per l’utilizzatore di cui all’allegato II in forma cartacea o elettronica. Tali informazioni e istruzioni sono fornite in una lingua facilmente comprensibile dagli utilizzatori e dalle autorità di vigilanza del mercato. Sono chiare, comprensibili, intelligibili e leggibili. Consentono un’installazione, un funzionamento e un utilizzo sicuri dei prodotti con elementi digitali. I fabbricanti mantengono a disposizione degli utilizzatori e delle autorità di vigilanza del mercato le informazioni e istruzioni per l’utilizzatore di cui all’allegato II per un periodo di almeno dieci anni dalla data in cui il prodotto con elementi digitali è stato immesso sul mercato o per il periodo di assistenza, se quest’ultimo è superiore. Qualora tali informazioni e istruzioni siano fornite online, i fabbricanti garantiscono che siano accessibili, di facile uso e disponibili online per un periodo di almeno dieci anni dalla data in cui il prodotto con elementi digitali è stato immesso sul mercato o per il periodo di assistenza, se quest’ultimo è superiore.

19. I fabbricanti garantiscono che la data finale del periodo di assistenza di cui al paragrafo 8, comprendente almeno il mese e l’anno, sia specificata in modo chiaro e comprensibile al momento dell’acquisto in modo facilmente accessibile e, se del caso, sul prodotto con elementi digitali, sul suo imballaggio o con mezzi digitali.

Ove tecnicamente fattibile alla luce della natura del prodotto con elementi digitali, i fabbricanti inviano una notifica agli utilizzatori per informarli che il loro prodotto con elementi digitali ha raggiunto la fine del periodo di assistenza.

20. I fabbricanti forniscono una copia della dichiarazione di conformità UE o una dichiarazione di conformità UE semplificata con il prodotto con elementi digitali. Se è fornita una dichiarazione di conformità UE semplificata, questa contiene l’esatto indirizzo Internet dove è possibile accedere alla dichiarazione di conformità UE completa.

21. A partire dall’immissione sul mercato e per la durata del periodo di assistenza, i fabbricanti che hanno la certezza o motivo di credere che il prodotto con elementi digitali o i processi messi in atto dal fabbricante non siano conformi ai requisiti essenziali di cibersicurezza di cui all’allegato I adottano immediatamente le misure correttive necessarie per rendere conformi il prodotto con elementi digitali o i processi del fabbricante oppure, a seconda dei casi, per ritirare o richiamare il prodotto.

22. I fabbricanti, su richiesta motivata di un’autorità di vigilanza del mercato, forniscono a tale autorità, in una lingua che può essere facilmente compresa da quest’ultima, tutte le informazioni e la documentazione, in formato cartaceo o elettronico, necessarie a dimostrare la conformità del prodotto con elementi digitali e dei processi messi in atto dal fabbricante ai requisiti essenziali di cibersicurezza di cui all’allegato I. I fabbricanti cooperano con tale autorità, su richiesta di quest’ultima, in merito a qualsiasi misura adottata per eliminare i rischi di cibersicurezza presentati dal prodotto con elementi digitali che hanno immesso sul mercato.

23. Il fabbricante che cessa l’attività e di conseguenza non è in grado di conformarsi al presente regolamento informa, prima che la cessazione dell’attività abbia effetto, le autorità di vigilanza del mercato competenti, nonché, con ogni mezzo disponibile e nella misura del possibile, gli utilizzatori dei prodotti pertinenti con elementi digitali interessati immessi sul mercato, dell’imminente cessazione dell’attività.

24. La Commissione può, mediante atti di esecuzione che tengano conto delle norme e delle migliori pratiche europee o internazionali, specificare il formato e gli elementi della distinta base del software di cui all’allegato I, parte II, punto 1. Tali atti di esecuzione sono adottati secondo la procedura d’esame di cui all’articolo 62, paragrafo 2.

25. Al fine di valutare la dipendenza degli Stati membri e dell’Unione nel suo complesso dai componenti software e, in particolare, dai componenti che si qualificano come software liberi e open source, l’ADCO può decidere di condurre una valutazione della dipendenza a livello dell’Unione per determinate categorie di prodotti con elementi digitali. A tal fine, le autorità di vigilanza del mercato possono chiedere ai fabbricanti di tali categorie di prodotti con elementi digitali di fornire le distinte base del software pertinenti di cui all’allegato I, parte II, punto 1. Sulla base di tali informazioni, le autorità di vigilanza del mercato possono fornire all’ADCO informazioni anonimizzate e aggregate sulle dipendenze in materia di software. L’ADCO presenta una relazione sui risultati della valutazione delle dipendenze al gruppo di cooperazione istituito a norma dell’articolo 14 della direttiva (UE) 2022/2555.
```

## Articolo 21 - Casi in cui gli obblighi dei fabbricanti si applicano agli importatori e ai distributori (integrale)

```
Articolo 21

Casi in cui gli obblighi dei fabbricanti si applicano agli importatori e ai distributori

Un importatore o distributore è ritenuto un fabbricante ai fini del presente regolamento, ed è soggetto agli obblighi di cui agli articoli 13 e 14, quando immette sul mercato un prodotto con elementi digitali con il proprio nome o marchio commerciale o apporta una modifica sostanziale a un prodotto con elementi digitali già immesso sul mercato.
```

## Articolo 27 - Presunzione di conformita' (paragrafi 1 e 8)

```
Articolo 27

Presunzione di conformità

1. I prodotti con elementi digitali e i processi messi in atto dal fabbricante che sono conformi alle norme armonizzate o a parti di esse i cui riferimenti sono stati pubblicati nella Gazzetta ufficiale dell’Unione europea si presumono conformi ai requisiti essenziali di cibersicurezza di cui all’allegato I oggetto di tali norme o parti di esse.

In conformità dell’articolo 10, paragrafo 1, del regolamento (UE) n. 1025/2012, la Commissione chiede a una o più organizzazioni europee di normazione di elaborare norme armonizzate per i requisiti essenziali di cibersicurezza di cui all’allegato I del presente regolamento. Nel preparare richieste di normazione per il presente regolamento, la Commissione si adopera per tenere conto delle norme europee ed internazionali esistenti in materia di cibersicurezza, siano esse in vigore o in corso di elaborazione, al fine di semplificare lo sviluppo delle norme armonizzate, ai sensi del regolamento (UE) n. 1025/2012.

[... paragrafi da 2 a 7 non trascritti]

8. I prodotti con elementi digitali e i processi messi in atto dal fabbricante per i quali sono stati rilasciati un certificato o una dichiarazione di conformità UE nell’ambito di un sistema europeo di certificazione della cibersicurezza adottato a norma del regolamento (UE) 2019/881 si presumono conformi ai requisiti essenziali di cibersicurezza di cui all’allegato I, nella misura in cui tali requisiti siano contemplati dal certificato europeo di cibersicurezza o dalla dichiarazione di conformità UE o da loro parti.

[... paragrafo 9 non trascritto]
```

## Articolo 31 - Documentazione tecnica (integrale)

```
Articolo 31

Documentazione tecnica

1. La documentazione tecnica contiene tutti i dati o i dettagli pertinenti relativi ai mezzi utilizzati dal fabbricante per garantire che il prodotto con elementi digitali e i processi messi in atto dal fabbricante siano conformi ai requisiti essenziali di cibersicurezza di cui all’allegato I. Essa contiene almeno gli elementi di cui all’allegato VII.

2. La documentazione tecnica è redatta prima dell’immissione sul mercato del prodotto con elementi digitali ed è costantemente aggiornata, se del caso, almeno per tutta la durata del periodo di assistenza.

3. Per i prodotti con elementi digitali di cui all’articolo 12 che sono soggetti anche ad altri atti giuridici dell’Unione che prevedono documentazione tecnica, è redatta un’unica documentazione tecnica contenente le informazioni di cui all’allegato VII e le informazioni richieste dai rispettivi atti giuridici dell’Unione.

4. La documentazione tecnica e la corrispondenza relativa a qualsiasi procedura di valutazione della conformità sono redatte in una delle lingue ufficiali dello Stato membro in cui è stabilito l’organismo notificato o in una lingua accettata da quest’ultimo.

5. Alla Commissione è conferito il potere di adottare atti delegati conformemente all’articolo 61 per integrare il presente regolamento aggiungendo elementi da includere nella documentazione tecnica di cui all’allegato VII, al fine di tenere conto degli sviluppi tecnologici e degli sviluppi riscontrati nel processo di attuazione del presente regolamento. A tal fine la Commissione si adopera affinché gli oneri amministrativi a carico delle microimprese e delle piccole e medie imprese siano proporzionati.
```

## Articolo 64 - Sanzioni (paragrafi da 1 a 4)

```
Articolo 64

Sanzioni

1. Gli Stati membri fissano le norme sulle sanzioni applicabili in caso di violazione del presente regolamento e prendono tutti i provvedimenti necessari per assicurarne l’applicazione. Le sanzioni previste devono essere effettive, proporzionate e dissuasive. Gli Stati membri notificano tali norme e misure alla Commissione, senza indugio, e provvedono poi a dare immediata notifica delle eventuali modifiche successive.

2. La non conformità ai requisiti essenziali di cibersicurezza di cui all’allegato I e agli obblighi di cui agli articoli 13 e 14 è soggetta a sanzioni amministrative pecuniarie fino a 15 000 000 EUR o, se l’autore del reato è un’impresa, fino al 2,5 % del fatturato mondiale totale annuo dell’esercizio precedente, se superiore.

3. La non conformità agli obblighi di cui agli articoli da 18 a 23, all’articolo 28, all’articolo 30, paragrafi da 1 a 4, all’articolo 31, paragrafi da 1 a 4, all’articolo 32, paragrafi 1, 2 e 3, all’articolo 33, paragrafo 5, e agli articoli 39, 41, 47, 49 e 53 è soggetta a sanzioni amministrative pecuniarie fino a 10 000 000 EUR o, se l’autore del reato è un’impresa, fino al 2 % del fatturato mondiale totale annuo dell’esercizio precedente, se superiore.

4. La fornitura di informazioni inesatte, incomplete o fuorvianti agli organismi notificati e alle autorità di vigilanza del mercato è soggetta a sanzioni amministrative pecuniarie fino a 5 000 000 EUR o, se l’autore del reato è un’impresa, fino all’1 % del fatturato mondiale totale annuo dell’esercizio precedente, se superiore.

[... paragrafi da 5 a 10 non trascritti]
```

## Articolo 69 - Disposizioni transitorie (integrale)

```
Articolo 69

Disposizioni transitorie

1. I certificati di esame UE del tipo e le decisioni di approvazione rilasciati in relazione ai requisiti di cibersicurezza per i prodotti con elementi digitali soggetti ad altra normativa di armonizzazione dell’Unione diversa dal presente regolamento rimangono validi fino all’11 giugno 2028, a meno che non scadano prima di tale data o non sia altrimenti disposto in tali altre normative di armonizzazione dell’Unione, nel qual caso rimangono validi come indicato in tali normative.

2. I prodotti con elementi digitali immessi sul mercato prima dell’11 dicembre 2027 sono soggetti ai requisiti stabiliti nel presente regolamento solo se, a decorrere da tale data, tali prodotti sono soggetti a una modifica sostanziale.

3. In deroga al paragrafo 2 del presente articolo, gli obblighi di cui all’articolo 14 si applicano a tutti i prodotti con elementi digitali che rientrano nell’ambito di applicazione del presente regolamento e che sono stati immessi sul mercato prima dell’11 dicembre 2027.
```

## Articolo 71 - Entrata in vigore e applicazione (integrale)

```
Articolo 71

Entrata in vigore e applicazione

1. Il presente regolamento entra in vigore il ventesimo giorno successivo alla pubblicazione nella Gazzetta ufficiale dell’Unione europea.

2. Il presente regolamento si applica dall’11 dicembre 2027.

Tuttavia, l’articolo 14 si applica a decorrere dall’11 settembre 2026 e il capo IV (articoli da 35 a 51) si applica a decorrere dall’11 giugno 2026.
```

## Allegato I - Requisiti essenziali di cibersicurezza (integrale)

```
ALLEGATO I

REQUISITI ESSENZIALI DI CIBERSICUREZZA

Parte I Requisiti di cibersicurezza relativi alle proprietà dei prodotti con elementi digitali

1) I prodotti con elementi digitali sono progettati, sviluppati e prodotti in modo da garantire un livello adeguato di cibersicurezza in base ai rischi.

2) Sulla base della valutazione dei rischi di cibersicurezza di cui all’articolo 13, paragrafo 2, e ove applicabile, i prodotti con elementi digitali:

a) sono messi a disposizione sul mercato senza vulnerabilità sfruttabili note;

b) sono messi a disposizione sul mercato con una configurazione sicura per impostazione predefinita, salvo diverso accordo tra il fabbricante e l’utilizzatore commerciale in relazione a un prodotto su misura con elementi digitali, con la possibilità di ripristinare il prodotto allo stato originale;

c) garantiscono che le vulnerabilità possano essere affrontate mediante aggiornamenti di sicurezza, anche, se del caso, mediante aggiornamenti di sicurezza automatici installati entro un periodo di tempo adeguato, abilitato come impostazione predefinita, con un meccanismo di disattivazione chiaro e di facile utilizzo, attraverso la notifica agli utilizzatori degli aggiornamenti disponibili e la possibilità di rinviarli temporaneamente;

d) garantiscono la protezione dall’accesso non autorizzato mediante adeguati meccanismi di controllo, tra cui, a titolo esemplificativo ma non esaustivo, sistemi di autenticazione e di gestione dell’identità o dell’accesso, e segnalano eventuali accessi non autorizzati;

e) proteggono la riservatezza dei dati personali o di altro tipo conservati, trasmessi o altrimenti trattati, ad esempio criptando i pertinenti dati a riposo o in transito mediante meccanismi all’avanguardia, e utilizzando altri mezzi tecnici;

f) proteggono l’integrità dei dati personali o di altro tipo conservati, trasmessi o altrimenti trattati, dei comandi, dei programmi e della configurazione da qualsiasi manipolazione o modifica non autorizzata da parte dell’utilizzatore, e segnalano le corruzioni;

g) trattano solo dati, personali o di altro tipo, adeguati, pertinenti e limitati a quanto necessario in relazione alla finalità prevista del prodotto con elementi digitali («minimizzazione dei dati»);

h) proteggono la disponibilità delle funzioni essenziali e di base, anche dopo un incidente, anche attraverso misure di resilienza e di attenuazione contro gli attacchi di negazione del servizio (denial of service);

i) riducono al minimo l’impatto negativo dei prodotti stessi o dei dispositivi connessi sulla disponibilità dei servizi forniti da altri dispositivi o reti;

j) sono progettati, sviluppati e prodotti per limitare le superfici di attacco, comprese le interfacce esterne;

k) sono progettati, sviluppati e prodotti per ridurre l’impatto degli incidenti utilizzando meccanismi e tecniche di attenuazione dello sfruttamento adeguati;

l) forniscono informazioni sulla sicurezza registrando e monitorando le attività interne pertinenti, compresi l’accesso a dati, servizi o funzioni o la modifica degli stessi, con un meccanismo di disattivazione per l’utilizzatore;

m) offrono agli utenti la possibilità di rimuovere in modo sicuro e agevole, su base permanente, tutti i dati e tutte le impostazioni e, qualora tali dati possano essere trasferiti ad altri prodotti o sistemi, garantiscono che ciò avvenga in modo sicuro.

Parte II Requisiti di gestione delle vulnerabilità

I fabbricanti di prodotti con elementi digitali:

1) identificano e documentano le vulnerabilità e i componenti contenuti nel prodotto con elementi digitali, redigendo anche una distinta base del software in un formato di uso comune e leggibile da un dispositivo automatico, che includa almeno le dipendenze di primo livello del prodotto;

2) in relazione ai rischi posti dai prodotti con elementi digitali, affrontano e correggono tempestivamente le vulnerabilità, anche fornendo aggiornamenti di sicurezza; ove tecnicamente fattibile, nuovi aggiornamenti di sicurezza sono forniti separatamente dagli aggiornamenti della funzionalità;

3) effettuano prove e riesami efficaci e periodici della sicurezza del prodotto con elementi digitali;

4) una volta reso disponibile un aggiornamento di sicurezza, condividono e divulgano pubblicamente informazioni sulle vulnerabilità risolte, compresi una descrizione delle vulnerabilità, informazioni che consentano agli utilizzatori di identificare il prodotto con elementi digitali interessato, l’impatto delle vulnerabilità, la loro gravità e informazioni chiare e accessibili che aiutino gli utilizzatori a correggere le vulnerabilità; in casi debitamente giustificati, qualora ritengano che i rischi di sicurezza legati alla divulgazione siano superiori ai benefici in termini di sicurezza, i fabbricanti possono ritardare la divulgazione di informazioni su una vulnerabilità risolta fino a quando gli utilizzatori non abbiano avuto la possibilità di applicare la pertinente patch;

5) mettono in atto e applicano una politica di divulgazione coordinata delle vulnerabilità;

6) adottano misure per facilitare la condivisione di informazioni sulle potenziali vulnerabilità nel loro prodotto con elementi digitali e nei componenti di terzi contenuti in tale prodotto, fornendo anche un indirizzo di contatto per la segnalazione delle vulnerabilità individuate nel prodotto con elementi digitali;

7) prevedono meccanismi per distribuire in modo sicuro gli aggiornamenti dei prodotti con elementi digitali, per garantire che le vulnerabilità siano corrette o attenuate in modo tempestivo e, ove applicabile per gli aggiornamenti di sicurezza, in modo automatico;

8) garantiscono che, qualora disponibili, siano diffusi tempestivamente e gratuitamente, salvo diversamente convenuto tra un fabbricante e un utilizzatore commerciale in relazione a un prodotto su misura con elementi digitali, aggiornamenti di sicurezza per risolvere i problemi di sicurezza individuati, accompagnati da messaggi di avviso che forniscano agli utilizzatori le informazioni pertinenti, comprese le potenziali misure da adottare.
```

## Allegato II - Informazioni e istruzioni per l'utilizzatore (integrale)

```
ALLEGATO II

INFORMAZIONI E ISTRUZIONI PER L’UTILIZZATORE

Il prodotto con elementi digitali è accompagnato, come minimo, dagli elementi seguenti:

1. il nome, la denominazione commerciale registrata o il marchio registrato del fabbricante e l’indirizzo postale, l’indirizzo di posta elettronica o altro contatto digitale nonché, ove disponibile, il sito web a cui il fabbricante può essere contattato;

2. il punto di contatto unico dove è possibile segnalare e ricevere informazioni sulle vulnerabilità del prodotto con elementi digitali e dove è possibile trovare la politica del fabbricante sulla divulgazione coordinata delle vulnerabilità;

3. nome e tipo e qualsiasi altra informazione che consenta l’identificazione univoca del prodotto con elementi digitali;

4. la finalità prevista del prodotto con elementi digitali, compreso l’ambiente di sicurezza fornito dal fabbricante, nonché le funzionalità essenziali del prodotto e le informazioni sulle proprietà di sicurezza;

5. qualsiasi circostanza nota o prevedibile connessa all’uso del prodotto con elementi digitali in conformità alla sua finalità prevista o in condizioni di uso improprio ragionevolmente prevedibile, che possa comportare rischi di cibersicurezza significativi;

6. se del caso, l’indirizzo Internet dove è possibile accedere alla dichiarazione di conformità UE;

7. il tipo di assistenza tecnica di sicurezza offerta dal fabbricante e la data finale del periodo di assistenza durante il quale gli utilizzatori possono aspettarsi che le vulnerabilità siano gestite e di ricevere gli aggiornamenti di sicurezza;

8. istruzioni dettagliate o un indirizzo Internet che rimandi a tali istruzioni e informazioni su quanto segue:

a) le misure necessarie durante la prima messa in servizio e per tutta la durata del prodotto con elementi digitali per garantirne l’uso sicuro;

b) in che modo le modifiche del prodotto con elementi digitali possono influire sulla sicurezza dei dati;

c) le modalità di installazione degli aggiornamenti rilevanti per la sicurezza;

d) lo smantellamento sicuro del prodotto con elementi digitali, comprese le informazioni sulle modalità di eliminazione sicura dei dati degli utilizzatori

e) come può essere disattivata l’impostazione predefinita che consente l’installazione automatica degli aggiornamenti di sicurezza, come richiesto nell’allegato I, parte I, punto 2, lettera c);

f) se il prodotto con elementi digitali è destinato all’integrazione in altri prodotti con elementi digitali, le informazioni necessarie affinché l’integratore soddisfi i requisiti essenziali di cibersicurezza di cui all’allegato I e i requisiti di documentazione di cui all’allegato VII.

9. Se il fabbricante decide di mettere a disposizione dell’utilizzatore la distinta base del software, informazioni sul luogo in cui è possibile accedere a tale distinta.
```

## Allegato VII - Contenuto della documentazione tecnica (integrale)

```
ALLEGATO VII

CONTENUTO DELLA DOCUMENTAZIONE TECNICA

La documentazione tecnica di cui all’articolo 31 include almeno le informazioni seguenti, a seconda dell’applicabilità al pertinente prodotto con elementi digitali:

1. una descrizione generale del prodotto con elementi digitali, tra cui:

a) la finalità prevista;

b) versioni del software importanti per la conformità ai requisiti essenziali di cibersicurezza;

c) se il prodotto con elementi digitali consiste di un prodotto hardware, fotografie o illustrazioni che mostrino le caratteristiche esterne, la marcatura e la disposizione interna;

d) informazioni e istruzioni per l’utilizzatore, come indicato nell’allegato II;

2. una descrizione della progettazione, dello sviluppo e della produzione del prodotto con elementi digitali e dei processi di gestione delle vulnerabilità, tra cui:

a) le informazioni necessarie sulla progettazione e sullo sviluppo del prodotto con elementi digitali, compresi, se del caso, disegni e schemi e una descrizione dell’architettura del sistema che spieghi in che modo i componenti software si basano l’uno sull’altro o si alimentano reciprocamente e si integrano nel processo complessivo;

b) le informazioni necessarie e specifiche sui processi di gestione delle vulnerabilità messi in atto dal fabbricante, tra cui la distinta base del software, la politica di gestione della divulgazione coordinata delle vulnerabilità, la prova della fornitura di un indirizzo di contatto per la segnalazione delle vulnerabilità e una descrizione delle soluzioni tecniche scelte per la distribuzione sicura degli aggiornamenti;

c) le informazioni necessarie e specifiche relative ai processi di produzione e monitoraggio del prodotto con elementi digitali e alla convalida di tali processi;

3. una valutazione dei rischi di cibersicurezza a fronte dei quali il prodotto con elementi digitali è progettato, sviluppato, prodotto, consegnato e sottoposto a manutenzione, a norma dell’articolo 13, incluse le modalità di applicazione dei requisiti essenziali di cibersicurezza di cui all’allegato I, parte I;

4. informazioni pertinenti di cui si è tenuto conto per determinare il periodo di assistenza a norma dell’articolo 13, paragrafo 8, del prodotto con elementi digitali;

5. un elenco delle norme armonizzate applicate integralmente o in parte, i cui riferimenti sono stati pubblicati nella Gazzetta ufficiale dell’Unione europea, delle specifiche comuni di cui all’articolo 27 del presente regolamento o dei sistemi europei di certificazione della cibersicurezza adottati conformemente al regolamento (UE) 2019/881 a norma dell’articolo 27, paragrafo 8, del presente regolamento e, qualora non siano stati applicati tali norme armonizzate, specifiche comuni o sistemi europei di certificazione della cibersicurezza, le descrizioni delle soluzioni adottate per soddisfare i requisiti essenziali di cibersicurezza di cui all’allegato I, parti I e II, compreso un elenco delle altre pertinenti specifiche tecniche applicate. In caso di applicazione parziale delle norme armonizzate, delle specifiche comuni o dei sistemi europei di certificazione della cibersicurezza, la documentazione tecnica specifica le parti che sono state applicate;

6. le relazioni delle prove effettuate per verificare la conformità del prodotto con elementi digitali di cibersicurezza e dei processi di gestione delle vulnerabilità ai requisiti essenziali applicabili di cui all’allegato I, parti I e II;

7. una copia della dichiarazione di conformità UE;

8. se del caso, la distinta base del software, a seguito di una richiesta motivata di un’autorità di vigilanza del mercato, a condizione che ciò sia necessario affinché tale autorità possa verificare la conformità ai requisiti essenziali di cibersicurezza di cui all’allegato I.
```

