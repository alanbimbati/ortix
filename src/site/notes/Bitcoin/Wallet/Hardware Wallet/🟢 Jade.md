---
{"dg-publish":true,"permalink":"/bitcoin/wallet/hardware-wallet/jade/","title":"🟢 Jade: sicurezza open source a prezzo accessibile","tags":["Bitcoin","Wallet","Hardware","ColdStorage","SelfCustody","OpenSource","Blockstream"]}
---


# 🟢 Jade: sicurezza open source a prezzo accessibile

💎 **Jade è la dimostrazione che sicurezza e accessibilità possono coesistere.**  
Prodotto da Blockstream, costa ~70€ ma offre caratteristiche da hardware wallet premium.

---

## 🔐 Cos'è Jade?

Jade è un **[[Bitcoin/Wallet/Hardware Wallet\|hardware wallet]]** completamente **[[Bitcoin/🧬 Open Source\|🧬 Open Source]]** prodotto da Blockstream.

Versioni disponibili:
- **Jade** (~70€) → standard, supporta Bitcoin + Liquid
- **Jade Plus** (~100€) → fotocamera integrata per QR code airgapped
- **Jade DIY** (~30€) → kit fai-da-te per smanettoni

🟢 È uno dei wallet hardware con il **miglior rapporto qualità/prezzo** sul mercato.

---

## 📱 Caratteristiche

### ✅ Punti di Forza

- **Completamente open source** → hardware, firmware, app
- **Prezzo accessibile** → ~70€ per funzionalità da 200€+
- **Bitcoin-focused** → pensato prima per Bitcoin (ma supporta Liquid)
- **Secure Element virtuale** → innovazione di Blockstream (spiega sotto)
- **Display a colori** → chiaro e facile da leggere
- **Fotocamera** → versione Plus supporta QR code airgapped
- **Watch-only mode** → coordinato con Green Wallet o Sparrow
- **Blind Oracle** → sicurezza anche senza secure element fisico

### ⚠️ Limiti

- **Non completamente airgapped** → si collega via USB/Bluetooth (Plus ha QR)
- **Batteria interna** → devi ricaricarla (non alimentato solo via USB)
- **Meno popolare** → community più piccola rispetto a Ledger/Trezor
- **Liquid supportato** → alcuni puristi Bitcoin criticano questo

---

## 🧠 Il Segreto: Secure Element Virtuale

Jade usa un approccio **innovativo** per la sicurezza:

**Problema:**  
- Secure element fisici sono closed source
- Senza secure element, dispositivo vulnerabile a attacchi fisici

**Soluzione di Jade:**  
- Usa un **"Blind Oracle"** (server di Blockstream)
- La chiave è cifrata e salvata sul device
- Per decifrarla serve autenticazione con il server
- Il server non vede mai la chiave, solo conferma l'autenticazione

🔐 Risultato: **protezione fisica senza chip proprietario closed source.**

⚠️ Lato negativo: **dipendi dal server Blockstream** (ma puoi hostarlo tu stesso se vuoi).

---

## 🧠 Funzionalità

- Supporta [[Bitcoin/Wallet/✍️ PSBT\|✍️ PSBT]] e [[Bitcoin/Wallet/🔐 Multisig\|🔐 Multisig]]
- Compatibile con **Green Wallet** (Blockstream), [[Bitcoin/Wallet/🐦 Sparrow Wallet\|🐦 Sparrow Wallet]], [[Bitcoin/Wallet/⚡ Electrum\|⚡ Electrum]]
- PIN con schermata di inserimento protetta
- Recovery phrase BIP39 da 12 o 24 parole
- Supporto per **Liquid Network** (sidechain Bitcoin)
- **Jade Plus**: modalità airgapped via QR code

📱 Green Wallet si integra perfettamente con Jade ed è molto user-friendly.

---

## 🎯 Per chi è adatto?

✅ **Buono per:**
- Chi vuole **sicurezza open source a prezzo basso**
- Chi apprezza l'innovazione di Blockstream
- Chi vuole un dispositivo Bitcoin-focused (ma non only)
- Chi cerca un wallet facile da usare ma trasparente
- Chi vuole provare Liquid Network

❌ **Non ideale per:**
- Chi vuole solo Bitcoin-only puro (senza Liquid)
- Chi vuole completamente airgapped (serve Jade Plus)
- Chi diffida di Blockstream e del loro oracle
- Massimalisti che vogliono zero dipendenze esterne

---

## 🔥 Opinione

Jade è **uno dei migliori hardware wallet per rapporto qualità/prezzo.**

🟢 È open source, economico, ben progettato, e ha un approccio innovativo alla sicurezza.

⚠️ L'unico dubbio è la dipendenza dal **Blind Oracle** di Blockstream.  
Se il server Blockstream sparisce, devi self-hostare il tuo oracle… o passare a un altro wallet.

💡 Per ~70€, però, è **difficile battere Jade** in termini di sicurezza e funzionalità.  
È un'ottima scelta per chi vuole entrare nel mondo della [[Bitcoin/Wallet/🔐 Self-custody\|🔐 Self-custody]] senza spendere 250€.

---

## ✅ Conclusione

Jade è un **hardware wallet moderno, accessibile e intelligente.**

🎯 Usalo se:
- Vuoi massima sicurezza a prezzo contenuto
- Apprezzi l'innovazione open source
- Vuoi un dispositivo Bitcoin-focused
- Ti fidi di Blockstream (o sei disposto a self-hostare l'oracle)

🚫 Considera alternative se:
- Vuoi solo Bitcoin-only puro (no Liquid)
- Vuoi zero dipendenze esterne
- Vuoi un dispositivo completamente airgapped

🟢 **Jade è il miglior wallet hardware sotto i 100€.** Punto.

---

🔗 _Sito ufficiale: [blockstream.com/jade](https://blockstream.com/jade)_

📎 _Vedi anche: [[Bitcoin/Wallet/Hardware Wallet\|Hardware Wallet]], [[Bitcoin/Wallet/❄️ Coldcard\|❄️ Coldcard]], [[Bitcoin/Wallet/✍️ SeedSigner\|✍️ SeedSigner]], [[Bitcoin/Wallet/🔐 Self-custody\|🔐 Self-custody]], [[Bitcoin/Wallet/🐦 Sparrow Wallet\|🐦 Sparrow Wallet]], [[Bitcoin/🧬 Open Source\|🧬 Open Source]]_
