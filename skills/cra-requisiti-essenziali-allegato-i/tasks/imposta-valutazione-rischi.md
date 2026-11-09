# Task: impostare o verificare la valutazione dei rischi di cibersicurezza (art. 13, par. 2-4)

## Obiettivo

Produrre la struttura della valutazione dei rischi di cibersicurezza richiesta dall'art. 13, par. 2-4, o verificare che una valutazione esistente contenga gli elementi minimi. E' il primo task della gap analysis: decide quali requisiti dell'allegato I, parte I, punto 2, si applicano e con quale giustificazione.

## Input richiesti

1. Descrizione del prodotto: hardware, software o entrambi; componenti; soluzioni di elaborazione dati da remoto senza le quali il prodotto non svolge una sua funzione (art. 3, punto 2).
2. **Finalita' prevista**, come risulta da istruzioni, materiale promozionale e documentazione (art. 3, punto 23).
3. **Usi ragionevolmente prevedibili** e **usi impropri ragionevolmente prevedibili** (art. 3, punti 24 e 25).
4. **Condizioni d'uso**: ambiente operativo (casa, ufficio, impianto industriale, rete pubblica), attivi da proteggere (dati personali, comandi, continuita' di servizio, sicurezza fisica).
5. **Durata di utilizzo prevista** del prodotto.
6. Se esiste gia', la valutazione dei rischi attuale e il metodo usato.

Se mancano 2, 4 o 5, chiedili: senza questi la valutazione non ha la base che l'art. 13, par. 3, richiede.

## Fonti

- `../references/estratti/cra-allegato-i-requisiti-e-obblighi.md`, sezioni B, C, D, E.
- `../references/fonti/reg-ue-2024-2847-cra-requisiti-essenziali.md`: art. 13, par. 2, 3, 4, 7; art. 3, punti 2, 23, 24, 25, 37, 38; allegato I; allegato VII, punto 3.

## Procedura

### 1. Verifica gli elementi minimi (art. 13, par. 3)

Una valutazione conforme contiene almeno:

| Elemento | Base testuale | Presente? |
|---|---|---|
| Analisi dei rischi basata sulla **finalita' prevista** | art. 13, par. 3 | |
| ... e sull'**uso ragionevolmente prevedibile** | art. 13, par. 3 | |
| **Condizioni d'uso**: ambiente operativo, attivi da proteggere | art. 13, par. 3 | |
| **Durata di utilizzo prevista** | art. 13, par. 3 | |
| Per ogni lettera a)-m) della parte I, punto 2: **se** si applica e **come** si attua | art. 13, par. 3 | |
| **Come** si applica la parte I, punto 1 | art. 13, par. 3 | |
| **Come** si applicano i requisiti della parte II | art. 13, par. 3 | |
| Giustificazione chiara per ogni requisito **non applicabile** | art. 13, par. 4 | |
| Documentata e inserita nella documentazione tecnica | art. 13, par. 3-4; allegato VII, punto 3 | |
| Aggiornamento previsto durante il periodo di assistenza | art. 13, par. 3 e 7 | |

### 2. Costruisci la matrice di applicabilita' della parte I, punto 2

Per ciascuna lettera a)-m) compila: applicabile si'/no, rischio che la motiva (in termini di entita' della perdita e probabilita', art. 3, punto 37), modalita' di attuazione prevista, evidenza attesa.

Regole:

- **Non applicabile** e' ammesso solo per le lettere della parte I, punto 2, e solo con una giustificazione legata alle caratteristiche del prodotto (per esempio: il prodotto non tratta dati oltre alla propria configurazione, quindi la lett. g) va motivata rispetto a quei soli dati).
- La parte I, punto 1, e la parte II **non** entrano nella matrice di applicabilita' basata sul rischio: per esse si descrivono le modalita' (art. 13, par. 3, ultimo periodo). Se un punto della parte II contiene una condizione propria ("ove applicabile", "ove tecnicamente fattibile") e non ricorre, la giustificazione va comunque scritta (art. 13, par. 4).
- Se la giustificazione e' debole o generica ("il prodotto e' semplice"), classificala **da verificare**.

### 3. Collega la valutazione al ciclo di vita

L'art. 13, par. 2, chiede di tener conto dei risultati in **pianificazione, progettazione, sviluppo, produzione, consegna e manutenzione**. Verifica che la valutazione dica, per ogni fase, quale decisione ha influenzato. Una valutazione scritta dopo lo sviluppo e mai collegata alle decisioni di progetto non soddisfa questa parte del testo.

### 4. Prevedi l'aggiornamento

Art. 13, par. 7: le vulnerabilita' note e le informazioni di terzi vanno documentate e, se del caso, la valutazione aggiornata. Indica chi la aggiorna e quali eventi la fanno riaprire. [pratica, non norma] Eventi tipici: nuova vulnerabilita' in un componente, nuova interfaccia, cambio dell'ambiente operativo, modifica della finalita' (che puo' essere modifica sostanziale, art. 3, punto 30).

## Output

1. Tabella degli elementi minimi (punto 1) con stato per ogni riga.
2. Matrice di applicabilita' a)-m) con rischio, attuazione, evidenza, stato.
3. Elenco delle giustificazioni di non applicabilita' da riportare nella documentazione tecnica.
4. Lacune in ordine di priorita'.
5. Rinvio: la valutazione e' del fabbricante; la skill ne verifica la struttura, non la correttezza tecnica dei rischi stimati.

## Limiti

- Non impone un metodo di analisi dei rischi: il testo non ne indica uno.
- Non stima probabilita' o impatti al posto del fabbricante.
- Non verifica se la valutazione possa confluire in quella prevista da altri atti dell'Unione (art. 13, par. 4, secondo periodo): l'art. 12 e gli altri atti non sono stati letti.
