---
{"dg-publish":true,"permalink":"/bitcoin/definizioni/hash/","title":"Hash","tags":["bitcoin","crittografia","sicurezza","hash","blockchain"]}
---


# 🧩 Hash

🔐 Un **hash** è una stringa alfanumerica fissa, generata da una funzione matematica che prende in input qualsiasi dato. È come un'impronta digitale: **breve, unica e non reversibile**.

---

## ⚙️ Come funziona?

🧠 Una **funzione di hash** prende un input di qualsiasi lunghezza e restituisce un output (l'hash) **a lunghezza fissa**.

Esempio (SHA-256):  
- Input: `Bitcoin è libertà`  
- Output: `cd0f2c5b4573b79b27f8a00a64adf1d7c8f7f9f03220c213c8e0bfa594c2978b`

---

## 🔐 Proprietà fondamentali

- ✂️ **Deterministico**: stesso input → stesso output
- 🔁 **Non reversibile**: non puoi risalire all’input dall’hash
- 🧩 **Univoco**: due input diversi producono hash diversi (collisioni estremamente rare)
- 🧱 **Velocissimo da calcolare**
- 🧪 **Sensibile**: anche un solo bit di differenza cambia completamente l'hash

---

## 🔗 Usi nel mondo Bitcoin

- 📦 Ogni **blocco** ha un hash che lo collega al precedente → [[Bitcoin/Definizioni/blockchain\|blockchain]]
- 🔒 Le transazioni sono identificate tramite hash
- 🧮 Il [[Bitcoin/Mining/⛏️ Mining\|⛏️ Mining]] cerca un hash che inizi con un certo numero di zeri → [[Bitcoin/Mining/⚙️  Proof of Work\|⚙️  Proof of Work]]

---

## 🧮 Esempi famosi

- 📌 **SHA-256**: usato in [[Bitcoin/Bitcoin\|Bitcoin]], resistente e consolidato
- 🧱 **RIPEMD160**: per comprimere gli hash pubblici negli indirizzi
- 🔁 **Double Hashing**: SHA256(SHA256(x)) è una pratica comune per aumentare la sicurezza


---

🧠 **Un hash non è cifrato**, non contiene il dato, ma lo rappresenta come **identificatore univoco e sicuro**. È la spina dorsale della fiducia matematica di Bitcoin.

---

🔗 #Hash #Bitcoin #SHA256 #Blockchain #Sicurezza #SovranitàDigitale #Ortix