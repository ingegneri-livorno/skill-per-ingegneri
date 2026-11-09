# Input - telecamera IP per uso domestico

Richiesta dell'utente (consulente incaricato da un importatore-marchio che rivende con il proprio marchio una telecamera prodotta in Asia):

> Mettiamo il nostro marchio su una telecamera IP e la vendiamo online dal giugno 2028. Il produttore originale dice che e' "CRA ready". Ci serve una gap analysis sull'allegato I. Per la parte II pensiamo di dichiararla non applicabile: e' un prodotto economico e non facciamo sviluppo software.

Dati forniti:

- **Prodotto**: telecamera Wi-Fi con app e cloud del produttore originale; venduta con il marchio del cliente.
- **Configurazione di fabbrica**: utente `admin` con password `admin` uguale per tutti gli esemplari, cambio password facoltativo; servizio telnet attivo sulla rete locale; interfaccia web su HTTP.
- **Aggiornamenti**: firmware scaricabile manualmente dal sito; nessuna notifica; le correzioni di sicurezza escono solo dentro la release annuale "Pro", venduta come abbonamento.
- **SBOM**: non disponibile; il produttore fornisce un PDF con l'elenco delle librerie principali alla data del 2026.
- **Vulnerabilita'**: nessuna scansione prima del rilascio; il produttore "non e' a conoscenza" di vulnerabilita'.
- **Processi**: nessuna politica CVD; contatto solo tramite chatbot sul sito.
- **Log**: il dispositivo invia log di uso al cloud, senza possibilita' di disattivarli.
- **Reset**: ripristina le impostazioni ma non cancella i video salvati sulla scheda SD ne' dissocia l'account cloud.
- **Periodo di assistenza**: 2 anni "come la garanzia". Durata d'uso tipica della categoria indicata dal cliente: 5-7 anni.
- **Istruzioni**: guida rapida in inglese, senza data di fine assistenza.
- **Valutazione dei rischi**: assente.
