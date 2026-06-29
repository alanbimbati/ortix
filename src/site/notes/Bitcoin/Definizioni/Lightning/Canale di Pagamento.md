---
{"dg-publish":true,"permalink":"/bitcoin/definizioni/lightning/canale-di-pagamento/","title":"🔌 Canale di Pagamento: il tubo del valore","tags":["Bitcoin","Lightning","Definizione","Canali"],"dg-note-properties":{"title":"🔌 Canale di Pagamento: il tubo del valore","tags":["Bitcoin","Lightning","Definizione","Canali"],"aliases":["Canale di pagamento","canale Lightning","payment channel","canali"]}}
---


# 🔌 Canale di Pagamento: il tubo del valore

⚡ Un **Canale di Pagamento** (Payment Channel) è la struttura fondamentale di [[Bitcoin/Lightning Network/⚡ Lightning Network\|Lightning Network]]. Può essere immaginato come un "tubo bidirezionale" aperto tra due nodi (peer) sulla rete, all'interno del quale scorrono satoshi senza bisogno di registrare ogni singola transazione sulla blockchain principale di Bitcoin.

---

## 🏗️ Come Funziona (In parole povere)

1. **Apertura**: Due parti decidono di aprire un canale effettuando una transazione on-chain speciale (un indirizzo [[Bitcoin/Definizioni/Blockchain/🔐 Multisig\|Multisig 2-di-2]]). Questa operazione deposita dei bitcoin nel canale (chiamati *capacità del canale*) e richiede il pagamento di una commissione di mining on-chain.
2. **Scambio**: Una volta aperto, le parti possono scambiarsi transazioni Lightning aggiornando il bilancio del canale istantaneamente. È come un abaco: sposti i gettoni da sinistra a destra e viceversa. Queste transazioni sono immediate e costano frazioni di centesimo.
3. **Chiusura**: Quando si decide di chiudere il canale, lo stato finale del bilancio viene registrato sulla blockchain di Bitcoin con un'ultima transazione on-chain. Ciascun partecipante riceve la quota che gli spetta.

---

## 🎯 Il Framework di Responsabilità

1. **Chi decide?** I due nodi che stabiliscono il canale decidono quanta capacità allocare e verso quali nodi aprirlo.
2. **Quali incentivi ha?** Gli incentivi sono economici e di efficienza. Aprire canali verso nodi molto interconnessi riduce i fallimenti dei pagamenti e consente di guadagnare micro-commissioni inoltrando i pagamenti altrui ([[Bitcoin/Definizioni/Lightning/Routing\|Routing]]).
3. **Chi è responsabile?** Ciascun partecipante è responsabile del mantenimento del proprio nodo online e della sicurezza del backup aggiornato dello [[Bitcoin/Definizioni/Lightning/Stato dei Canali\|Stato dei Canali]].

---

## 🧭 Canale Singolo vs Multi-Canale

* **Canale Singolo (es. [[Bitcoin/Lightning Network/Phoenix\|Phoenix]])**: Il wallet si connette a un solo nodo centrale (ACINQ). È molto facile da usare perché la complessità è delegata, ma sei dipendente dalle condizioni economiche e dall'uptime di quel singolo operatore.
* **Multi-Canale (es. [[Bitcoin/Lightning Network/Blixt\|Blixt]] o [[Bitcoin/Lightning Network/Zeus\|Zeus]])**: Gestisci autonomamente canali con nodi diversi del network. Questo offre maggiore stabilità (ridondanza se un nodo va offline), commissioni inferiori e privacy più elevata.
