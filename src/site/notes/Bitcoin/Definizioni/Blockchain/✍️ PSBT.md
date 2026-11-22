---
{"dg-publish":true,"permalink":"/bitcoin/definizioni/blockchain/psbt/","title":"✍️ PSBT: firmare Bitcoin senza rischi","tags":["Bitcoin","PSBT","Sicurezza","SelfCustody","Multisig"],"dg-note-properties":{"title":"✍️ PSBT: firmare Bitcoin senza rischi","tags":["Bitcoin","PSBT","Sicurezza","SelfCustody","Multisig"],"date":"2025-07-09"}}
---


# ✍️ PSBT: firmare Bitcoin senza rischi

🔐 **Firmare una transazione è come mettere la tua firma su un assegno.**  
Ma quando usi Bitcoin, vuoi farlo senza mai esporre le tue chiavi private a rischi.  
Qui entra in gioco il PSBT: *Partially Signed Bitcoin Transaction*.

---

📜 **Cos’è PSBT?**

È uno standard che permette di creare e condividere una transazione Bitcoin in più fasi,  
in cui diverse parti possono **firmare senza mai vedere le chiavi private**.

🔑 **Cosa c'è dentro, e cosa no.** Un PSBT contiene i dati della transazione: gli UTXO che stai spendendo, gli indirizzi di destinazione e di resto, gli importi, la fee e le informazioni pubbliche che servono a chi firma per riconoscere le proprie chiavi. **Le chiavi private non ci sono mai.** Il file può passare da un computer online senza che nessuno possa spendere i tuoi sats. Chi lo intercetta però vede i tuoi movimenti: il PSBT non dà potere di spesa, ma non è anonimo.

---

⚙️ **Come funziona?**

1. Un wallet crea una transazione “parzialmente firmata” (PSBT) senza chiavi  
2. La invia a un altro wallet (spesso hardware o airgapped) per la firma  
3. Il wallet con la chiave privata firma la transazione senza esporre la chiave  
4. La transazione firmata torna al wallet iniziale o a un nodo per essere trasmessa

---

📦 **Come viaggia il PSBT tra i dispositivi**

Il PSBT è un file e può spostarsi in quattro modi:

- **QR code**: il wallet mostra un QR (spesso animato) e il dispositivo offline lo legge con la fotocamera. È il canale di [SeedSigner](https://ortix.vercel.app/bitcoin/wallet/hardware-wallet/seed-signer/) e delle versioni airgapped di altri dispositivi.
- **microSD**: il file si salva su una scheda che si sposta a mano, come con [Coldcard](https://ortix.vercel.app/bitcoin/wallet/hardware-wallet/coldcard/).
- **USB**: cavo diretto tra computer e hardware wallet, come con [BitBox02](https://ortix.vercel.app/bitcoin/wallet/hardware-wallet/bit-box02/) o [Jade](https://ortix.vercel.app/bitcoin/wallet/hardware-wallet/jade/). È comodo, ma il dispositivo non è più [air-gapped](https://ortix.vercel.app/bitcoin/definizioni/blockchain/air-gapped/).
- **NFC**: avvicini il telefono o il computer al dispositivo, come con [ColdCard Q](https://ortix.vercel.app/bitcoin/wallet/hardware-wallet/cold-card-q/).

🧪 **Esempio: Sparrow + Coldcard via microSD**

1. In [Sparrow](https://ortix.vercel.app/bitcoin/wallet/software-wallet/sparrow-wallet/), che conosce solo le chiavi pubbliche, preparo la transazione e la salvo come file PSBT sulla microSD.
2. Inserisco la scheda nella Coldcard, che non è mai collegata a internet.
3. Sul display della Coldcard controllo destinazione, importo e fee, poi confermo.
4. La Coldcard scrive la transazione firmata sulla stessa microSD.
5. Riporto la scheda nel computer, carico il file in Sparrow e trasmetto.

✅ **La regola d'oro: verifica sul display del dispositivo che firma.** Il computer può essere compromesso, e un malware può cambiare l'indirizzo di destinazione nel PSBT. L'unico schermo di cui ti puoi fidare è quello del dispositivo che custodisce la chiave. Prima di confermare controlla lì:

- l'**indirizzo** di destinazione (tutto, non solo le prime lettere);
- l'**importo**;
- la **fee**;
- che il **resto** torni a un indirizzo tuo.

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

- [[Bitcoin/Wallet/Hardware Wallet/❄️ Coldcard\|❄️ Coldcard]]  
- [[Bitcoin/Wallet/Hardware Wallet/✍️ SeedSigner\|✍️ SeedSigner]]
- [[Bitcoin/Wallet/Software Wallet/🐦 Sparrow Wallet\|🐦 Sparrow Wallet]]
- Electrum  
- BlueWallet (avanzato)

---

⚠️ **Limiti e rischi**

- **Errori di verifica**: il PSBT protegge le chiavi, non la tua attenzione. Se confermi senza leggere il display, o controlli l'indirizzo solo sul computer, firmi quello che ha deciso qualcun altro.
- **Compatibilità tra wallet**: lo standard è uno, ma i software non lo applicano tutti allo stesso modo. Cambiano i formati dei QR animati, le versioni del PSBT e le funzioni supportate, e un dispositivo può rifiutare un file creato da un altro wallet. Prima di affidare cifre importanti a una combinazione nuova, prova il giro completo con una piccola somma.
- **Multisig complessi**: con molti input e più firmatari il PSBT diventa pesante. I QR animati si allungano e il file deve passare da un dispositivo all'altro raccogliendo le firme. Ogni dispositivo deve conoscere la configurazione completa del [multisig](https://ortix.vercel.app/bitcoin/definizioni/blockchain/multisig/), altrimenti non riesce a riconoscere il resto come tuo. Più passaggi vogliono dire più occasioni di errore.
- **Privacy del file**: il PSBT mostra i tuoi UTXO e i tuoi indirizzi. Non lasciarlo su microSD o cartelle condivise dopo l'uso.

Per il flusso di firma completamente offline vedi anche [Airgap Vault](https://ortix.vercel.app/bitcoin/wallet/software-wallet/airgap-vault/).

---

🔥 **Conclusione**

PSBT è il ponte che collega sicurezza e praticità.  
Ti permette di firmare le tue transazioni senza mai mettere a rischio le tue chiavi.  
Se vuoi fare self-custody **seriamente**, imparare a usare PSBT è fondamentale.

---

🔗 _Approfondisci con [[Bitcoin/Definizioni/Blockchain/🔐 Self-custody\|🔐 Self-custody]], [[Bitcoin/Definizioni/Blockchain/🔐 Multisig\|🔐 Multisig]], [[Bitcoin/Definizioni/Blockchain/Cold Wallet\|Cold Wallet]], [[Bitcoin/Wallet/Software Wallet/🐦 Sparrow Wallet\|🐦 Sparrow Wallet]], [[Bitcoin/Wallet/Hardware Wallet/❄️ Coldcard\|❄️ Coldcard]]_