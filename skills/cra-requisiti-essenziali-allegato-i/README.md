# cra-requisiti-essenziali-allegato-i

> Versione: 0.1.0-alpha
> Stato: in sviluppo (Livello 1, autore + review adversariale)

Skill di supporto alla **gap analysis** di un prodotto con elementi digitali (PDE) rispetto ai **requisiti essenziali di cibersicurezza dell'allegato I** del **Regolamento (UE) 2024/2847 - Cyber Resilience Act (CRA)** e agli **obblighi del fabbricante dell'art. 13**, applicabili dall'**11 dicembre 2027** (art. 71, par. 2).

## Target

Ingegneri di prodotto, firmware e software, security engineer, responsabili tecnici e compliance manager di chi immette sul mercato UE hardware o software connesso, compresi importatori e distributori che lo vendono con il proprio marchio (art. 21).

## Cosa fa

Quattro sotto-attivita':

1. **Valutazione dei rischi** (`tasks/imposta-valutazione-rischi.md`): elementi minimi dell'art. 13, par. 3, e matrice di applicabilita' delle lettere a)-m) della parte I, punto 2.
2. **Requisiti di prodotto** (`tasks/gap-analysis-parte-i.md`): verifica lettera per lettera della parte I, con evidenze per l'allegato VII.
3. **Processi di gestione delle vulnerabilita'** (`tasks/gap-analysis-parte-ii.md`): parte II punti 1-8 (SBOM, CVD, aggiornamenti), componenti di terzi, periodo di assistenza.
4. **Informazioni per l'utilizzatore** (`tasks/check-informazioni-utilizzatore.md`): allegato II e obblighi dell'art. 13, par. 15-20.

## Cosa NON fa (limiti noti)

- Non verifica l'ambito, non classifica il prodotto e non sceglie il modulo di valutazione della conformita': usa `cra-classificazione-pde`.
- Non gestisce le notifiche dell'art. 14: usa `cra-segnalazione-art14`.
- Non fissa parametri tecnici (algoritmi, tempi di patch, soglie): il testo non li contiene.
- Non sa quali norme armonizzate siano pubblicate in GU UE.
- Non applica atti delegati o di esecuzione della Commissione (formato SBOM, periodi minimi di assistenza per categoria): non letti.
- Non applica norme nazionali italiane di adeguamento al CRA (sanzioni, autorita'): nessun atto nazionale e' fra le fonti lette; l'art. 64, par. 1, rimette le sanzioni agli Stati membri.
- Non esegue test ne' scansioni: ne legge i risultati.

## Installazione

Per installare la skill in Claude Code:

```bash
ln -s "$(pwd)/skills/cra-requisiti-essenziali-allegato-i" "$HOME/.claude/skills/cra-requisiti-essenziali-allegato-i"
```

Per Codex (OpenAI):

```bash
ln -s "$(pwd)/skills/cra-requisiti-essenziali-allegato-i" "$HOME/.agents/skills/cra-requisiti-essenziali-allegato-i"
```

## Fonti consultate

- **Regolamento (UE) 2024/2847** del Parlamento europeo e del Consiglio del 23 ottobre 2024 (Cyber Resilience Act) - CELEX 32024R2847. ELI: <http://data.europa.eu/eli/reg/2024/2847/oj>.

Dettaglio, SHA256 e path locale in `references/sources.yaml`. Trascrizione verbatim in `references/fonti/`, estratto operativo in `references/estratti/`.

## Disclaimer

Strumento di supporto alla verifica. Non sostituisce il giudizio del professionista che firma la valutazione ne' la responsabilita' del fabbricante, unico titolare della dichiarazione di conformita' UE. Non produce documenti pronti alla firma.

## Changelog

Vedi [CHANGELOG.md](CHANGELOG.md).
