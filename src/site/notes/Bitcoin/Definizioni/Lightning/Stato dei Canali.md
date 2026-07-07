---
{"dg-publish":true,"permalink":"/bitcoin/definizioni/lightning/stato-dei-canali/","title":"💾 Stato dei Canali: la veridicità contabile","tags":["Bitcoin","Lightning","Definizione","Backup"],"dg-note-properties":{"title":"💾 Stato dei Canali: la veridicità contabile","tags":["Bitcoin","Lightning","Definizione","Backup"],"aliases":["Stato dei canali","channel state","backup dei canali","static channel backup","SCB"]}}
---


# 💾 Stato dei Canali: la veridicità contabile

⚡ In [[Bitcoin/Lightning Network/⚡ Lightning Network\|Lightning Network]], lo **Stato dei Canali** (Channel State) è il registro crittografico costantemente aggiornato che specifica quanti satoshi appartengono a ciascuna delle parti all'interno di un [[Bitcoin/Definizioni/Lightning/Canale di Pagamento\|Canale di Pagamento]].

A differenza delle normali transazioni Bitcoin on-chain, dove basta la [[Bitcoin/Definizioni/Blockchain/🧠 Seed Phrase\|Seed Phrase]] per recuperare l'intero saldo, su Lightning **la sola seed phrase non basta a recuperare la liquidità bloccata nei canali attivi.** Serve l'ultimo stato registrato.

---

## ⚠️ Il rischio di recupero e la frode

Poiché le transazioni si muovono fuori dalla blockchain principale, se perdi il telefono o l'app si distrugge, il tuo wallet ha bisogno di sapere qual era l'ultimo stato concordato con i vari nodi per poter chiudere i canali on-chain e recuperare i fondi.

* **Se usi uno stato vecchio**: Se provi a pubblicare on-chain uno stato del canale non aggiornato (magari una versione in cui avevi più bitcoin rispetto a quelli attuali), la controparte può pubblicare una transazione di penalizzazione (Justice Transaction) e **sequestrarti l'intero saldo del canale**. Questo previene le frodi nel protocollo, ma punisce gli errori accidentali di ripristino.

---

## 🎯 Il Framework di Responsabilità

1. **Chi decide?** Il software del wallet gestisce lo stato ad ogni singolo pagamento inviato o ricevuto, scrivendo un nuovo record crittografato.
2. **Quali incentivi ha?** L'utente ha l'incentivo cruciale di avere sempre un backup aggiornato all'ultimo millisecondo per evitare la perdita di fondi in caso di guasto hardware.
3. **Chi è responsabile?** Nei wallet custodial (Livello 1), la responsabilità è delegata al provider. Nei wallet non-custodial:
   * [[Bitcoin/Lightning Network/Phoenix\|Phoenix]] (Livello 2) usa una gestione automatizzata sui server di ACINQ.
   * [[Bitcoin/Lightning Network/Blixt\|Blixt]] (Livello 3) costringe l'utente a configurare un backup dello stato dei canali (Static Channel Backup - SCB). Questo backup può essere salvato in modo sicuro su servizi cloud come Google Drive.

---

## 🛡️ Il Backup su Google Drive è sicuro?

Sì. Una delle domande più frequenti è se salvare lo Stato dei Canali su cloud esterni metta a rischio i propri fondi.
> [!NOTE]
> Il backup dello stato dei canali **non contiene le tue chiavi private**. Si tratta solo di una mappa contabile cifrata che dice dove si trovano i tuoi canali e qual è il saldo. Senza la tua [[Bitcoin/Definizioni/Blockchain/🧠 Seed Phrase\|Seed Phrase]], nessuno può rubare un singolo satoshi da quel file di backup. Serve unicamente a ripristinare la comunicazione e forzare la chiusura unilaterale dei canali per rimetterti i bitcoin on-chain.

---

🔗 _Vedi anche: [[Bitcoin/Lightning Network/00 - Come Essere Sovrano su LN (Step-by-Step)\|00 - Come Essere Sovrano su LN (Step-by-Step)]], [[Bitcoin/Definizioni/Lightning/Canale di Pagamento\|Canale di Pagamento]], [[Bitcoin/Definizioni/Blockchain/🧠 Seed Phrase\|🧠 Seed Phrase]], [[Bitcoin/Lightning Network/Blixt\|Blixt]], [[Bitcoin/Lightning Network/Phoenix\|Phoenix]], [[Bitcoin/Lightning Network/Zeus\|Zeus]]_
