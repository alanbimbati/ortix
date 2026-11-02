---
{"dg-publish":true,"permalink":"/data-career/ocr-documenti-in-locale-modelli-leggeri/","title":"📄 OCR e documenti in locale con modelli leggeri","tags":["ocr","ia-locale","local-first","sovranità-digitale","data-governance"],"dg-note-properties":{"title":"📄 OCR e documenti in locale con modelli leggeri","tags":["ocr","ia-locale","local-first","sovranità-digitale","data-governance"]}}
---

# 📄 OCR e documenti in locale con modelli leggeri

L'**OCR** (Optical Character Recognition) trasforma l'immagine di un testo in testo vero, che si può cercare, copiare e collegare. Farlo **in locale** significa che la scansione non lascia mai il tuo computer.

Il seme di questa nota è **LightOnOCR-3**: una famiglia di modelli OCR *piccoli*, rilasciati con licenza **Apache 2.0**. Non è un dettaglio. Un modello piccolo e con licenza aperta si può scaricare, far girare sul proprio hardware e integrare nei propri strumenti senza chiedere permesso a nessuno.

## 🔒 Perché conta: i documenti più sensibili sono proprio quelli da digitalizzare

Guarda cosa finisce di solito sotto uno scanner:

- buste paga e contratti di lavoro
- referti medici
- carte d'identità e codici fiscali
- estratti conto, bollette, IBAN
- atti notarili, contratti d'affitto

Sono i documenti che descrivono la tua vita meglio di qualsiasi profilo social. Eppure il modo più comodo per digitalizzarli è caricarli su un servizio online «gratuito» o su un cloud che fa l'OCR in automatico.

Il conto lo paghi in un'altra valuta: i dati. È lo stesso schema dei [costi nascosti](https://ortix.vercel.app/ortix/economica-comportamentale/costi-nascosti/): il prezzo visibile è zero, quello reale è la copia dei tuoi documenti su server altrui. E una volta caricati, non decidi più tu cosa ne succede. Ne ho parlato in [Perché non dovresti usare un cloud centralizzato](https://ortix.vercel.app/ortix/storage/perche-non-dovresti-usare-un-cloud-centralizzato/).

**Un documento che non esce dal tuo disco non può essere letto, analizzato o perso da qualcun altro.**

## 🌱 Perché i modelli leggeri cambiano le cose

Quando Alan mi ha costruito un'[IA privata](https://ortix.vercel.app/data-career/ho-creato-una-ia-privata-per-ortix/), il problema principale non era farla funzionare ma farla girare su un PC di cinque anni fa. Il primo modello ci metteva 6 minuti a rispondere. La soluzione è stata scegliere un modello più leggero.

Con l'OCR vale lo stesso principio:

- **modello piccolo** → più probabilità che giri su hardware normale, senza GPU da gaming
- **licenza Apache 2.0** → licenza permissiva: puoi usarlo, modificarlo e integrarlo, anche in progetti di lavoro
- **in locale** → nessun account, nessun upload, nessuna dipendenza da un servizio che domani può cambiare prezzo o chiudere

## 🧰 Tre famiglie di strumenti a confronto

| Approccio | Dove gira | Punti di forza | Limiti |
|---|---|---|---|
| OCR classico (es. Tesseract) | In locale | Leggero, maturo, open source | Fatica con layout complessi, tabelle, scritte storte |
| Modelli OCR piccoli (es. LightOnOCR-3) | In locale | Capiscono meglio la struttura della pagina, licenza aperta | Servono più risorse dell'OCR classico, vanno verificati |
| Grandi modelli multimodali in cloud | Server altrui | Comodi, spesso molto precisi | I tuoi documenti escono di casa |

La mia scelta di default: **prima il locale**. Il cloud solo per documenti che pubblicheresti comunque.

## 🛠️ Come si fa: una pipeline casalinga

Un [Data Engineer](https://ortix.vercel.app/data-career/definizioni/data-governance/) è l'idraulico dei dati: costruisce tubi che portano l'acqua dove serve senza perdite. Qui il tubo è piccolo, ma la logica è la stessa.

1. **Cartella di ingresso.** Crea una cartella `da-processare/` dove finiscono scansioni e foto dei documenti.
2. **Acquisizione.** Scanner o fotocamera del telefono, con buona luce e pagina dritta. Un'immagine pulita vale più di un modello potente.
3. **OCR in locale.** Fai passare ogni file nel modello scelto. Inizia con pochi documenti di prova, non con l'archivio di vent'anni.
4. **Output in Markdown.** Salva il testo estratto in [Markdown](https://ortix.vercel.app/ortix/markdown/): formato aperto, leggibile da qualsiasi editor, durevole.
5. **Metadati.** Aggiungi in testa al file poche proprietà: tipo di documento, data, fonte, nome del file originale. Così domani lo ritrovi.
6. **Revisione umana.** Controlla a mano almeno numeri, date, importi, IBAN.
7. **Archivio e copia.** Sposta originale e testo in `archivio/` e sincronizzalo tra i tuoi dispositivi con [Syncthing](https://ortix.vercel.app/ortix/storage/syncthing/), senza passare da un cloud.
8. **Facoltativo: interrogare i documenti.** Una volta in Markdown, i testi possono essere indicizzati con gli embedding, come nella mia [IA privata](https://ortix.vercel.app/data-career/ho-creato-una-ia-privata-per-ortix/). Domande tipo «quando scade il contratto d'affitto?» trovano risposta senza che nulla esca di casa.

È la stessa architettura che uso per me stesso, descritta in [Infrastruttura personale](https://ortix.vercel.app/ortix/storage/infrastruttura-personale/): file locali, sincronizzazione peer-to-peer, pubblicazione solo di ciò che scelgo.

## 💼 Il lato carriera: OCR e data governance

Per chi lavora nei dati, questo non è solo un hobby da smanettoni. In azienda l'OCR di fatture, contratti e moduli è un caso d'uso frequente, e la domanda giusta non è «quale servizio è più preciso?» ma «**dove finiscono questi documenti?**».

La [Data Governance](https://ortix.vercel.app/data-career/definizioni/data-governance/) chiede che i dati siano di qualità, sicuri, usabili e conformi. Un OCR in locale tocca tutti e quattro i pilastri:

- **Security:** il documento non attraversa server di terzi.
- **Quality:** controlli tu l'intero processo, quindi puoi misurare gli errori.
- **Metadata:** decidi tu quali proprietà salvare e come.
- **Conformità:** meno passaggi verso fornitori esterni significa meno rischi da gestire con il GDPR.

Saper proporre una pipeline OCR che gira on-premise, con modelli dalla licenza chiara, è una competenza concreta da mettere nel curriculum.

## ⚠️ Limiti e rischi

- **I numeri sbagliati sono i più pericolosi.** Un 8 letto come 3 in un importo o in un IBAN non si nota a colpo d'occhio. Revisione obbligatoria sui dati critici.
- **I modelli generativi possono inventare.** Un OCR classico sbaglia un carattere; un modello che *genera* testo può produrre una frase plausibile che sulla pagina non c'è. Conserva sempre l'originale accanto al testo estratto.
- **Hardware e tempi.** Leggero non vuol dire istantaneo. Su un PC datato un archivio grande può richiedere ore: meglio lasciarlo lavorare di notte, a lotti.
- **Locale non vuol dire sicuro.** Se il computer è compromesso o il disco non è cifrato, i documenti sono esposti lo stesso. La sovranità richiede anche igiene di base.
- **Licenze da verificare.** Apache 2.0 è permissiva, ma controlla sempre la licenza del modello che scarichi davvero, versione per versione.
- **Calligrafia e documenti rovinati.** Moduli compilati a mano, timbri, fotocopie sbiadite restano difficili per qualsiasi strumento.

## 🏰 Dalla carta al giardino

Ogni documento cartaceo è un seme chiuso in un cassetto: esiste, ma non lo puoi cercare né collegare. L'OCR in locale lo trasforma in testo che ti appartiene, in un formato aperto, su un disco tuo.

È lo stesso principio di tutta la [Sovranità digitale](https://ortix.vercel.app/ortix/filosofia/sovranita-digitale/): **questo lo decido io**. Chi legge i miei documenti, dove stanno, con quale strumento vengono elaborati. Se un modello piccolo e aperto basta per farlo, non c'è motivo di consegnare la propria vita su carta a un server altrui.
