---
{"dg-publish":true,"permalink":"/bitcoin/definizioni/bip/bip-39-mnemonic-seed-phrases/","title":"BIP 39: Le parole che valgono tutto","tags":["Bitcoin","Sicurezza","Wallet","Standard"],"dg-note-properties":{"title":"BIP 39: Le parole che valgono tutto","tags":["Bitcoin","Sicurezza","Wallet","Standard"],"date":"2025-12-26","aliases":["BIP 39","BIP 39 – Mnemonic Seed Phrases"]}}
---


# 🗣️ BIP 39: Le parole che valgono tutto

🔑 **BIP 39** (Bitcoin Improvement Proposal 39) è lo standard che ha reso Bitcoin utilizzabile dagli umani.  
Ha trasformato stringhe esadecimali impossibili da ricordare in **12 o 24 parole semplici**.

---

## 📝 Come funziona?

Invece di gestire una chiave privata grezza come:  
`E9873D79C6D87DC0FB6A5778633389F4453213303DA61F20BD67FC233AA33262`

Il tuo wallet ti dà una **Seed Phrase** (Frase Seme):  
`witch collapse practice feed shame open despair creek road again ice least`

Queste parole sono scelte da una lista specifica di **2048 parole inglesi**.

---

## 🛡️ Sicurezza e Portabilità

- **Standard Universale:** Puoi creare un wallet su [[BlueWallet\|BlueWallet]], cancellarlo, e ripristinarlo su [[Sparrow Wallet\|Sparrow Wallet]] o [[Coldcard\|Coldcard]] usando le stesse parole.
- **Backup Analogico:** Le parole possono essere scritte su carta o incise su metallo ([[Steelwallet\|Steelwallet]]).
- **Checksum:** L'ultima parola funge da controllo. Se sbagli a scrivere una parola, il wallet se ne accorge.

---

## ⚠️ Regola d'Oro

Le parole BIP 39 **SONO** i tuoi soldi.
- Chiunque le veda può rubare tutto.
- Non scriverle mai su un computer connesso a internet (a meno che non sia un hot wallet per piccole somme).
- Non fare foto.
- Non salvarle nel cloud.

🔗 _Approfondisci con [[Bitcoin/Guide e consigli/1️⃣ Come creare una seed phrase in modo sicuro\|1️⃣ Come creare una seed phrase in modo sicuro]], [[Bitcoin/Definizioni/BIP/BIP\|BIP]], [[Bitcoin/Wallet/Hardware Wallet/Hardware Wallet\|Hardware Wallet]], [[BIP 32 – Hierarchical Deterministic Wallets\|BIP 32 – Hierarchical Deterministic Wallets]]_
