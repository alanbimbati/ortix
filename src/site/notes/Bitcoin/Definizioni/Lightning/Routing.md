---
{"dg-publish":true,"permalink":"/bitcoin/definizioni/lightning/routing/","title":"📡 Routing: instradare il valore","tags":["Bitcoin","Lightning","Definizione","Routing"],"dg-note-properties":{"title":"📡 Routing: instradare il valore","tags":["Bitcoin","Lightning","Definizione","Routing"],"aliases":["Routing","instradamento","routing fee"]}}
---


# 📡 Routing: instradare il valore

⚡ Il **Routing** (instradamento) è il processo mediante il quale una transazione su [[Bitcoin/Lightning Network/⚡ Lightning Network\|Lightning Network]] viaggia da un trasmettitore a un ricevitore passando attraverso una catena di [[Bitcoin/Definizioni/Lightning/Canale di Pagamento\|Canali di Pagamento]] intermediati da nodi terzi.

Consente di inviare fondi a chiunque sulla rete, anche se non si ha un canale direttamente aperto con quella specifica persona.

---

## 🏗️ Come Funziona

Se Alice vuole inviare 1000 sats a Carlo, ma ha un canale aperto solo con Bob, e Bob ha un canale aperto con Carlo:
1. Alice invia i fondi a Bob.
2. Bob inoltra i fondi a Carlo.
3. Ciascun nodo intermediario (Bob, in questo caso) trattiene una piccolissima *routing fee* (es. 1 o 2 sats) per il servizio prestato e per il costo dell'immobilizzazione dei propri fondi.

Il routing utilizza la **crittografia onion** (simile a [[Ortix/Navigazione/Web/Tor\|Tor]]): i nodi intermedi conoscono solo il peer precedente e il peer successivo, ma non conoscono l'origine finale né il destinatario finale del pagamento, garantendo un'elevata privacy.

---

## 🎯 Il Framework di Responsabilità

1. **Chi decide?** Gli algoritmi del wallet o del nodo decidono il percorso ottimale per il pagamento, cercando il bilanciamento ideale tra commissioni basse ed elevata probabilità di successo.
2. **Quali incentivi ha?** Chi possiede un [[Bitcoin/Definizioni/Blockchain/Full Node\|Full Node]] sempre attivo (Livello 4, come [[Bitcoin/Lightning Network/Zeus\|Zeus]] + Nodo) ha l'incentivo economico di lasciare canali liquidi aperti ed equilibrati per guadagnare satoshi passivamente instradando le transazioni degli altri.
3. **Chi è responsabile?** Gli operatori dei nodi sono responsabili della liquidità e delle fee impostate sui propri canali. Su smartphone, fare routing è inefficace perché il telefono non è online 24 ore su 24 e le variazioni di IP declassano il nodo sul grafico del network.

---

## 📊 Esempio Empirico (Blixt vs Phoenix)

L'instradamento non costa uguale dappertutto. Durante i test reali:
* Una transazione da [[Bitcoin/Lightning Network/Blixt\|Blixt]] a [[Bitcoin/Lightning Network/Phoenix\|Phoenix]] è costata solo **21 sats** di routing fee.
* Il percorso inverso, da [[Bitcoin/Lightning Network/Phoenix\|Phoenix]] a [[Bitcoin/Lightning Network/Blixt\|Blixt]], è costato ben **71 sats** (il triplo!), poiché Phoenix instrada forzatamente tramite il nodo di ACINQ applicando tariffe extra.
