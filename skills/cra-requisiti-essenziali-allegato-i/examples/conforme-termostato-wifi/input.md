# Input - termostato Wi-Fi con app e servizio cloud

Richiesta dell'utente (ingegnere elettronico, responsabile tecnico di una PMI italiana fabbricante):

> Immettiamo sul mercato UE a marzo 2028 un termostato Wi-Fi con app mobile e backend cloud nostro. Abbiamo gia' classificato il prodotto come PDE default con `cra-classificazione-pde`. Vorrei una gap analysis completa sull'allegato I prima di chiudere la documentazione tecnica.

Dati forniti:

- **Prodotto**: termostato (MCU con stack Wi-Fi), app iOS/Android, backend cloud sviluppato dal fabbricante senza il quale la programmazione da remoto non funziona.
- **Finalita' prevista**: regolazione della temperatura domestica, locale e da remoto. Uso improprio prevedibile individuato: installazione in piccoli uffici con rete condivisa.
- **Durata di utilizzo prevista**: 10 anni. **Periodo di assistenza dichiarato**: 10 anni, motivato con la durata d'uso degli impianti termici e il periodo di assistenza del sistema operativo del modulo Wi-Fi (12 anni da contratto col fornitore).
- **Valutazione dei rischi**: documentata, con matrice a)-m) e giustificazioni; aggiornata a ogni rilascio.
- **Configurazione di fabbrica**: nessuna credenziale predefinita, accoppiamento con codice univoco per esemplare stampato sull'etichetta; porta di debug disabilitata in produzione; unico servizio esposto in rete locale per l'accoppiamento, chiuso dopo l'accoppiamento; reset di fabbrica da menu.
- **Aggiornamenti**: OTA firmati, verificati all'avvio e all'installazione; automatici di default, disattivabili dall'app; notifica nell'app con possibilita' di rinviare fino a 7 giorni. Aggiornamenti di sicurezza rilasciati separati dalle nuove funzioni, gratuiti.
- **Dati**: temperatura, programmi, account e-mail; cifratura TLS verso il cloud, cifratura a riposo nel cloud; nessuna geolocalizzazione.
- **Log**: accessi e modifiche di configurazione registrati, consultabili e disattivabili dall'app; tentativi di accesso falliti notificati all'utente.
- **Disponibilita'**: la regolazione locale funziona anche senza connessione; limitazione del traffico verso il cloud.
- **Cancellazione dati**: reset di fabbrica cancella dati locali e dissocia l'account; dall'app si cancella l'account e i dati nel cloud.
- **SBOM**: CycloneDX generata in CI a ogni build, con dipendenze dirette e transitive, confrontata ogni notte con un database di vulnerabilita'.
- **Processi**: PSIRT di 2 persone, policy CVD pubblicata con indirizzo security@ e modulo web; avvisi di sicurezza pubblicati sul sito dopo ogni patch; penetration test esterno annuale e test automatici in CI.
- **Componenti di terzi**: inventario, monitoraggio delle vulnerabilita', segnalazione ai manutentori open source prevista dalla procedura.
- **Istruzioni**: manuale cartaceo breve + pagina web con tutte le voci dell'allegato II; data di fine assistenza "03/2038" sulla confezione e nella scheda del negozio online.
- **Norme armonizzate**: il fabbricante dichiara di seguire una norma tecnica di cui non sa se il riferimento sia pubblicato in GU UE.
