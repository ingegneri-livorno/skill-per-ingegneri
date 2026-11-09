# AGENTS.md - cra-requisiti-essenziali-allegato-i

> Convenzioni di dominio per agent che lavorano su questa skill. Per le convenzioni globali del repo vedi `../../AGENTS.md`.

## Dominio

Gap analysis dei **requisiti essenziali di cibersicurezza dell'allegato I** del **Regolamento (UE) 2024/2847 - Cyber Resilience Act** e degli **obblighi del fabbricante dell'art. 13**, applicabili dall'**11 dicembre 2027** (art. 71, par. 2). Target: ingegnere di prodotto, firmware o software, security engineer, responsabile tecnico, compliance manager del fabbricante. Skill sorelle: `cra-classificazione-pde` (ambito, classe, modulo di conformita') e `cra-segnalazione-art14` (notifiche, gia' applicabili dall'11 settembre 2026).

## Fonti autoritative

Una sola fonte, trascritta verbatim in `references/fonti/reg-ue-2024-2847-cra-requisiti-essenziali.md`:

- **Reg. (UE) 2024/2847 (CRA)** - CELEX 32024R2847, via CELLAR con `Accept: application/xhtml+xml` + `Accept-Language: ita`, sha256 `c545dfacd04be16112595c2de51b35c6d6d0329b565b393de581c77b63659f5b` (stesso binario di `cra-segnalazione-art14`).

Estratto operativo: `references/estratti/cra-allegato-i-requisiti-e-obblighi.md` (sezioni A-K).

## Articoli e punti chiave

- **Art. 6**: due condizioni cumulative, prodotto conforme alla parte I e processi conformi alla parte II.
- **Art. 13, par. 2-4**: valutazione dei rischi; decide se e come si applica la **parte I, punto 2**; giustificazione dei requisiti non applicabili nella documentazione tecnica.
- **Allegato I, parte I**: punto 1 (sempre) e punto 2, lettere a)-m) (ove applicabile).
- **Allegato I, parte II**: punti 1-8, non filtrati dalla valutazione dei rischi; eventuale non applicabilita' solo sulla base della formulazione del singolo punto e con giustificazione (art. 13, par. 4).
- **Art. 13, par. 5-11 e 19**: componenti di terzi, periodo di assistenza (minimo cinque anni salvo uso previsto inferiore), disponibilita' degli aggiornamenti per dieci anni, versioni successive, fine assistenza comunicata all'acquisto.
- **Art. 13, par. 15-20 e allegato II**: identificazione, contatti, punto di contatto unico, istruzioni, dichiarazione UE.
- **Art. 21**: importatore o distributore con il proprio marchio, o che apporta una modifica sostanziale, e' fabbricante.
- **Art. 27, par. 1 e 8**: presunzione di conformita' da norme armonizzate pubblicate in GU UE o certificazione europea.
- **Art. 31 e allegato VII**: documentazione tecnica in cui confluiscono le evidenze.
- **Art. 64, par. 1-4**: massimali; norme sanzionatorie nazionali.
- **Considerando 38, art. 69 e 71**: date; i requisiti valgono per ogni esemplare immesso dall'11 dicembre 2027; gli esemplari immessi prima sono soggetti solo se modificati in modo sostanziale dopo quella data.

## Convenzioni specifiche

### Cosa NON fare

- Non usare la valutazione dei rischi per dichiarare non applicabile la parte I, punto 1, o un punto della parte II: "ove applicabile" come filtro di rischio riguarda solo la parte I, punto 2. Non applicabilita' nella parte II solo se il punto stesso la prevede ("ove applicabile", "ove tecnicamente fattibile") e con giustificazione; mai per prezzo o assenza di sviluppo interno.
- Non concludere che un modello immesso prima dell'11 dicembre 2027 sia esente: i requisiti valgono per ogni esemplare immesso da quella data (considerando 38; art. 69, par. 2).
- Non inventare soglie tecniche (tempi di patch, algoritmi, lunghezze di chiave, CVSS): il testo non le contiene.
- Non nominare norme armonizzate come pubblicate in GU UE: l'elenco non e' fra le fonti lette.
- Non far coincidere il periodo di assistenza con la garanzia legale: il criterio del testo e' la durata di utilizzo prevista, con minimo di cinque anni.
- Non trattare la SBOM come documento da consegnare all'utente: va redatta sempre (parte II, punto 1), resa disponibile all'utente solo se il fabbricante lo decide (allegato II, punto 9).
- Non citare atti nazionali italiani di adeguamento al CRA: nessuno e' fra le fonti lette.
- Non classificare il prodotto ne' scegliere il modulo di conformita': rinviare a `cra-classificazione-pde`.

### Cosa fare

- Citare sempre allegato, parte, punto e lettera, oppure articolo e paragrafo.
- Usare cinque stati: soddisfatto / parziale / mancante / non applicabile (giustificato) / da verificare. In dubbio, "da verificare".
- Per ogni requisito indicare l'evidenza che entra nell'allegato VII.
- Marcare **[pratica, non norma]** ogni suggerimento tecnico che non viene dal testo.
- Chiudere con il rinvio al fabbricante, unico responsabile della dichiarazione di conformita' UE.

## Validatori

- Validatore di dominio (product security engineer o ingegnere dell'informazione con esperienza di marcatura CE e CRA) - da identificare per la validazione di Livello 2.

## Stato attuale

- Versione: vedi `CHANGELOG.md` (`0.1.0-alpha`).
- Validazione: Livello 1 (autore + adversarial review).
- Task files: 4 (`imposta-valutazione-rischi`, `gap-analysis-parte-i`, `gap-analysis-parte-ii`, `check-informazioni-utilizzatore`).
- Esempi: 1 conforme + 1 problematico.
