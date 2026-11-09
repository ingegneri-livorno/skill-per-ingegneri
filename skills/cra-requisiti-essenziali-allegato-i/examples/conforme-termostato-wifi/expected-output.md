# Output atteso - termostato Wi-Fi

## Precondizioni

- Ambito e classificazione: gia' accertati dal fabbricante con `cra-classificazione-pde` (PDE default). Il backend cloud rientra come soluzione di elaborazione dati da remoto (art. 3, punti 1 e 2).
- Immissione prevista marzo 2028, dopo l'11 dicembre 2027: allegato I e art. 13 si applicano integralmente (art. 71, par. 2).

## Valutazione dei rischi (art. 13, par. 2-4)

Tutti gli elementi minimi presenti: finalita' prevista, uso improprio prevedibile, condizioni d'uso, durata d'uso, matrice a)-m), modalita' per la parte I, punto 1, e per la parte II, aggiornamento a ogni rilascio. **Soddisfatto.**

## Parte I

| Requisito | Stato | Nota |
|---|---|---|
| Punto 1 | soddisfatto | scelte derivate dalla valutazione dei rischi |
| 2 a) | soddisfatto | confronto SBOM con database di vulnerabilita' a ogni build; conservare il rapporto della build di rilascio come evidenza (allegato VII, punto 6) |
| 2 b) | soddisfatto | nessuna credenziale predefinita condivisa, debug disabilitato, reset di fabbrica |
| 2 c) | soddisfatto | automatici di default, disattivabili, notifica, rinvio temporaneo |
| 2 d) | soddisfatto | accoppiamento con codice univoco; segnalazione degli accessi falliti |
| 2 e) | soddisfatto | TLS in transito, cifratura a riposo nel cloud; **da verificare** la cifratura dei dati a riposo sul dispositivo o la sua giustificazione nella valutazione dei rischi |
| 2 f) | soddisfatto | firmware firmato e verificato all'avvio e all'installazione |
| 2 g) | soddisfatto | dati limitati alla funzione |
| 2 h) | soddisfatto | regolazione locale senza connessione |
| 2 i) | soddisfatto | limitazione del traffico |
| 2 j) | soddisfatto | servizio locale chiuso dopo l'accoppiamento |
| 2 k) | da verificare | non descritte tecniche di attenuazione dello sfruttamento: chiedere quali sono attive sul firmware e sull'app |
| 2 l) | soddisfatto | log con disattivazione per l'utente |
| 2 m) | soddisfatto | reset e cancellazione account |

## Parte II e art. 13

Punti 1-8 soddisfatti: SBOM leggibile da macchina con dipendenze oltre il primo livello, aggiornamenti separati e gratuiti, test periodici, avvisi pubblici, CVD applicata con indirizzo di contatto, OTA firmati.

Periodo di assistenza 10 anni, non inferiore alla durata d'uso prevista, motivato e coerente con l'assistenza del componente di terzi (art. 13, par. 8). Da documentare nella documentazione tecnica la politica di conservazione degli aggiornamenti per almeno dieci anni dal rilascio (art. 13, par. 9): **da verificare**, il dato non e' stato fornito.

## Informazioni all'utilizzatore

Allegato II completo sulla pagina web; data di fine assistenza con mese e anno al momento dell'acquisto (art. 13, par. 19). Verificare che la pagina resti online almeno dieci anni o per il periodo di assistenza (art. 13, par. 18).

## Presunzione di conformita'

Il fabbricante non sa se il riferimento della norma tecnica seguita sia pubblicato in GU UE. Finche' non e' verificato, **non contare sulla presunzione dell'art. 27, par. 1**, e descrivere nella documentazione tecnica le soluzioni adottate per ogni requisito (allegato VII, punto 5).

## Lacune in ordine di priorita'

1. Verifica della pubblicazione in GU UE della norma seguita, o descrizione delle soluzioni per requisito (allegato VII, punto 5).
2. Lett. k): documentare le tecniche di attenuazione dello sfruttamento.
3. Lett. e): cifratura a riposo sul dispositivo o giustificazione.
4. Art. 13, par. 9 e 18: politica di conservazione di aggiornamenti e istruzioni.

## Rinvio

Gap analysis di supporto. La conformita' e' dichiarata dal fabbricante sotto la propria responsabilita' dopo la procedura di valutazione della conformita'; i giudizi tecnici restano del professionista che firma la valutazione.
