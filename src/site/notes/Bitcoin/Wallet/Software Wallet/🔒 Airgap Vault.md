---
{"dg-publish":true,"permalink":"/bitcoin/wallet/software-wallet/airgap-vault/","title":"🔒 Airgap Vault: firmare transazioni senza rischi","tags":["Bitcoin","Airgap","Sicurezza","PSBT","ColdStorage","SelfCustody"]}
---


# 🔒 Airgap Vault: firmare transazioni senza rischi

🛰️ **Immagina un monaco in cima alla montagna: non parla con nessuno, ma può approvare ogni tua decisione.**  
Questo è un *Airgap Vault*: un dispositivo completamente **offline**, progettato per **firmare transazioni Bitcoin senza mai toccare internet.**

---

📡 **Cos'è un Airgap Vault?**

È un wallet isolato fisicamente e digitalmente dal mondo esterno.  
Niente Wi-Fi. Niente Bluetooth. Niente porte USB attive. Nessuna connessione.

✅ Firma le transazioni tramite **PSBT** (Partially Signed Bitcoin Transaction)  
✅ Comunica solo con **QR code** o **microSD**

👁️‍🗨️ Non può essere attaccato da virus, malware, hacker… perché **non ha una porta d'ingresso.**

---

🧱 **Esempi reali**

- [[Bitcoin/Wallet/Hardware Wallet/✍️ SeedSigner\|✍️ SeedSigner]] → fotocamera + QR, nessuna memoria permanente  
- [[Bitcoin/Wallet/Hardware Wallet/❄️ Coldcard\|❄️ Coldcard]] → microSD per firmare e trasmettere  
- Laptop con [[Bitcoin/Wallet/Software Wallet/⚡ Electrum\|⚡ Electrum]] offline e chiavetta USB (se configurato bene)

---

🔐 **Perché è sicuro?**

- Le **chiavi private non escono mai** dal vault  
- Anche se il wallet “connesso” viene compromesso, **non può firmare nulla** da solo  
- Airgap = barriera fisica, non solo logica

📦 È come firmare contratti in una stanza blindata, mentre i dati viaggiano con corrieri… ma **senza aprire la porta.**

---

⚙️ **Come si usa**

1. Il wallet online prepara una transazione → file PSBT  
2. La invii al vault (via microSD o QR)  
3. Il vault firma la transazione  
4. Rimandi il file firmato al wallet online  
5. Lo trasmetti alla rete

🧠 La firma avviene **offline**. Il broadcast avviene **online**. Sicurezza totale.

---

🔗 _Vedi anche: [[Bitcoin/Definizioni/Blockchain/✍️ PSBT\|✍️ PSBT]], [[Bitcoin/Wallet/Hardware Wallet/✍️ SeedSigner\|✍️ SeedSigner]], [[Bitcoin/Wallet/Hardware Wallet/❄️ Coldcard\|❄️ Coldcard]], [[Bitcoin/Wallet/Software Wallet/🐦 Sparrow Wallet\|🐦 Sparrow Wallet]], [[Bitcoin/Definizioni/Blockchain/🔐 Self-custody\|🔐 Self-custody]], [[Bitcoin/Definizioni/Blockchain/Cold Wallet\|Cold Wallet]]_