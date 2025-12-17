---
{"dg-publish":true,"permalink":"/bitcoin/wallet/wallet-gerarchico/","title":"🌳 Wallet gerarchico con BIP85: una sola radice, infiniti rami","tags":["Wallet","BIP85","SelfCustody","Sicurezza","Seed","ColdStorage"]}
---


# 🌳 Wallet gerarchico con BIP85: una sola radice, infiniti rami

🧠 **Immagina di avere una sola chiave principale…  
e da lì generare decine di wallet diversi, isolati, sicuri.**  
Benvenuto nel mondo di **BIP85**, lo standard per creare wallet **gerarchici deterministici indipendenti**.

Una sola seed → infiniti semi secondari.  
Come un albero: 🌱 una radice, mille rami.

---

🔐 **Cos’è BIP85?**

- Uno standard Bitcoin che consente di **derivare altre seed BIP39, password, chiavi per app o account**,  
  **da una seed principale**, in modo deterministico  
- Non serve inventarsi nuove parole o scriverle ovunque  
- Ogni derivazione è **indipendente** e **ripetibile**, ma solo se conosci **la root**

---

🧰 **A cosa serve nella pratica?**

- Creare wallet diversi per scopi diversi (es. hot wallet, cold wallet, figli, backup)  
- Isolare i fondi tra più livelli o utenti  
- Evitare di scrivere mille seed diverse  
- Mantenere **una singola copia cartacea/offline**  
- Automazione avanzata per progetti self-hosted

📦 Perfetto per chi vuole **ordine e sicurezza senza compromessi**.

---

🛠️ **Esempio pratico**

1. Generi una seed principale da 12 o 24 parole  
2. La importi in un software compatibile con BIP85 (es. [SeedSigner](https://seedsigner.com), [Specter DIY](https://specter.solutions), [Keystone], Trezor fw alternativo, ecc.)  
3. Derivi:  
   - Seed per figlio n.1 → `BIP85 Derivation 0`  
   - Seed per wallet emergenza → `BIP85 Derivation 5`  
   - Seed per password manager → `BIP85 Derivation 10`

🎯 Ogni derivazione è **un nuovo wallet completo, isolato**, ma ricostruibile se hai la master key.

---

⚠️ **Attenzione: potere = responsabilità**

🧨 Chi ha la seed master… ha accesso a tutto.  
Per questo va **protetta con cura assoluta**, meglio in [[Bitcoin/Cold Wallet\|Cold Wallet]], su carta, acciaio, o meglio ancora con [[Bitcoin/Wallet/🔐 Multisig\|🔐 Multisig]].

---

📱 **Wallet compatibili con BIP85 (parziale)**

| Wallet/App       | Supporto BIP85 | Note                              |
|------------------|----------------|-----------------------------------|
| SeedSigner       | ✅ Sì          | Cold wallet DIY, open source     |
| Specter DIY      | ✅ Sì          | Hardware wallet open source      |
| Keystone (fw btc)| ✅ Sì          | Dopo aggiornamento firmware      |
| Trezor (con mod) | ⚠️ Parziale   | Solo con firmware alternativo    |
| Electrum         | ❌ No diretto  | Ma puoi importare manualmente    |

---

🔥 **Conclusione**

🌳 BIP85 è come **avere un albero della sovranità digitale personale**.  
Puoi generare wallet per i tuoi figli, amici, progetti —  
senza mai uscire dal tuo schema mentale, senza perdere il controllo.

🧠 Una seed per domarli tutti.  
**Ma solo tu devi conoscerla.**

---

🔗 _Approfondisci con [[Bitcoin/Wallet/🧠 Seed Phrase\|Bitcoin/Wallet/🧠 Seed Phrase]], [[Bitcoin/Cold Wallet\|Cold Wallet]], [[Bitcoin/Wallet/🔐 Multisig\|🔐 Multisig]], [[Bitcoin/Wallet/🪨 Steelwallet\|Bitcoin/Wallet/🪨 Steelwallet]], [[Bitcoin/Wallet/🧭 Wallet Index\|🧭 Wallet Index]], [[Bitcoin/Wallet/🔐 Self-custody\|🔐 Self-custody]]_