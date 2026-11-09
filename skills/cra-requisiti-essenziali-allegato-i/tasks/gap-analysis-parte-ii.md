# Task: gap analysis sui processi di gestione delle vulnerabilita' (allegato I, parte II; art. 13)

## Obiettivo

Verificare che i **processi del fabbricante** soddisfino l'allegato I, parte II (art. 6, lett. b), e gli obblighi dell'art. 13 che li completano: componenti di terzi, periodo di assistenza, disponibilita' degli aggiornamenti. La parte II non e' filtrata dalla valutazione dei rischi: "non applicabile" e' ammesso solo dove il punto stesso lo prevede (punto 2, "ove tecnicamente fattibile"; punto 7, "ove applicabile"; art. 13, par. 10) e con la giustificazione dell'art. 13, par. 4.

## Input richiesti

1. Elenco dei componenti software, anche di terzi e open source; esistenza e formato della SBOM; profondita' (solo dipendenze dirette o anche transitive).
2. Processo di triage e correzione delle vulnerabilita': chi lo gestisce, in quanto tempo, come si decide la priorita'.
3. Come vengono rilasciati gli aggiornamenti di sicurezza: separati o insieme alle nuove funzioni, a pagamento o gratuiti, con quale meccanismo di distribuzione e di verifica dell'integrita'.
4. Prove e riesami di sicurezza periodici: quali, con quale frequenza.
5. Politica di divulgazione coordinata (CVD): esiste, e' pubblicata, e' applicata? Indirizzo di contatto per le segnalazioni.
6. Come vengono pubblicati gli avvisi di sicurezza sulle vulnerabilita' risolte.
7. **Periodo di assistenza** dichiarato e **durata di utilizzo prevista** del prodotto, con le informazioni usate per fissarlo.
8. Per quanto tempo restano scaricabili gli aggiornamenti gia' rilasciati.
9. Per il software: politica sulle versioni precedenti (aggiornamento gratuito all'ultima versione?).

## Fonti

- `../references/estratti/cra-allegato-i-requisiti-e-obblighi.md`, sezioni B, E, F, H.
- `../references/fonti/reg-ue-2024-2847-cra-requisiti-essenziali.md`: allegato I, parte II; art. 13, par. 5-11, 19, 24; art. 3, punti 20, 39, 48; allegato VII, punti 2 lett. b), 4.

## Procedura

### 1. Parte II, punto per punto

| Punto | Domanda di controllo (dal testo) |
|---|---|
| 1) | Esiste una SBOM in **formato di uso comune e leggibile da dispositivo automatico**, con **almeno le dipendenze di primo livello**? Le vulnerabilita' dei componenti sono identificate e documentate? |
| 2) | Le vulnerabilita' sono corrette **tempestivamente** in relazione ai rischi? Gli aggiornamenti di sicurezza sono **separati** da quelli di funzionalita', ove tecnicamente fattibile? Se non lo sono, e' motivato perche' non e' fattibile? |
| 3) | Ci sono **prove e riesami efficaci e periodici**? "Periodici" esclude un solo test prima del lancio. |
| 4) | Dopo ogni aggiornamento c'e' una **divulgazione pubblica** con descrizione, prodotto interessato, impatto, gravita' e istruzioni? Se viene ritardata, il ritardo e' motivato e limitato al tempo per applicare la patch? |
| 5) | La politica CVD e' **messa in atto e applicata**, non solo scritta? |
| 6) | Esiste un **indirizzo di contatto** per le segnalazioni, anche sui componenti di terzi? |
| 7) | La **distribuzione** degli aggiornamenti e' **sicura**? E automatica, ove applicabile, per gli aggiornamenti di sicurezza? |
| 8) | Gli aggiornamenti di sicurezza sono **gratuiti** e **tempestivi**, con **messaggi di avviso** sulle misure da adottare? L'eccezione vale solo per un prodotto su misura con accordo con un utilizzatore commerciale. |

Rilievi tipici da discutere col fabbricante:

- correzioni di sicurezza disponibili solo dentro una nuova versione a pagamento: in conflitto con il punto 8 e, per il software, con le condizioni dell'art. 13, par. 10;
- SBOM prodotta una volta in PDF e non mantenuta: non e' "leggibile da un dispositivo automatico" (punto 1) e non serve a identificare le vulnerabilita' nel tempo;
- policy CVD pubblicata ma senza nessuno che riceva le segnalazioni: punto 5 "applicata" e punto 6 non soddisfatti.

[pratica, non norma] Formati SBOM di uso comune: SPDX, CycloneDX. Il testo non li nomina; un eventuale atto di esecuzione ex art. 13, par. 24, potrebbe fissare formato ed elementi e non e' stato verificato da questa skill.

### 2. Componenti di terzi (art. 13, par. 5 e 6)

- Dovuta diligenza sui componenti di terzi, **anche open source non commerciali** (par. 5): come vengono scelti, monitorati, aggiornati?
- Vulnerabilita' trovate in un componente: vengono segnalate al manutentore e la correzione viene condivisa con lui (par. 6)?

### 3. Periodo di assistenza (art. 13, par. 8, 9, 10, 11, 19)

Verifica in quest'ordine:

1. **Durata**: almeno **cinque anni**, salvo uso previsto inferiore, nel qual caso pari alla durata di utilizzo prevista (par. 8, terzo comma). Un periodo inferiore alla durata d'uso prevista, se questa e' di almeno cinque anni, e' un rilievo.
2. **Motivazione**: le informazioni usate per determinarlo sono documentate nella documentazione tecnica (par. 8, quinto comma; allegato VII, punto 4)? Sono quelle che il testo elenca (aspettative degli utilizzatori, natura e finalita', diritto dell'Unione sulla durata di vita; facoltativamente prodotti analoghi, ambiente operativo, assistenza dei componenti di terzi, orientamenti ADCO)?
3. **Disponibilita' degli aggiornamenti**: ciascun aggiornamento di sicurezza resta disponibile almeno **dieci anni** dal rilascio o per il restante periodo di assistenza, se superiore (par. 9).
4. **Versioni successive di software** (par. 10): se si corregge solo l'ultima versione, l'accesso deve essere **gratuito** e **senza costi** di adeguamento di hardware e software.
5. **Comunicazione della fine**: data finale con almeno **mese e anno**, chiara **al momento dell'acquisto**; notifica a fine assistenza ove tecnicamente fattibile (par. 19).

Attenzione: un componente di terzi con assistenza piu' breve del periodo dichiarato e' un fattore che il fabbricante puo' considerare (par. 8, secondo comma), non una ragione per accorciare il periodo sotto il minimo del terzo comma.

### 4. Documentazione

L'allegato VII, punto 2, lett. b), chiede nella documentazione tecnica: SBOM, politica CVD, **prova** della fornitura dell'indirizzo di contatto, descrizione delle soluzioni per la distribuzione sicura degli aggiornamenti. Verifica che ogni processo produca un'evidenza conservabile.

## Output

1. Tabella punti 1-8 con stato (soddisfatto / parziale / mancante / da verificare), cosa manca, evidenza per l'allegato VII.
2. Sezione sul periodo di assistenza con durata, motivazione, disponibilita' degli aggiornamenti e comunicazione della fine.
3. Sezione sui componenti di terzi.
4. Lacune in ordine di priorita'.
5. Promemoria: la gestione delle vulnerabilita' **attivamente sfruttate** ha obblighi di notifica gia' applicabili dall'11 settembre 2026 (art. 71, par. 2; art. 69, par. 3): rinvio a `cra-segnalazione-art14`.

## Limiti

- Non fissa tempi di correzione: il testo dice "tempestivamente" senza numeri.
- Non verifica tecnicamente la SBOM ne' la sicurezza del canale di aggiornamento.
- Non applica eventuali atti delegati o di esecuzione della Commissione (art. 13, par. 8 e 24), non letti.
