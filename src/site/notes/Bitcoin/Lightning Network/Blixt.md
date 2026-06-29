---
{"dg-publish":true,"permalink":"/bitcoin/lightning-network/blixt/","title":"⚡ Blixt: lo snodo multi-canale mobile","tags":["Bitcoin","Lightning","Wallet","NonCustodial","MultiChannel"],"dg-note-properties":{"title":"⚡ Blixt: lo snodo multi-canale mobile","tags":["Bitcoin","Lightning","Wallet","NonCustodial","MultiChannel"],"aliases":["Blixt","Blixt Wallet"]}}
---


# ⚡ Blixt: lo snodo multi-canale mobile

⚡ **Livello 3: la vera svolta sovrana su smartphone.**  
Blixt Wallet rappresenta un punto di rottura tecnologico. Non è un semplice wallet che delega la gestione del network a un server centrale: Blixt fa girare un vero e proprio micro-nodo Lightning (basato su [[Bitcoin/Definizioni/Lightning/LND\|LND]]/Neutrino) direttamente all'interno del tuo telefono.

---

## 🔌 La Gestione Autonoma dei Canali

A differenza di [[Bitcoin/Lightning Network/Phoenix\|Phoenix]], che ti incatena a un singolo canale verso ACINQ, con Blixt sei **completamente libero di aprire canali in totale autonomia** verso qualsiasi nodo che preferisci (es. nodi di grandi esercenti, nodi di amici o nodi di routing strategici).

* Molti nodi del network (compreso il nodo ufficiale di Blixt) non richiedono commissioni di apertura canale e sono perfettamente interconnessi con i nodi principali (come [[Bitcoin/Lightning Network/Wallet of Satoshi\|Wallet of Satoshi]] e [[Bitcoin/Lightning Network/Phoenix\|Phoenix]]).
* Potendo gestire **più canali contemporaneamente (multi-canale)**, se usi spesso Lightning puoi direzionare i pagamenti sulle rotte più economiche e resilienti, assicurando che le transazioni arrivino a destinazione in ogni condizione.

---

## 📥 La Gestione della Liquidità in Entrata (Inbound Liquidity)

Una delle grandi barriere all'ingresso di Lightning Network è la capacità di ricevere pagamenti se non si è ancora speso del denaro. Blixt risolve brillantemente questo problema con l'automazione della [[Bitcoin/Definizioni/Lightning/Liquidità in Entrata\|Liquidità in Entrata]]:

Se qualcuno tenta di inviarti dei satoshi ma il tuo lato del canale non ha spazio sufficiente a ricevere, Blixt richiede in automatico l'apertura di un canale di supporto verso di te (pagando una piccola fee on-chain). Questa operazione necessita del tempo di conferma di un blocco Bitcoin (circa 10 minuti di attesa tecnica on-chain), ma consente di ricevere fondi in auto-custodia senza alcuna configurazione manuale o preventiva.

---

## 📊 I Dati Empirici delle Fee (Test reali sul campo)

L'efficienza di questa gestione multi-canale autonoma si riflette direttamente nei dati reali registrati durante le mie prove empiriche:

* **Da Blixt a Phoenix**: Una transazione di ~18.000 sats è costata solo **21 sats** di routing fee.
* **Percorso inverso (da Phoenix a Blixt)**: Per la stessa transazione abbiamo pagato ben **71 sats** (il triplo!), a causa dell'intermediazione obbligata del nodo ACINQ.
* **Da Blixt a Wallet of Satoshi**: Una transazione di 1000 sats è costata appena **3 sats** di fee (costi praticamente azzerati).

Una piccola nota: le fee sono in percentuale all'importo speso

---

## 💾 Sicurezza e Backup

> [!IMPORTANT]
> **Il recupero su Blixt richiede due elementi:**
> 1. La tua **[[Bitcoin/Definizioni/Blockchain/🧠 Seed Phrase\|Seed Phrase]]** (le 24 parole del wallet: segretissima e da scrivere su carta o metallo).
> 2. Lo **[[Bitcoin/Definizioni/Lightning/Stato dei Canali\|Stato dei Canali]]** cifrato (Static Channel Backup - SCB).
> 
> Blixt ti consente di automatizzare il salvataggio dello stato dei canali sul tuo Google Drive. Questo processo è del tutto sicuro: il file di backup **non contiene chiavi private e non espone i tuoi bitcoin al furto**. Serve esclusivamente come mappa contabile per recuperare le coordinate dei canali attivi se il telefono si rompe.

---

## 📡 Rilevazione sul Routing da Mobile

Gettando un micro-nodo sempre in tasca si potrebbe essere tentati di guadagnare satoshi facendo [[Bitcoin/Definizioni/Lightning/Routing\|Routing]] passivo per le transazioni altrui. In pratica, però, **questo su smartphone non funziona**:
* Il telefono non è costantemente online 24 ore su 24.
* I continui cambi di connessione (da Wi-Fi a rete dati cellulare 4G/5G) cambiano l'indirizzo IP del nodo.
* Questa instabilità mina la reputazione del nodo sulla rete globale di routing, escludendolo dai percorsi preferenziali.

---

## 🖼️ Ottimizzazione Strutturale

![Ortix_Blixt.png\|300](/img/user/Immagini/Ortix_Blixt.png)  
*Figura 3: Ottimizzazione multi-canale e monitoraggio delle fee minime (con Ortix).*

---

## ⚖️ Le Tre Domande di Ortix

1. **Chi decide?** Decidi tu. Scegli a quali peer connetterti, che canali aprire e quanta liquidità allocare alle varie rotte.
2. **Quali incentivi ha?** Blixt ha l'incentivo a supportare il protocollo [[Bitcoin/Definizioni/Lightning/LND\|LND]] ed eliminare i intermediari aziendali per favorire la vera decentralizzazione.
3. **Chi è responsabile?** Sei tu il solo responsabile dei tuoi fondi e del mantenimento aggiornato del backup dello stato dei canali.

---

🔗 _Vedi anche: [[Bitcoin/Lightning Network/00 - Come Essere Sovrano su LN (Step-by-Step)\|00 - Come Essere Sovrano su LN (Step-by-Step)]], [[Bitcoin/Definizioni/Lightning/Liquidità in Entrata\|Liquidità in Entrata]], [[Bitcoin/Definizioni/Lightning/Stato dei Canali\|Stato dei Canali]], [[Bitcoin/Definizioni/Lightning/Routing\|Routing]], [[Bitcoin/Lightning Network/Zeus\|Zeus]]_
