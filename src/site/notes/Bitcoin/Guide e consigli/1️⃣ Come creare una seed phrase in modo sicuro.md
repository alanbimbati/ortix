---
{"dg-publish":true,"permalink":"/bitcoin/guide-e-consigli/1-come-creare-una-seed-phrase-in-modo-sicuro/","title":"Come creare una seed phrase in modo sicuro","tags":["Bitcoin","Sicurezza","SeedPhrase","Guide","SelfCustody"],"dg-note-properties":{"title":"Come creare una seed phrase in modo sicuro","tags":["Bitcoin","Sicurezza","SeedPhrase","Guide","SelfCustody"],"date":"2024-08-09","aliases":["Creare Seed Phrase","Generazione Seed"]}}
---


# 1️⃣ Come creare una seed phrase in modo sicuro

La **Seed Phrase** (o frase di recupero) è la chiave maestra del tuo patrimonio.
Chi possiede queste 12 o 24 parole possiede i tuoi Bitcoin.
Ecco perché **come** la crei è fondamentale.

---

## 🚫 Cosa NON fare mai

1. **Non usare wallet online** (hot wallet) per somme importanti.
2. **Non fare screenshot** della seed phrase.
3. **Non salvarla su cloud** (Google Drive, iCloud, Note, Email).
4. **Non scriverla sul computer** o sul telefono mentre sei connesso a internet.
5. **Non pronunciarla ad alta voce** vicino a dispositivi "smart" (Alexa, Siri).

---

## ✅ La procedura sicura (Cold Storage)

Il metodo migliore è generare la seed phrase in un ambiente **completamente offline** (Air-Gapped).

### Metodo 1: Hardware Wallet (Consigliato)
Dispositivi come **BitBox02**, **Jade**, **Passport** o **Coldcard** generano la seed phrase usando un chip sicuro (TRNG - True Random Number Generator).
1. Inizializza il dispositivo.
2. Copia le parole su carta (o metallo) **senza che passino mai dal PC**.
3. Verifica le parole sul dispositivo.

### Metodo 2: App Mobile Offline (AirGap Vault)
Se non hai un hardware wallet, puoi usare un vecchio smartphone **resettato e senza SIM/WiFi**.
1. Scarica **[[Bitcoin/Wallet/Software Wallet/🔒 Airgap Vault\|🔒 Airgap Vault]]** o **[[Bitcoin/Wallet/Software Wallet/🔵 BlueWallet\|🔵 BlueWallet]]**.
2. Metti il telefono in **Modalità Aereo** (o meglio, rimuovi fisicamente i moduli se sei paranoico).
3. Genera il wallet.
4. Copia la seed phrase su carta.
5. **Verifica il backup prima di tutto** ✅: cancella il wallet dall'app, reimportalo usando solo le parole scritte su carta e controlla che il primo indirizzo di ricezione sia identico a quello di prima. Se qualcosa non torna, hai sbagliato a trascrivere: meglio scoprirlo adesso, a wallet vuoto.
6. Solo dopo il test, cancella l'app o il telefono se non lo usi come cold storage dedicato.

### Metodo 3: Dadi (Entropia Fisica)
Per i veri cypherpunk. Non ti fidi del software? Usa la fisica.
1. Prendi un dado da 6 facce.
2. Lancialo circa 100 volte. Ogni lancio di un D6 vale circa 2,58 bit di entropia, quindi per arrivare a 256 bit (una seed da 24 parole) servono circa 99-100 lanci. Annota ogni risultato nell'ordine, senza saltarne né ripeterne.
3. **Non** convertire i lanci in parole scegliendole a mano dalla [lista BIP39](https://ortix.vercel.app/bitcoin/definizioni/bip/bip-39-mnemonic-seed-phrases/). L'ultima parola contiene un **checksum** calcolato a partire dall'entropia: se lo sbagli, la seed non è valida oppure non è quella che credi. Il calcolo va fatto da un dispositivo offline.
4. Molti hardware wallet (es. Coldcard, Jade) permettono di inserire i lanci di dadi per calcolare la seed phrase.

⚠️ La procedura passo passo è nel [🥇 Metodo 3 — Creazione di un wallet Livello Difficile](https://ortix.vercel.app/bitcoin/come-creare-un-wallet/metodo-3-crazione-di-un-wallet-livello-difficile/). Lì trovi la funzione «Fornisci entropia» di BlueWallet, che calcola checksum e parole, e il numero di lanci necessari.

Con i dadi l'errore umano è il rischio principale: un lancio annotato male o una parola trascritta storta e la seed non è più quella giusta. Prima di ricevere anche un solo sat fai lo **stress test di ripristino**: cancella il wallet, reimportalo dalle parole su carta e controlla che gli indirizzi coincidano. Senza questo test non hai un backup, hai solo un foglio con delle parole sopra.

---

## 🔒 Come conservarla

Una volta generata, la conservazione è vitale.

- **Carta:** Scrivila su un foglio. Attenzione a fuoco e acqua.
- **Metallo:** Incidila su piastre d'acciaio (es. Cryptosteel) per resistere a incendi e allagamenti.
- **Passphrase:** Aggiungi una "25esima parola" (password) che protegge la seed phrase. Se qualcuno trova le 24 parole ma non ha la passphrase, il wallet è vuoto.

> **Ricorda:** Non sei tu a scegliere le parole. È la matematica che le sceglie per te. Tu devi solo proteggerle.

---

🔗 _Approfondisci con [[Bitcoin/Guide e consigli/🔑 Come creare un Wallet (non custodial)\|🔑 Come creare un Wallet (non custodial)]], [[Bitcoin/Definizioni/Blockchain/🔐 Self-custody\|🔐 Self-custody]], [[Ortix/Filosofia/🛡️ Sovranità digitale\|🛡️ Sovranità digitale]]_