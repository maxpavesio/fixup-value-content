# FIXUP · Esempio Report Strategico Google Ads

**Cliente:** Caso multi-brand anonimizzato (Cliente A · Servizi locali + Cliente B · E-commerce nicchia)
**Tipo deliverable:** Audit strutturale account · Accorpamento · Architettura unica · Copy pronti al lancio
**Data esempio:** Aprile 2026
**Pagine equivalenti:** 28 sezioni · 6 capitoli operativi

> Versione anonimizzata di un report reale FIXUP. Scopo: mostrare struttura, profondità e formato del deliverable tipico durante una fase di audit + restructuring account Google Ads. Tutti i nomi, ID e KW specifiche sono stati sostituiti con placeholder.

---

## 📋 Indice

1. **Sintesi esecutiva & KPI** — pag. 03
2. **Struttura account unica** — pag. 04
3. **Audit keyword e search terms** — pag. 05
4. **Liste negative pronte all'uso** — pag. 09
5. **Keyword set finali per campagna** — pag. 13
6. **Copy annunci RSA + PMax** — pag. 17

> Il piano di lancio operativo (timeline, fasi, scaling) è gestito separatamente in fase di kick-off progetto. Questo report copre la parte strategico-creativa.

---

## 01 · Sintesi esecutiva

### Performance attuale · LAST_30_DAYS (situazione pre-intervento)

| Metric | Valore |
|---|---|
| Spesa totale | €2.683 |
| Conversioni | 280 |
| CPA medio | €9,58 |
| Keyword attive | 508 |

### Account a confronto

| Account | Customer ID | Spesa | Conv. | CPA | Stato |
|---|---|---|---|---|---|
| Cliente B (e-com) | YYY-YYY-YYYY | €244 | 73 | €3,35 | 🟢 Performante |
| Cliente A (servizi) | XXX-XXX-XXXX | €2.439 | 207 | €11,77 | 🟡 Da ottimizzare |

### Problemi rilevati

#### 🔴 CRITICO · Campagna prodotto-specifico (Cliente A)
**€395 spesi in 30 giorni con 0 conversioni.** KW concentrate su modelli prodotto specifici. L'utente cerca scheda tecnica, non installatore.

#### 🟡 ATTENZIONE · Campagna chiamate-sito (Cliente A)
196 KW miste, di cui 15+ BROAD generiche (`[brand top 1]`, `[brand top 2]`, `fai da te`, `tutorial`) e 28 KW DIY. **CPA €39 vs target €25.**

#### 🟡 ATTENZIONE · Campagna ricerca brand (Cliente B)
**62% delle 112 KW sono brand competitor diretti** (8+ competitor brand) → traffico fuori target.

#### 🟠 CANNIBALIZZAZIONE
2 PMax attive sullo stesso brand Cliente A. **Tenerne una sola** post-merge per ottimizzare il learning.

### Target post-accorpamento · 90 giorni

| KPI | Baseline attuale | Target | Variazione |
|---|---|---|---|
| Conversioni mensili | ~280 | 330+ | **+18%** |
| CPA medio | €9,58 | €8,00–€9,00 | **−12%** |
| Spesa mensile | €2.683 | €3.000 | +12% |
| Search Impr. Share core | n/a | >65% | nuovo KPI |

---

## 02 · Struttura account unica

**Architettura proposta:** 1 account · 2 brand · 3 linee servizio · 5 campagne iniziali + 2 in fase 2

### Account Google Ads unico
**Cliente A SRL · XXX-XXX-XXXX** (mantenuto come master, accorpato con Cliente B)

### Mappa logica

```
Account Master
├── Brand Cliente A (servizi locali)
│   ├── Linea servizio 1 (urgenza/intervento)  → Search
│   └── Linea servizio 2 (sostituzione/installazione) → Search + PMax + DemGen Fase 2
│
└── Brand Cliente B (e-com prodotto nicchia)
    └── Linea servizio 3 (vendita prodotto core) → Search + PMax + DemGen Fase 2
```

### Sintesi struttura

| Numero | Cosa |
|---|---|
| 2 | Brand |
| 3 | Linee servizio |
| 5 | Campagne iniziali |
| +2 | DemGen fase 2 |

### Logica di lancio in 2 fasi

**FASE 1 · Lancio iniziale (5 campagne)**
- CA_Search_LineaServizio1 · €15/g
- CA_Search_LineaServizio2 · €15/g
- CA_PMax_LineaServizio2 · €25/g
- CB_Search_Prodotto · €10/g
- CB_PMax_Prodotto · €15/g

**Totale: €80/giorno · €2.400/mese**

**FASE 2 · Espansione DemGen (gate dopo 30 giorni)**
- Si valuta come stanno deliverando le PMax sui due brand
- Se PMax si stabilizza con CPA in target → DemGen per estendere awareness/consideration
- Se PMax satura la domanda esistente → DemGen necessaria per aprire nuovi segmenti
- Budget aggiuntivo previsto: €20/giorno (€10 per brand)

### Naming convention

Pattern unico: `{BRAND}_{TIPO}_{SERVIZIO}`

| Brand | Tipo | Servizio | Nome finale |
|---|---|---|---|
| CA | Search | LineaServizio1 | `CA_Search_LineaServizio1` |
| CA | Search | LineaServizio2 | `CA_Search_LineaServizio2` |
| CA | PMax | LineaServizio2 | `CA_PMax_LineaServizio2` |
| CB | Search | Prodotto | `CB_Search_Prodotto` |
| CB | PMax | Prodotto | `CB_PMax_Prodotto` |

---

## 03 · Audit keyword e search terms

### Panoramica campagne attive (pre-intervento)

| Campagna | Account | Tipo | Spesa 30g | Conv. | CPA | Verdetto |
|---|---|---|---|---|---|---|
| Ricerca_lead | CB | Search | €244 | 73 | €3,35 | 🟢 OK · base buona |
| Chiamate-Sito | CA | Search | €275 | 7 | €39,27 | 🟡 KW caotiche |
| Ricerca_lead_LineaServizio2 | CA | Search | €395 | 0 | — | 🔴 CRITICO |
| Agency precedente · PMax | CA | PMax | €1.069 | 134 | €7,98 | 🟢 Driver principale |
| Website traffic · PMax-3 | CA | PMax | €699 | 67 | €10,44 | 🟠 Cannibalizza driver |

### Cliente B · Campagna Ricerca_lead · 112 KW

**COSA FUNZIONA:**
- Brand exact match → Quality Score 10
- KW core: `[KW core 1]`, `[KW core 2]`, `[KW core 3]`, `[KW core 4]` → QS 3-5

**COSA NON FUNZIONA:**
- 62% delle KW sono brand competitor (8+ marchi) → traffico fuori target
- KW informazionali alto costo zero conv: `[KW informazionale 1]`, `[KW informazionale 2]`, `[KW informazionale 3]`
- KW DIY: `[KW DIY 1]`, `[KW DIY 2]`
- KW aggregatori: `[KW aggregatore 1]`, `[KW aggregatore 2]`

**DA FARE:**
- Pausare tutte le brand competitor exact (mantenere solo se prevista campagna dirottamento dedicata)
- Pausare KW informazionali e DIY
- Tenere e potenziare core: `[KW core 1-4]` + varianti exact + phrase
- Aggiungere KW geo: `[KW core 1] [città provincia]`, `installazione [prodotto] [capoluogo]`

### Cliente A · Campagna Chiamate-Sito · 196 KW

**COSA FUNZIONA:**
- KW geo locali QS 1-4: `[servizio] [capoluogo]`, `pronto intervento [servizio] [capoluogo]`, `[servizio] h24 [capoluogo]`
- KW frazioni: `[servizio] [zona1]`, `[servizio] [zona2]`, `[servizio] [zona3]`

**COSA NON FUNZIONA · CATASTROFE STRUTTURALE:**
- 15+ KW BROAD generiche spaccano il budget: `[brand top 1-7]`, `fai da te`, `gratis`, `pulire`, `pulizia`, `istruzioni`, `tutorial`, `video`, `modulo pdf` → impossibile QS decente
- Servizio "[secondario]" (12 KW) NON è il focus dichiarato — togliere
- KW "errore [codice]" (12 KW) → utenti cercano riparazione/reset, non sostituzione
- KW "come [verbo]/[verbo]/[verbo]" (28 KW) → 100% DIY informazionale
- Brand assistenza specifici (8+ marchi) → cercano installatore SPECIFICO, non Cliente A
- KW [servizio secondario] (10 KW) → fuori scope dichiarato

**DA FARE:**
- Riscrivere campagna **da zero** con SOLO ad group geo. KW core da tenere:
  - `[servizio] [capoluogo]` + varianti città/zona (phrase)
  - `pronto intervento [servizio] [zona]`
  - `[servizio] urgente`, `[servizio] 24 ore`, `[servizio] h24`
  - `[riparazione tipo 1] [capoluogo]`, `[riparazione tipo 2] [capoluogo]`, `[riparazione tipo 3] [capoluogo]`, `sos [servizio] [capoluogo]`

### Cliente A · Campagna LineaServizio2 · 200+ KW

**🔴 CATASTROFICO · 0 conversioni in 30 giorni con €395 spesi.** La struttura attuale non funziona. CPC medio €5,35, segno chiaro di Quality Score basso e mismatch tra annuncio e intent.

**COSA NON FUNZIONA:**
- 90% delle KW sono modelli specifici (`[modello 1]`, `[modello 2]`, `[modello 3]`, `[modello 4]`, `[modello 5]`...) → utente cerca scheda tecnica/prezzo prodotto, non installatore
- KW "bonus/incentivi/detrazione" (40+ KW) → utenti in fase informativa, non pronti
- KW "preventivo" mancano quasi del tutto

**DA FARE:**
Riscrivere con focus **transazionale + locale**:
- **Core:** `sostituzione [prodotto] [capoluogo]`, `cambio [prodotto] [capoluogo]`, `installazione [prodotto] [capoluogo]`, `preventivo sostituzione [prodotto]`
- **Modelli generici (no specifici):** `[prodotto] [tipo] prezzo installazione`, `quanto costa cambiare [prodotto]`
- **Brand top installati (3-4 max):** `installazione [prodotto] [brand top 1] [capoluogo]`, `installazione [prodotto] [brand top 2] [capoluogo]`

Pausare tutte le KW modello specifico → trasferire in PMax (gestisce shopping intent meglio).

### PMax · Search terms intercettati · storici

**TERMINI AD ALTA CONVERSIONE (Cliente A):**

| Termine | Click | Conv. | Note |
|---|---|---|---|
| `[brand cliente A] [capoluogo]` | 406 | 64,8 | Brand search · ottimo |
| `[brand top 1] [capoluogo]` | 311 | 88 | Brand prodotto + geo |
| `pulizia [prodotto] [capoluogo]` | 95 | 15,3 | Servizio chiaro |
| `[servizio] [capoluogo]` | 38 | 14 | Categoria core |
| `[brand cliente A] [capoluogo] pronto intervento` | 8 | 5 | Pronto intervento |

**TERMINI DA ESCLUDERE A LIVELLO ACCOUNT:**
- `[brand X] assistenza clienti`, `[brand Y] assistenza clienti`, `[brand Z] centro assistenza` → cercano supporto produttore
- `[servizio] [comune fuori area 1]`, `[servizio] [comune fuori area 2]` → fuori area servita
- `pulizia [prodotto altro]`, `manutenzione [prodotto altro]` → 0 conv su 150+ impressioni
- `tecnico [prodotto] vicino a me`, `[brand] [zona] [via]` → scarso intento

---

## 04 · Liste negative pronte all'uso

> Le tre liste vanno create come **shared negative lists** in Google Ads e applicate selettivamente. Non vanno aggiunte come negativi a livello campagna singola — riduce la manutenibilità nel tempo.

### Lista A · GLOBALE (account-level)

Da applicare a **tutte** le campagne. Esclude DIY, informazionali, competitor non rilevanti.

**DIY · Informazionale (40+):**
fai da te · fai-da-te · tutorial · istruzioni · istruzione · video · modulo · moduli · pdf · gratis · gratuito · gratuita · come fare · come funziona · come installare · come pulire · come stappare · come sturare · come sbloccare · come riparare · come liberare · come spurgare · come montare · come cambiare · rimedi · rimedi naturali · soda caustica · bicarbonato · amazon · ebay · leroy merlin · brico · bricoman · recensioni · opinioni · altroconsumo · forum · wikipedia · youtube · significato

**Lavoro · Formazione (10+):**
lavoro · stipendio · corso · corsi · diploma · attestato · patentino · assunzione · offerte di lavoro · cv · curriculum

**Documenti · Certificazioni (8):**
certificazione · dichiarazione conformità · modulo dichiarazione · allegato · normativa · legge · decreto

**Brand competitor (assistenza locale, 30+):**
[lista brand assistenza locale generica del settore]

### Lista B · BRAND CLIENTE A (specifica servizi)

**Geo fuori area (12):**
[provincia 1] · [provincia 2] · [provincia 3] · [provincia 4] · [provincia 5] · [provincia 6] · [provincia 7] · [provincia 8] · [provincia 9] · [provincia 10] · [provincia 11] · [provincia 12]

**Servizi non offerti (8):**
[servizio non offerto 1] · [servizio non offerto 2] · [servizio non offerto 3] · [servizio non offerto 4] · [servizio non offerto 5] · [servizio non offerto 6] · [servizio non offerto 7] · [servizio non offerto 8]

**Errori · Reset (riparazione, non sostituzione, 25+):**
errore e01 · errore e02 · ... · errore 60 · errore 73 · ot errore · codice errore · tasto reset · spia rossa · valvola pressione · non parte · lampeggia · reset 01 · non si accende · numero verde · servizio clienti · assistenza clienti · contatti

**Bonus · Incentivi (fase informativa, 12):**
bonus · incentivo · incentivi · detrazione · detrazioni · agevolazione · agevolazioni · conto termico · sconto in fattura · 730 · agenzia entrate

**Modelli prodotto specifici (40+):**
[modello 1] · [modello 2] · [modello 3] · ... · [modello 40+]

### Lista C · BRAND CLIENTE B (specifica e-com prodotto)

**Brand competitor depuratori (40+):**
[competitor 1] · [competitor 2] · [competitor 3] · ... · [competitor 40+]

**DIY + Informazionali specifici (10):**
fai da te · kit [prodotto] · [prodotto] casa fai da te · come funziona · pro e contro · opinioni mediche · cosa elimina · differenza tra · microfiltrazione

**Aggregatori + Geo fuori area (10):**
amazon · leroy merlin · gold box · gratis · recensioni · recensioni negative · forum · altroconsumo · [città fuori area 1] · [città fuori area 2] · [città fuori area 3] · [città fuori area 4]

### Mappa applicazione

| Campagna | Lista A | Lista B | Lista C |
|---|---|---|---|
| CA_Search_LineaServizio1 | ✓ | ✓ | — |
| CA_Search_LineaServizio2 | ✓ | ✓ | — |
| CA_PMax_LineaServizio2 | ✓ | ✓ (escl. brand top) | — |
| CB_Search_Prodotto | ✓ | — | ✓ |
| CB_PMax_Prodotto | ✓ | — | ✓ |

---

## 05 · Keyword set finali per campagna

> Convenzione: `"phrase"` = PHRASE · `[esatta]` = EXACT

### Campagna 1 · CA_Search_LineaServizio1
**€15/g · Search · Geo: Capoluogo + 25 km · Bid: Maximize Conversions · 24/7**

**Ad Group A · Pronto Intervento (urgenza)**
```
"[servizio] [capoluogo]"           [[servizio] [capoluogo]]
"pronto intervento [servizio]"     [pronto intervento [servizio]]
"[servizio] urgente [capoluogo]"   [[servizio] urgente [capoluogo]]
"[servizio] h24 [capoluogo]"
"[servizio] 24 ore [capoluogo]"
"sos [servizio] [capoluogo]"
"[servizio] notturno [capoluogo]"
"[servizio] domenica [capoluogo]"
"[servizio] festivo [capoluogo]"
"[servizio] subito [capoluogo]"
"chiamare [servizio] [capoluogo]"
```

**Ad Group B · Frazioni & Comuni limitrofi**
```
"[servizio] [zona 1]"
"[servizio] [zona 2]"
"[servizio] [zona 3]"
... (12 zone totali)
```

**Ad Group C · Riparazioni specifiche**
```
"[riparazione 1] [capoluogo]"
"[riparazione 2] [capoluogo]"
"[riparazione 3] [capoluogo]"
... (10 riparazioni)
```

### Campagna 2 · CA_Search_LineaServizio2
**€15/g · Search · Geo: Capoluogo + 30 km · Bid: Maximize Conversions · Lun-Sab 7-22**

**Ad Group A · Sostituzione/Cambio**
```
"sostituzione [prodotto] [capoluogo]"   [sostituzione [prodotto] [capoluogo]]
"cambio [prodotto] [capoluogo]"         [cambio [prodotto] [capoluogo]]
"sostituire [prodotto] [capoluogo]"
"nuova [prodotto] [capoluogo]"
"installazione [prodotto] [capoluogo]"  [installazione [prodotto] [capoluogo]]
"preventivo sostituzione [prodotto]"
"preventivo [prodotto] [capoluogo]"
```

**Ad Group B · Tecnologia core**
```
"[prodotto] [tipologia core] [capoluogo]"
"[prodotto] [tipologia core] installazione"
"installazione [prodotto] [tipologia core] [capoluogo]"
"[prodotto] [tipologia core] prezzo installazione"
```

**Ad Group C · Brand top installati (4 brand max)**
```
"installazione [prodotto] [brand top 1] [capoluogo]"
"installazione [prodotto] [brand top 2] [capoluogo]"
"installazione [prodotto] [brand top 3] [capoluogo]"
"installazione [prodotto] [brand top 4] [capoluogo]"
```

### Campagna 3 · CA_PMax_LineaServizio2
**€25/g · PMax · Geo: Capoluogo + 30 km · Bid: Max Conv (→ tCPA €45 dopo 30 conv) · Final URL expansion ON**

**Asset Group unico:** "[Prodotto] [tipologia] [Capoluogo]"

**Search themes (5):**
1. sostituzione [prodotto] [tipologia]
2. installazione [prodotto] [capoluogo]
3. preventivo [prodotto]
4. cambio [prodotto] [tipologia]
5. [prodotto] [brand top] [capoluogo]

**Audience signals:**
- Custom segment: cerche "sostituzione [prodotto]" / "[prodotto] [tipologia]" ultimi 30g
- In-market: Home & Garden > Home Improvement > [categoria specifica]
- Demografica: 35-65 anni, proprietari casa
- Geo intent: [Capoluogo] metropolitana

### Campagna 4 · CB_Search_Prodotto
**€10/g · Search · Geo: Capoluogo + 50 km · Bid: Maximize Conversions**

**Ad Group A · Prodotto core**
```
"[prodotto] casa"                  [[prodotto] casa]
"[prodotto] [capoluogo]"           [[prodotto] [capoluogo]]
"installazione [prodotto] casa"
"[prodotto] sotto[area]"
"[prodotto] casa prezzo"
"miglior [prodotto] casa"
```

**Ad Group B · [Tecnologia specifica]**
```
"[tecnologia] casa"                [[tecnologia]]
"[tecnologia] [capoluogo]"
"[prodotto] [tecnologia]"
"impianto [tecnologia] casa"       [impianto [tecnologia] casa]
"[prodotto] [tecnologia]"
"installazione [tecnologia]"
```

**Ad Group C · Brand**
```
[brand cliente B]
"[brand cliente B]"
"[brand cliente B] [capoluogo]"
"[brand cliente B] [prodotto]"
"[brand cliente B] recensioni"
```

**Ad Group D · Problemi locali**
```
"[problema 1] [capoluogo]"
"[problema 2] [capoluogo]"
"[problema 3] casa"
"trattamento [problema] casa [capoluogo]"
```

### Campagna 5 · CB_PMax_Prodotto
**€15/g · PMax · Geo: Regione · Bid: Max Conv · Final URL expansion ON**

**Asset Group unico:** "[Prodotto] [Tipologia] Casa"

**Search themes (5):**
1. [prodotto] casa
2. [tecnologia] domestica
3. installazione [prodotto] [capoluogo]
4. [prodotto] [posizionamento]
5. trattamento [problema] casa

**Audience signals:**
- Custom segment: cerche "[prodotto]", "[tecnologia] casa"
- In-market: Home & Garden > Home Appliances > [categoria]
- Affinity: Health & Wellness Enthusiasts
- Demografica: 30-65, proprietari casa
- Lookalike: clienti acquistati ultimi 12 mesi

### Fase 2 · DemGen (gate dopo 30 giorni)

**ESPANSIONE CONDIZIONATA:** Le campagne DemGen verranno valutate dopo 30 giorni di delivery delle PMax. Pre-set di lookalike e custom intent già preparati ma non lanciati. Budget aggiuntivo previsto: €20/giorno (€10 per brand).

---

## 06 · Copy annunci

**Convenzione validazione:** Headline ≤ 30 caratteri · Descriptions ≤ 90 caratteri · Long headline PMax ≤ 90 caratteri · validati carattere per carattere.

### Esempio · CA_Search_LineaServizio1 · Ad Group A · Pronto Intervento

**RSA #1 · Headlines (15)**
1. [Servizio] [Capoluogo] 24h
2. Pronto Intervento Subito
3. [Servizio] Urgente Oggi
4. Chiamaci Ora · [Capoluogo]
5. Risolviamo in 30 Minuti
6. [Servizio] H24 [Capoluogo]
7. Tecnico in Sede Oggi
8. SOS [Servizio] [Capoluogo]
9. Preventivo Gratuito
10. 20+ Anni di Esperienza
11. Notturno · Festivo · Subito
12. Centro · Provincia [BO]
13. Garanzia Lavoro Scritta
14. [Brand Cliente A] [Capoluogo]
15. Chiama Ora · Risolviamo

**Descriptions (4)**
1. [Servizio] professionista a [Capoluogo]. Pronto intervento 24/7, preventivo chiaro, garanzia.
2. [Riparazione 1], [riparazione 2], [riparazione 3]. Risolviamo subito a [Capoluogo] e provincia. Chiama ora.
3. Tecnici qualificati in 30 minuti. Senza chiamata fuori porta nascosta. Trasparenza totale.
4. [Brand Cliente A]: pronto intervento [Capoluogo] H24. 20+ anni nel settore. Preventivo gratis.

Path: `/[servizio]-[capoluogo]` · `/pronto-intervento`

### Esempio · CA_Search_LineaServizio1 · Ad Group B · Frazioni

**RSA #1 · Headlines (15)**
1. [Servizio] in Provincia [BO]
2. [Zona 1] · [Zona 2]
3. [Zona 3] · [Zona 4]
4. Tecnico nella Tua Zona
5. Intervento Rapido Frazioni
6. [Zona 5] · [Zona 6]
7. [Servizio] Vicino a Te
8. [Brand Cliente A] [Capoluogo]
9. Preventivo Gratuito
10. Garanzia Lavoro Scritta
11. Chiama Subito · [Capoluogo]
12. Tecnici Qualificati
13. 20+ Anni Esperienza
14. Senza Costi Nascosti
15. Risolviamo in Giornata

**Descriptions (4)**
1. Servizio [servizio] in tutta la provincia di [Capoluogo]. Tecnici nella tua zona, intervento rapido.
2. [Zona 1], [Zona 2], [Zona 3], [Zona 4]: [servizio] [Brand Cliente A] a un solo colpo di telefono.
3. Riparazioni, sostituzioni, manutenzioni. Preventivo trasparente prima del lavoro.
4. 20+ anni di esperienza nel territorio. Chiama oggi, risolviamo oggi.

### Esempio · CA_Search_LineaServizio1 · Ad Group C · Riparazioni

**RSA #1 · Headlines (15)**
1. [Riparazione 1] [BO]
2. [Riparazione 2]
3. [Riparazione 3]? Risolviamo
4. [Riparazione 4] · [Capoluogo]
5. [Riparazione 5]
6. [Servizio] Subito [Capoluogo]
7. Pronto Intervento 24h
8. Preventivo Gratuito
9. 20+ Anni Esperienza
10. Tecnico Sul Posto Oggi
11. [Brand Cliente A] [Capoluogo]
12. Garanzia Lavoro Scritta
13. Chiama Ora · [Capoluogo]
14. Riparazioni [Servizio]
15. Senza Costi Nascosti

**Descriptions (4)**
1. [Riparazione 1], [riparazione 2], [riparazione 3]? [Brand Cliente A] risolve subito.
2. [Riparazione 1] a [Capoluogo]: tecnico sul posto entro 60 minuti. Preventivo chiaro.
3. [Riparazione varie]. Lavoro garantito per iscritto.
4. [Brand Cliente A] [Capoluogo] · 20+ anni di riparazioni [servizio]. Chiama, ti aiutiamo.

### Pattern replicato per le altre 4 campagne

> Per ognuna delle 4 campagne residue (CA_Search_LineaServizio2, CA_PMax, CB_Search, CB_PMax) il report originale contiene:
> - 1+ RSA con 15 headlines + 4 descriptions per ogni Ad Group
> - Per le PMax: lista headlines/long headlines/descriptions/CTA + brief asset visuali
> - Tutto validato carattere per carattere su limiti Google

---

## 📌 Note operative finali

- **Modello costo Fixup:** ore consulenza + setup + presidio settimanale 30 min
- **Tempistiche tipiche:** report consegnato in 7-10 giorni lavorativi · go-live campagne in 2-3 giorni post-approvazione
- **Cosa serve dal cliente:** accessi Google Ads + brief brand voice + validazione legale copy
- **Cosa NON è incluso in questa fase:** SEO, content production sito, gestione social organico, email marketing automation (sono pacchetti separati)

---

*Documento esempio anonimizzato · Versione FIXUP showcase aprile 2026*
*Per il deliverable reale completo (28 pagine PDF brandizzato): contattare https://cal.com/max-pavesio/call-30-minuti*
