---
{"dg-publish":true,"permalink":"/bitcoin/bitcoin-dal-punto-di-vista-tecnologico/","title":"🔧 Bitcoin dal punto di vista tecnologico","tags":["Bitcoin","Tecnologia","Blockchain","Crittografia","ProofOfWork","Nodi"]}
---


# 🔧 Bitcoin dal punto di vista tecnologico

![Bitcoin Technology](/img/user/Immagini/Ortix_BitcoinTecnologia.jpg)

Bitcoin è un **protocollo open source** che implementa un sistema di pagamento peer-to-peer decentralizzato.  
Non è un'app, non è un'azienda: è **un'infrastruttura pubblica** che nessuno può spegnere.

---

## 🏗️ Architettura del sistema

Bitcoin si basa su diversi componenti tecnologici che lavorano insieme:

### 1. [[Bitcoin/Definizioni/Blockchain/blockchain\|Blockchain]]
Un registro distribuito e immutabile che contiene tutte le transazioni mai effettuate.  
Ogni blocco è collegato crittograficamente al precedente tramite [[Bitcoin/Definizioni/Blockchain/hash\|hash]].

**Caratteristiche:**
- **Immutabilità**: modificare il passato richiederebbe ricalcolare tutti i blocchi successivi
- **Trasparenza**: chiunque può verificare l'intera storia delle transazioni
- **Decentralizzazione**: migliaia di copie identiche distribuite globalmente

🔗 Vedi anche: [[Bitcoin/Definizioni/Blockchain/Full Node\|Full Node]], [[Bitcoin/Definizioni/Blockchain/UTXO\|UTXO]]

---

### 2. [[Bitcoin/Definizioni/Mining/⚙️  Proof of Work\|⚙️  Proof of Work]]
Il meccanismo di consenso che protegge la rete da attacchi.  
I [[Bitcoin/Definizioni/Mining/⛏️ Mining\|miner]] competono per trovare un [[Bitcoin/Definizioni/Blockchain/hash\|hash]] valido, consumando energia reale.

**Perché è importante:**
- Rende costoso attaccare la rete
- Trasforma energia in sicurezza
- Crea un ancoraggio al mondo fisico

🔗 Vedi anche: [[Bitcoin/Definizioni/Mining/⛏️ Mining\|⛏️ Mining]], [[Bitcoin/Definizioni/Mining/🌱 Mining Green\|🌱 Mining Green]], [[Bitcoin/Definizioni/Mining/🍀Il mining di Bitcoin riduce l'inquinamento\|🍀Il mining di Bitcoin riduce l'inquinamento]]

---

### 3. [[Bitcoin/Definizioni/Blockchain/Full Node\|Nodi completi]]
Software che verifica **ogni transazione** e **ogni blocco** secondo le regole del protocollo.

**Cosa fa un nodo:**
- Scarica l'intera blockchain
- Verifica tutte le firme crittografiche
- Rifiuta transazioni e blocchi invalidi
- Propaga transazioni valide alla rete

**Perché è fondamentale:**
- Non devi fidarti di nessuno: **verifichi tu stesso**
- Più nodi = più decentralizzazione
- Chiunque può gestire un nodo

🔗 Vedi anche: [[Bitcoin/Filosofia/🕸️ Decentralizzazione\|🕸️ Decentralizzazione]]

---

### 4. Crittografia a chiave pubblica

Bitcoin usa crittografia asimmetrica per garantire proprietà e sicurezza:

- **Chiave privata**: il segreto che ti permette di spendere i tuoi bitcoin
- **Chiave pubblica**: derivata dalla privata, usata per generare indirizzi
- **[[Firme digitali\|Firme digitali]]**: provano che sei il proprietario senza rivelare la chiave privata

**Componenti crittografici:**
- [[Hash crittografici\|Hash crittografici]]: SHA-256, RIPEMD-160
- [[Firme digitali\|Firme digitali]]: ECDSA, Schnorr
- Curve ellittica: secp256k1

---

### 5. [[Bitcoin/Definizioni/Blockchain/🧠 Seed Phrase\|Seed Phrase]] e [[Bitcoin/Wallet/🌳 Wallet gerarchico\|Wallet gerarchici]]

I wallet moderni usano lo standard **BIP39** per generare chiavi:

1. Una [[Bitcoin/Definizioni/Blockchain/🧠 Seed Phrase\|🧠 Seed Phrase]] (12-24 parole) rappresenta il tuo "seme" crittografico
2. Da questa vengono derivate **infinite chiavi** in modo deterministico
3. Ogni chiave può ricevere bitcoin in modo indipendente

**Standard importanti:**
- [[Bitcoin/Definizioni/BIP/BIP\|BIP]]: Bitcoin Improvement Proposals
- [[Bitcoin/Wallet/🌳 Wallet gerarchico\|🌳 Wallet gerarchico]]: HD Wallets (BIP32, BIP44)
- [[Bitcoin/Definizioni/Blockchain/xpub\|xpub]]: chiave pubblica estesa per generare indirizzi

🔗 Vedi anche: [[Bitcoin/Wallet/🧭 Wallet Index\|🧭 Wallet Index]], [[Bitcoin/Guide e consigli/1️⃣ Come creare una seed phrase in modo sicuro\|1️⃣ Come creare una seed phrase in modo sicuro]]

---

## 🔐 Modelli di custodia e sicurezza

### [[Bitcoin/Definizioni/Blockchain/🔐 Self-custody\|Self-Custody]]
**"Not your keys, not your coins"**

Quando custodisci i tuoi bitcoin:
- Controlli le chiavi private
- Nessuno può bloccare o confiscare i tuoi fondi
- Sei responsabile della sicurezza

### [[Bitcoin/Definizioni/Blockchain/Cold Wallet\|Cold Wallet]] e [[Bitcoin/Definizioni/Blockchain/air-gapped\|air-gapped]]
Wallet che **non sono mai connessi a internet**:
- Massima sicurezza contro attacchi remoti
- Usati per grandi somme
- Richiedono procedure più complesse

🔗 Vedi anche: [[Bitcoin/Wallet/Hardware Wallet/Hardware Wallet\|Hardware Wallet]], [[Bitcoin/Wallet/🪨 Steelwallet\|🪨 Steelwallet]]

### [[Bitcoin/Definizioni/Blockchain/🔐 Multisig\|Multisig]]
Richiede **più firme** per autorizzare una transazione.

**Esempi:**
- 2-di-3: servono 2 chiavi su 3 per spendere
- 3-di-5: servono 3 chiavi su 5

**Vantaggi:**
- Riduce il rischio di singolo punto di fallimento
- Utile per aziende o eredità
- Maggiore sicurezza contro furto

---

## 🔒 Privacy e fungibilità

### [[Bitcoin/Definizioni/Blockchain/🌀 CoinJoin\|CoinJoin]]
Tecnica per **mescolare transazioni** di più utenti, rendendo difficile tracciare i flussi.

**Come funziona:**
- Più utenti creano una transazione collaborativa
- Gli input e output vengono mescolati
- Difficile capire chi ha pagato chi

### [[Bitcoin/Definizioni/Blockchain/✍️ PSBT\|PSBT]] (Partially Signed Bitcoin Transaction)
Standard per creare transazioni che richiedono **più firme** in momenti diversi.

**Casi d'uso:**
- Multisig
- Hardware wallet
- Coordinazione tra più dispositivi

---

## ⚡ Scalabilità: [[Bitcoin/Lightning Network/⚡ Lightning Network\|Lightning Network]]

Bitcoin on-chain può gestire ~7 transazioni al secondo.  
Per pagamenti istantanei e micropagamenti serve un [[Bitcoin/Lightning Network/🧱 Layer 2\|🧱 Layer 2]].

### Come funziona Lightning
1. Apri un **canale di pagamento** on-chain
2. Fai transazioni **istantanee e quasi gratuite** off-chain
3. Chiudi il canale quando vuoi, registrando il saldo finale on-chain

**Vantaggi:**
- Transazioni in millisecondi
- Commissioni trascurabili
- Scalabilità praticamente infinita

🔗 Vedi anche: [[Bitcoin/Lightning Network/⚡ Scalabilità di Lightning Network\|⚡ Scalabilità di Lightning Network]], [[Bitcoin/Lightning Network/⚡️ Bitcoin come una Carta Prepagata\|⚡️ Bitcoin come una Carta Prepagata]]

---

## 🧱 Componenti tecnici avanzati

### [[Bitcoin/Definizioni/Blockchain/UTXO\|UTXO]] (Unspent Transaction Output)
Bitcoin non usa "saldi" ma **output non spesi**.

**Analogia:**
- Come avere banconote di diverso taglio
- Ogni UTXO è una "banconota" che puoi spendere
- Quando spendi, crei nuovi UTXO

### [[Bitcoin/Definizioni/Blockchain/blockchain\|Blockchain]] e consenso distribuito
- **Difficoltà dinamica**: si aggiusta ogni 2016 blocchi (~2 settimane)
- **Tempo di blocco**: ~10 minuti in media
- **Ricompensa**: dimezzata ogni 210.000 blocchi (halving)

---

## 🛠️ Strumenti e standard

### [[Bitcoin/Definizioni/BIP/BIP\|Bitcoin Improvement Proposals]]
Proposte per migliorare il protocollo Bitcoin.

**Esempi importanti:**
- BIP32: HD Wallets
- BIP39: Mnemonic seed phrases
- BIP141: SegWit
- BIP340-342: Taproot

### Software e implementazioni
- **Bitcoin Core**: implementazione di riferimento
- **btcd**: implementazione in Go
- **libbitcoin**: libreria C++

---

## 🔗 Collegamenti alle altre "porte"

Bitcoin non è solo tecnologia. Esplora anche:

- 💰 **Economia**: [[Bitcoin/Economia/📉 Inflazione\|📉 Inflazione]], [[Bitcoin/Economia/💰 Le caratteristiche del vero denaro\|💰 Le caratteristiche del vero denaro]]
- 🧠 **Filosofia**: [[Bitcoin/Filosofia/🕸️ Decentralizzazione\|🕸️ Decentralizzazione]]
- 🔐 **Privacy**: [[Bitcoin/Filosofia/🕵️‍♂️ Privacy\|🕵️‍♂️ Privacy]], [[Bitcoin/Definizioni/Blockchain/🌀 CoinJoin\|🌀 CoinJoin]]
- ⚡ **Energia**: [[Bitcoin/Definizioni/Mining/🌱 Mining Green\|🌱 Mining Green]], [[Bitcoin/Definizioni/Mining/🍀Il mining di Bitcoin riduce l'inquinamento\|🍀Il mining di Bitcoin riduce l'inquinamento]]
- 📚 **Guide pratiche**: [[Bitcoin/Guide e consigli/🔑 Come creare un Wallet (non custodial)\|🔑 Come creare un Wallet (non custodial)]], [[Bitcoin/Guide e consigli/Acquistare Bitcoin\|Acquistare Bitcoin]]

---

## 📜 Conclusione

Bitcoin è **ingegneria monetaria**.  
Ogni componente è progettato per funzionare **senza fiducia**, solo con **verifica matematica**.

🔧 Non serve permesso per partecipare.  
🔧 Non serve fiducia per verificare.  
🔧 Non serve intermediario per transare.

**Questa è la rivoluzione tecnologica di Bitcoin.**

---

🔙 Torna alla [[Bitcoin/Bitcoin\|home di Bitcoin]]
