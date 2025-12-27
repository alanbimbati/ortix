---
{"dg-publish":true,"permalink":"/bitcoin/definizioni/blockchain/utxo/","title":"UTXO: il modello delle banconote digitali","tags":["Bitcoin","UTXO","Tecnologia","Blockchain","Transazioni","Privacy"]}
---

# 🧾 UTXO: il modello delle banconote digitali

💰 **UTXO sta per "Unspent Transaction Output" (Output di Transazione Non Speso).**  
È il modo in cui Bitcoin tiene traccia di chi possiede cosa, **senza usare saldi**.

---

## 🤔 Cos'è un UTXO?

Invece di avere un "saldo" nel tuo wallet (come in un conto bancario), Bitcoin usa **output non spesi**.

**Analogia con il contante:**
- Hai un portafoglio con banconote da 10€, 20€, 50€
- Ogni banconota è **separata e indipendente**
- Quando paghi, usi una o più banconote
- Se la banconota è troppo grande, ricevi il **resto**

🧾 **Gli UTXO funzionano esattamente così.**

---

## ⚙️ Come Funziona?

### Esempio Pratico

1. **Ricevi 1 BTC** da Alice  
   → Crei un UTXO da 1 BTC a tuo nome

2. **Ricevi 0.5 BTC** da Bob  
   → Crei un altro UTXO da 0.5 BTC

**Il tuo "saldo" è 1.5 BTC, ma in realtà hai 2 UTXO separati:**
- UTXO #1: 1 BTC
- UTXO #2: 0.5 BTC

3. **Vuoi inviare 1.2 BTC a Carlo**  
   → Devi usare **entrambi gli UTXO** (1 + 0.5 = 1.5 BTC)  
   → Invii 1.2 BTC a Carlo  
   → Ricevi **0.3 BTC di resto** come nuovo UTXO

**Risultato finale:**
- UTXO #1 e #2 → **spesi** (non esistono più)
- Nuovo UTXO di Carlo → 1.2 BTC
- Nuovo UTXO tuo (resto) → 0.3 BTC

---

## 🆚 UTXO vs Modello Account

### Modello Account (Ethereum, banche)
- Ogni account ha un **saldo**
- Le transazioni **modificano il saldo**
- Semplice da capire, ma meno privacy

### Modello UTXO (Bitcoin)
- Non ci sono "saldi", solo **output non spesi**
- Ogni transazione **consuma UTXO vecchi e crea UTXO nuovi**
- Più complesso, ma **migliore per privacy e sicurezza**

---

## ✅ Vantaggi del Modello UTXO

### 1. Privacy
🕵️ Ogni UTXO è **indipendente**.  
Puoi usare indirizzi diversi per ogni transazione, rendendo più difficile tracciare i tuoi fondi.

### 2. Parallelizzazione
⚡ Le transazioni che usano UTXO diversi possono essere **verificate in parallelo**.  
Migliora l'efficienza della rete.

### 3. Sicurezza
🔐 Ogni UTXO ha la propria **firma crittografica**.  
Non puoi spendere un UTXO senza la chiave privata corretta.

### 4. Auditabilità
📊 È facile verificare che **nessun bitcoin sia stato creato dal nulla**.  
Ogni UTXO ha una storia tracciabile fino al blocco di origine.

---

## 🧠 UTXO Management

### Consolidamento
Se hai **molti UTXO piccoli**, il tuo wallet potrebbe diventare inefficiente.  
Soluzione: **consolidare** gli UTXO in uno più grande quando le fee sono basse.

**Esempio:**
- Hai 10 UTXO da 0.01 BTC ciascuno
- Li consolidi in 1 UTXO da 0.1 BTC
- Risparmi fee nelle transazioni future

### Coin Control
🎯 Alcuni wallet avanzati (come [[Bitcoin/Wallet/Software Wallet/🐦 Sparrow Wallet\|🐦 Sparrow Wallet]]) permettono di **scegliere quali UTXO usare** in una transazione.

**Perché è utile:**
- Gestire la privacy (evitare di collegare UTXO)
- Ottimizzare le fee
- Evitare di spendere UTXO "sporchi" (da fonti non desiderate)

---

## 🔗 UTXO e Privacy

### Problema: Collegamento UTXO
Se usi **più UTXO nella stessa transazione**, riveli che appartengono alla stessa persona.

**Esempio:**
- UTXO #1 da Alice
- UTXO #2 da Bob
- Li usi insieme → **Alice e Bob sanno che sei la stessa persona**

### Soluzione: CoinJoin
[[Bitcoin/Definizioni/Blockchain/🌀 CoinJoin\|🌀 CoinJoin]] mescola UTXO di più utenti, rendendo difficile tracciare chi possiede cosa.

---

## 🧮 UTXO nella Blockchain

Ogni [[Bitcoin/Definizioni/Blockchain/blockchain\|blocco]] contiene transazioni che:
1. **Consumano** UTXO esistenti (input)
2. **Creano** nuovi UTXO (output)

**Regola fondamentale:**  
La somma degli input deve essere **maggiore o uguale** alla somma degli output.

La differenza è la **fee** pagata ai [[Bitcoin/Definizioni/Mining/⛏️ Mining\|miner]].

---

## 🔥 Conclusione

🧾 **Gli UTXO sono il cuore del modello di transazioni di Bitcoin.**

Invece di saldi modificabili, Bitcoin usa **banconote digitali** che vengono spese e ricreate.

Questo modello offre:
- ✅ Maggiore privacy
- ✅ Migliore sicurezza
- ✅ Parallelizzazione efficiente
- ✅ Auditabilità completa

💡 Capire gli UTXO è fondamentale per **gestire i tuoi bitcoin in modo intelligente** e proteggere la tua privacy.

---

🔗 _Approfondisci con [[Bitcoin/🔧 Bitcoin dal punto di vista tecnologico\|🔧 Bitcoin dal punto di vista tecnologico]], [[Bitcoin/Definizioni/Blockchain/blockchain\|blockchain]], [[Bitcoin/Definizioni/Blockchain/🌀 CoinJoin\|🌀 CoinJoin]], [[Bitcoin/Filosofia/🕵️‍♂️ Privacy\|🕵️‍♂️ Privacy]], [[Bitcoin/Wallet/Software Wallet/🐦 Sparrow Wallet\|🐦 Sparrow Wallet]], [[Bitcoin/Definizioni/Mining/⛏️ Mining\|⛏️ Mining]]_