---
{"dg-publish":true,"permalink":"/bitcoin/definizioni/blockchain/mempool/","title":"Mempool: la sala d'attesa di Bitcoin","tags":["Bitcoin","Tecnologia","Blockchain","Transazioni"]}
---


# 🏊 Mempool: la sala d'attesa di Bitcoin

⏳ La **Mempool** (Memory Pool) è l'insieme di tutte le transazioni Bitcoin valide che sono state trasmesse alla rete ma **non sono ancora state confermate** in un blocco.

---

## 🚦 Come funziona?

1. **Invio:** Quando fai una transazione, il tuo wallet la trasmette ai nodi vicini.
2. **Propagazione:** I nodi verificano la validità e la passano ad altri nodi.
3. **Attesa:** La transazione finisce nella Mempool di ogni nodo.
4. **Selezione:** I [[Bitcoin/Definizioni/Mining/⛏️ Mining\|miner]] pescano dalla Mempool le transazioni da inserire nel prossimo blocco.

---

## 💸 Il mercato delle Fee

La Mempool non è una coda "primo arrivato, primo servito". È un'asta.
I miner sono incentivati economicamente a includere le transazioni che pagano le **commissioni (fee) più alte**.

- **Alta priorità:** Paghi fee alte → entri nel prossimo blocco.
- **Bassa priorità:** Paghi fee basse → aspetti che la Mempool si svuoti.

---

## 🌊 La Mempool non è unica

Non esiste "una" Mempool centrale.  
Ogni [[Bitcoin/Definizioni/Blockchain/Full Node\|Full Node]] ha la sua versione locale della Mempool.  
Tuttavia, poiché i nodi si sincronizzano rapidamente, le Mempool tendono a essere molto simili in tutta la rete.

---

## 📉 Visualizzare la Mempool

Siti come **mempool.space** permettono di visualizzare lo stato della rete in tempo reale:
- Quante transazioni sono in attesa?
- Qual è la fee consigliata?
- Quanto è "piena" la rete?

🔗 _Approfondisci con [[Bitcoin/Definizioni/Mining/⛏️ Mining\|⛏️ Mining]], [[Bitcoin/Definizioni/Blockchain/blockchain\|blockchain]], [[Bitcoin/Definizioni/Blockchain/Full Node\|Full Node]], [[Bitcoin/Definizioni/Blockchain/UTXO\|UTXO]]_
