---
{"dg-publish":true,"permalink":"/bitcoin/definizioni/blockchain/xpub/","title":"🔗 Cos’è l’XPUB – Il cuore dei wallet watch-only","tags":["bitcoin","xpub","wallet","self-custody","airgap","educazione"],"dg-note-properties":{"title":"🔗 Cos’è l’XPUB – Il cuore dei wallet watch-only","description":"Spiegazione chiara e approfondita dell’XPUB in Bitcoin: cos’è, a cosa serve e perché è centrale per i wallet watch-only.","tags":["bitcoin","xpub","wallet","self-custody","airgap","educazione"],"date":"2025-12-16","author":"Alan Bimbati"}}
---


# 🔗 Cos’è l’XPUB – Il cuore dei wallet watch-only

Quando parliamo di Bitcoin e di wallet, spesso sentiamo sigle misteriose come **XPUB**.  
Non è magia, né un codice segreto: è **il meccanismo che permette di osservare i fondi senza possederli**.

---

## 🧠 XPUB – Extended Public Key

**XPUB** sta per *Extended Public Key*, ovvero “chiave pubblica estesa”.

- È **una chiave pubblica speciale** che può generare tutti gli indirizzi di un wallet derivato da una seed.
- Non permette di **spendere** i fondi: può solo **vedere saldo e ricevere pagamenti**.
- Funziona come un **master key pubblica**, utile per wallet watch-only.

---

## 📱 Perché serve nei wallet watch-only

Un wallet watch-only è un wallet che:

- **mostra il saldo**
- **prepara transazioni**
- **non può firmare nulla**

XPUB permette di:

1. collegare il wallet **offline** (custodia) con il wallet **online** (uso)
2. creare tutti gli indirizzi derivati senza mai esporre la seed
3. ricevere pagamenti in sicurezza
4. verificare transazioni in modo trasparente

> Con XPUB, la privacy e la sicurezza restano intatte: chiunque lo possieda **non può rubare i tuoi bitcoin**.

---

## 🔄 Come funziona in pratica

1. Wallet offline (Airgap, hardware wallet):
   - genera XPUB
   - conserva le chiavi private offline
2. Wallet online (BlueWallet, Electrum):
   - importa XPUB
   - mostra saldo e transazioni
   - prepara transazioni da firmare offline

👉 Il flusso di firma resta **[[Bitcoin/Definizioni/Blockchain/air-gapped\|air-gapped]]**: mai esposizione delle chiavi private.

---

## 💡 Uso consapevole dell’XPUB

- Condividere XPUB con cautela: chiunque può **vedere il saldo e gli indirizzi generati**, quindi potenzialmente **tracciare le tue transazioni**.
- Non è pericoloso come la chiave privata, ma può ridurre **la privacy** se esposto pubblicamente.
- Ottimo per **contabilità, monitoraggio e audit**, senza rischio di furto.

---

## 🧩 XPUB vs PrivKey

| XPUB | Chiave Privata |
|------|----------------|
| Pubblica | Segreta |
| Permette solo di **vedere saldo e generare indirizzi** | Permette di **spendere i bitcoin** |
| Sicura da condividere con attenzione | Mai condividere |
| Utile per **watch-only** e bookkeeping | Necessaria per firmare transazioni |

---

## 🎯 Messaggio chiave

> L’XPUB è la chiave della **trasparenza senza rischio**.  
> Ti permette di **vedere e organizzare** i tuoi fondi senza mai esporli.

In un percorso di self-custody, capire l’XPUB è un passo fondamentale verso **autonomia, sicurezza e consapevolezza**.

---
