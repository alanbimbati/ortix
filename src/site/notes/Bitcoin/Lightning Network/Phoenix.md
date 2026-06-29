---
{"dg-publish":true,"permalink":"/bitcoin/lightning-network/phoenix/","title":"🕊️ Phoenix: la self-custody semplificata","tags":["Bitcoin","Lightning","Wallet","SelfCustodial"],"dg-note-properties":{"title":"🕊️ Phoenix: la self-custody semplificata","tags":["Bitcoin","Lightning","Wallet","SelfCustodial"],"aliases":["Phoenix Wallet","Phoenix"]}}
---


# 🕊️ Phoenix: la self-custody semplificata

🕊️ **Livello 2: il primo passo nella sovranità reale.**  
Phoenix Wallet, sviluppato da **ACINQ**, rappresenta un eccellente compromesso per l'utente che vuole possedere le proprie chiavi private delegando al software la gestione tecnica dei canali.

---

## 🏗️ La Struttura dei Canali

A differenza dei wallet tradizionali, Phoenix ti fornisce una [[Bitcoin/Definizioni/Blockchain/🧠 Seed Phrase\|Seed Phrase]] di 12 parole: questo significa che **sei il reale proprietario dei fondi on-chain** e nessuno può censurare o congelare i tuoi satoshi.

Tuttavia, per nascondere la complessità tecnica di Lightning Network al grande pubblico:
* Phoenix stabilisce e gestisce **un unico [[Bitcoin/Definizioni/Lightning/Canale di Pagamento\|Canale di Pagamento]] automatico** diretto verso i nodi centrali di ACINQ.
* Non devi scegliere i tuoi peer, bilanciare i canali o preoccuparti dello stato dei canali: l'applicazione fa tutto in automatico.

---

## 💸 Il Compromesso dei Costi (Fee dello 0,4%)

Questa estrema comodità non è gratuita e incide significativamente sull'uso quotidiano:
* **Fee fissa dello 0.4%**: Ogni volta che invii o ricevi pagamenti tramite Lightning, paghi una commissione fissa dello 0.4% sul valore scambiato, in aggiunta alle normali commissioni di [[Bitcoin/Definizioni/Lightning/Routing\|Routing]] della rete (routing fee).
* **Costo di apertura canali**: L'apertura automatica del canale iniziale (e di quelli successivi necessari a espandere la capacità) richiede il pagamento di una commissione on-chain specchio dei reali costi di mining, riducendo l'efficienza per transazioni molto piccole.

---

## 🖼️ Mappa Automatica di ACINQ

![Ortix_Phoenix.png\|300](/img/user/Immagini/Ortix_Phoenix.png)  
*Figura 2: Gestione a canale singolo automatizzato di ACINQ (con Ortix).*

---

## ⚖️ Le Tre Domande di Ortix

1. **Chi decide?** ACINQ decide le dinamiche di instradamento del tuo canale e modula le fee di apertura. Tu decidi di possedere i tuoi fondi tramite seed.
2. **Quali incentivi ha?** ACINQ ha l'incentivo a trarre profitto dalle commissioni dello 0.4% e a massimizzare l'uptime del proprio nodo per garantire pagamenti fluidi.
3. **Chi è responsabile?** Tu sei responsabile del backup delle tue 12 parole. ACINQ è responsabile di mantenere attive le rotte del canale sul loro server.

---

🔗 _Vedi anche: [[Bitcoin/Lightning Network/00 - Come Essere Sovrano su LN (Step-by-Step)\|00 - Come Essere Sovrano su LN (Step-by-Step)]], [[Bitcoin/Definizioni/Blockchain/🔐 Self-custody\|🔐 Self-custody]], [[Bitcoin/Lightning Network/Wallet of Satoshi\|Wallet of Satoshi]], [[Bitcoin/Lightning Network/Blixt\|Blixt]]_
