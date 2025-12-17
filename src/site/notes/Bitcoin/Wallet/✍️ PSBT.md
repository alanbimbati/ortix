---
{"dg-publish":true,"permalink":"/bitcoin/wallet/psbt/","title":"✍️ PSBT: firmare Bitcoin senza rischi","tags":["Bitcoin","PSBT","Sicurezza","SelfCustody","Multisig"]}
---


# ✍️ PSBT: firmare Bitcoin senza rischi

🔐 **Firmare una transazione è come mettere la tua firma su un assegno.**  
Ma quando usi Bitcoin, vuoi farlo senza mai esporre le tue chiavi private a rischi.  
Qui entra in gioco il PSBT: *Partially Signed Bitcoin Transaction*.

---

📜 **Cos’è PSBT?**

È uno standard che permette di creare e condividere una transazione Bitcoin in più fasi,  
in cui diverse parti possono **firmare senza mai vedere le chiavi private**.

---

⚙️ **Come funziona?**

1. Un wallet crea una transazione “parzialmente firmata” (PSBT) senza chiavi  
2. La invia a un altro wallet (spesso hardware o airgapped) per la firma  
3. Il wallet con la chiave privata firma la transazione senza esporre la chiave  
4. La transazione firmata torna al wallet iniziale o a un nodo per essere trasmessa

---

🛡️ **Perché è importante?**

- Permette **airgapped signing** (firma offline), aumentando la sicurezza  
- Essenziale per i wallet **multisig** (più firme richieste)  
- Riduce il rischio di furti o malware durante la firma  
- Facilita l’uso di hardware wallet insieme a software wallet (es. Sparrow + Coldcard)

---

🎯 **PSBT e Self-Custody**

PSBT è la chiave per mantenere la **massima sovranità** pur usando dispositivi diversi.  
Ti consente di firmare in modo sicuro e flessibile, anche con più persone o dispositivi.

---

💡 **Strumenti che usano PSBT**

- [[Bitcoin/Wallet/❄️ Coldcard\|❄️ Coldcard]]  
- [[Bitcoin/Wallet/✍️ SeedSigner\|✍️ SeedSigner]]
- [[Bitcoin/Wallet/🐦 Sparrow Wallet\|🐦 Sparrow Wallet]]
- Electrum  
- BlueWallet (avanzato)

---

🔥 **Conclusione**

PSBT è il ponte che collega sicurezza e praticità.  
Ti permette di firmare le tue transazioni senza mai mettere a rischio le tue chiavi.  
Se vuoi fare self-custody **seriamente**, imparare a usare PSBT è fondamentale.

---

🔗 _Approfondisci con [[Bitcoin/Wallet/🔐 Self-custody\|🔐 Self-custody]], [[Bitcoin/Wallet/🔐 Multisig\|🔐 Multisig]], [[Bitcoin/Cold Wallet\|Cold Wallet]], [[Bitcoin/Wallet/🐦 Sparrow Wallet\|🐦 Sparrow Wallet]], [[Bitcoin/Wallet/❄️ Coldcard\|❄️ Coldcard]]_