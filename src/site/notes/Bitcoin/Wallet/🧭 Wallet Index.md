---
{"dg-publish":true,"permalink":"/bitcoin/wallet/wallet-index/","title":"🧭 Wallet Index: tutti i portafogli Bitcoin a confronto","tags":["Bitcoin","Wallet","SelfCustody","Lightning","Sicurezza","Confronto"],"dg-note-properties":{"title":"🧭 Wallet Index: tutti i portafogli Bitcoin a confronto","tags":["Bitcoin","Wallet","SelfCustody","Lightning","Sicurezza","Confronto"],"date":"2025-07-09"}}
---


# 🧭 Wallet Index: tutti i portafogli Bitcoin a confronto

📦 Che tu voglia un wallet super semplice o una cassaforte digitale, qui trovi una selezione dei principali wallet Bitcoin **organizzati per tipo**, con una tabella comparativa completa per **scegliere quello giusto per te**.

---

## 🗂️ Tabella comparativa

| Wallet                | Custodial | Rete        | Complessità    | Sicurezza    | Grafica UI         | Funzionalità principali                                    | Link |
| --------------------- | --------- | ----------- | -------------- | ------------ | ------------------ | ---------------------------------------------------------- | ---- |
| [[Bitcoin/Wallet/Software Wallet/🟠 Wallet of Satoshi\|🟠 Wallet of Satoshi]] | ✅ Sì      | ⚡ Lightning | 🔰 Molto bassa | ❌ Bassa      | 🎨 Molto semplice  | Pagamenti istantanei custodial                             | 🟠   |
| [[Bitcoin/Wallet/Software Wallet/🕊 Phoenix Wallet\|🕊 Phoenix Wallet]]    | ❌ No      | ⚡ Lightning | 🟡 Media       | ✅ Alta       | 🎨 Pulita          | Canali automatici, non-custodial                           | 🔥   |
| [[Bitcoin/Wallet/Software Wallet/🔵 BlueWallet\|🔵 BlueWallet]]        | ✅/❌       | ⚡ / ₿       | 🟡 Media       | ⚠️ Mista     | 🎨 Moderna         | LN custodial, on-chain non-custodial, multisig, watch-only | 🔵   |
| [[Bitcoin/Wallet/Software Wallet/🐦 Sparrow Wallet\|🐦 Sparrow Wallet]]           | ❌ No      | ₿ On-chain  | 🔴 Alta        | ✅✅ Altissima | 🖥️ Tecnica        | CoinJoin, PSBT, multisig, hardware wallet                  | 🐦   |
| [[Bitcoin/Wallet/Hardware Wallet/✍️ SeedSigner\|✍️ SeedSigner]]        | ❌ No      | ₿ Cold      | 🔴 Molto alta  | ✅✅ Estrema   | 📷 Nessuna         | Firma airgapped, QR, seed temporanea                       | 🟧   |
| [[Bitcoin/Wallet/Hardware Wallet/❄️ Coldcard\|❄️ Coldcard]]          | ❌ No      | ₿ Cold      | 🔴 Alta        | ✅✅ Estrema   | 🖲️ Display fisico | Firma offline via PSBT, secure element                     | ❄️   |
| [[Bitcoin/Wallet/Software Wallet/⚡ Electrum\|⚡ Electrum]]          | ❌ No      | ₿ On-chain  | 🔴 Alta        | ✅ Alta       | 🧮 Essenziale      | PSBT, multisig, fee custom, scripting                      | ⚡    |

---

## 📚 Approfondimenti individuali

👉 Per ogni wallet trovi un post dedicato con dettagli, pro, contro, esempi e link:

-  [[Bitcoin/Wallet/Software Wallet/🟠 Wallet of Satoshi\|🟠 Wallet of Satoshi]] – Lightning custodial, semplicissimo  
-  [[Bitcoin/Wallet/Software Wallet/🕊 Phoenix Wallet\|🕊 Phoenix Wallet]] – Lightning non-custodial con canali automatici  
-  [[Bitcoin/Wallet/Software Wallet/🔵 BlueWallet\|🔵 BlueWallet]] – Ibrido, versatile, multi-wallet  
-  [[Bitcoin/Wallet/Software Wallet/🐦 Sparrow Wallet\|🐦 Sparrow Wallet]]– On-chain avanzato, CoinJoin, PSBT  
-  [[Bitcoin/Wallet/Hardware Wallet/✍️ SeedSigner\|✍️ SeedSigner]] – Airgapped, senza memoria, sicurezza estrema  
-  [[Bitcoin/Wallet/Hardware Wallet/❄️ Coldcard\|❄️ Coldcard]] – Hardware wallet solo BTC, firma offline  
-  [[Bitcoin/Wallet/Software Wallet/⚡ Electrum\|⚡ Electrum]] – On-chain desktop, multisig e fee custom  

---

## 🔩 Altri wallet nel giardino

La tabella non esaurisce il giardino. Ecco gli altri wallet che hanno una nota dedicata.

**Hardware wallet**, dal più sovrano al meno:

- [🟡 ColdCard Q](https://ortix.vercel.app/bitcoin/wallet/hardware-wallet/cold-card-q/): Bitcoin-only, airgapped, PSBT via NFC, duress PIN. Costa circa 400€ ed è pensato per somme elevate.
- [🔶 Passport](https://ortix.vercel.app/bitcoin/wallet/hardware-wallet/passport/): Bitcoin-only, airgapped via QR, open source, si usa con l'app Envoy. Costa circa 270€.
- [🟢 Jade](https://ortix.vercel.app/bitcoin/wallet/hardware-wallet/jade/): completamente open source, circa 70€; la versione Plus è airgapped via QR. ⚠️ Il blind oracle dipende dal server Blockstream.
- [🔷 BitBox02](https://ortix.vercel.app/bitcoin/wallet/hardware-wallet/bit-box02/): open source, esiste in versione solo Bitcoin, interfaccia semplice. Non è airgapped (usa USB-C). Costa circa 140€.
- [🔴 Trezor](https://ortix.vercel.app/bitcoin/wallet/hardware-wallet/trezor/): open source ma senza secure element. ⚠️ Senza passphrase è vulnerabile ad attacchi fisici.
- [🔸 KeyStone](https://ortix.vercel.app/bitcoin/wallet/hardware-wallet/key-stone/): airgapped con touchscreen, multisig e Shamir Backup, ma multi-crypto e prodotto in Cina.
- [🟣 Ledger](https://ortix.vercel.app/bitcoin/wallet/hardware-wallet/ledger/): firmware chiuso, data breach del 2020, Ledger Recover. Va bene come primo passo, non come scelta sovrana.
- [🟤 SafePal](https://ortix.vercel.app/bitcoin/wallet/hardware-wallet/safe-pal/): economico (circa 40€), ma legato a Binance e con firmware solo in parte open source. Sconsigliato per somme significative.

**Lightning:**

- [Breez](https://ortix.vercel.app/bitcoin/wallet/software-wallet/breeze/): non custodial, con POS per commercianti e podcasting 2.0. Gestisce l'on-chain solo tramite swap.
- Blixt e Zeus sono i gradini più alti della scala di sovranità descritta in [⚡ Lightning Network](https://ortix.vercel.app/bitcoin/lightning-network/lightning-network/).

**Concetti:** il flusso di firma offline con PSBT è spiegato in [🔒 Airgap Vault](https://ortix.vercel.app/bitcoin/wallet/software-wallet/airgap-vault/).

---

## 📌 Consigli pratici

🛣️ **Percorso di apprendimento, da semplice a complesso:**

1. 🔰 *Prova* con [[Bitcoin/Wallet/Software Wallet/🟠 Wallet of Satoshi\|🟠 Wallet of Satoshi]]  
2. 🧭 Passa a [[Bitcoin/Wallet/Software Wallet/🕊 Phoenix Wallet\|🕊 Phoenix Wallet]] per vera self-custody 
3. 🐦 Impara con [[Bitcoin/Wallet/Software Wallet/🐦 Sparrow Wallet\|🐦 Sparrow Wallet]]
4. ❄️ Custodisci con [[Bitcoin/Wallet/Hardware Wallet/❄️ Coldcard\|❄️ Coldcard]] o [[Bitcoin/Wallet/Hardware Wallet/✍️ SeedSigner\|✍️ SeedSigner]]  
5. ⚡ Automatizza e personalizza con [[Bitcoin/Wallet/Software Wallet/⚡ Electrum\|⚡ Electrum]]

⚠️ Questa scala serve a imparare, non a decidere dove tenere i sats. Wallet of Satoshi è custodial: va bene per provare con pochi sats, mai per conservare valore. Electrum non viene «dopo» il cold storage: è un'alternativa desktop a Sparrow, e tutti e due fanno da coordinatore per un Coldcard o un SeedSigner.

🔺 Per distribuire i fondi usa la piramide: il patrimonio sta in un cold wallet, il medio termine in un hot wallet, le spese quotidiane su Lightning. La trovi in [📊 Come scegliere il wallet giusto - Flow Chart](https://ortix.vercel.app/bitcoin/guide-e-consigli/come-scegliere-il-wallet-giusto-flow-chart/), con il ragionamento completo in [Gestire i Bitcoin in modo intelligente](https://ortix.vercel.app/bitcoin/guide-e-consigli/gestire-i-bitcoin-in-modo-intelligente/).

🧱 Costruisci la tua sicurezza un wallet alla volta: prima le chiavi, poi la comodità. Il principio di fondo è in [🔐 Self-custody](https://ortix.vercel.app/bitcoin/definizioni/blockchain/self-custody/).

---
