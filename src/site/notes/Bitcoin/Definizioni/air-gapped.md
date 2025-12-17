---
{"dg-publish":true,"permalink":"/bitcoin/definizioni/air-gapped/","title":"🛡️ Air-gapped – Separare custodia e uso in Bitcoin","tags":["bitcoin","self-custody","airgap","sicurezza","coldwallet"]}
---


# 🛡️ Air-gapped – Separare custodia e uso

In Bitcoin, la **sicurezza nasce dalla separazione**.  
L’idea di **air-gapped** è proprio questa: un dispositivo è **fisicamente isolato da internet**.

---

## 🧠 Cos’è un dispositivo air-gapped

Un dispositivo air-gapped:

- **non ha connessione internet**
- **non comunica direttamente con altri dispositivi**
- conserva le chiavi private al sicuro
- firma transazioni offline

> In poche parole: è un **[[Bitcoin/Cold Wallet\|Cold Wallet]] estremo**, protetto da qualsiasi attacco remoto.

---

## 🔄 Perché è importante

- Previene furti via malware o hacking
- Riduce il rischio di esposizione accidentale della chiave privata
- Permette di firmare transazioni in sicurezza
- Abitua l’utente a un **modello di custodia consapevole**

---

## 🪜 Come funziona in pratica

### 1️⃣ Dispositivo offline (Airgap Vault, hardware wallet)
- genera la seed
- conserva le chiavi
- firma transazioni

### 2️⃣ Dispositivo online (BlueWallet, Electrum)
- mostra saldo e transazioni
- prepara transazioni da firmare
- trasmette la transazione firmata

**Comunicazione:** tramite QR code o file [[Bitcoin/Wallet/✍️ PSBT\|✍️ PSBT]]  
**Mai esposizione diretta della chiave privata**

---

## 💡 Concetto chiave

> Air-gapped significa **separazione fisica e concettuale** tra custodia e utilizzo.  
> È il principio base dei cold wallet avanzati e della self-custody responsabile.

---

## 🌱 Benefici

- Sicurezza estrema senza fiducia esterna
- Controllo totale delle proprie risorse
- Educazione alla responsabilità finanziaria
- Applicabile a wallet hardware e software offline

---

## ⚠️ Limiti

- Minor comodità rispetto ai wallet hot
- Necessita di procedure consapevoli per firmare e trasmettere
- Non elimina tutti i rischi, ma li rende **gestibili e comprensibili**

---
