---
{"dg-publish":true,"permalink":"/ortix/storage/backup-sovrano-con-3-dispositivi-e-syncthing/","title":"🛡️ Backup sovrano con 3 dispositivi e Syncthing","tags":["Backup","SovranitàDigitale","Syncthing","ReteMesh","SelfHosting","Sicurezza","Offline"],"dg-note-properties":{"title":"🛡️ Backup sovrano con 3 dispositivi e Syncthing","tags":["Backup","SovranitàDigitale","Syncthing","ReteMesh","SelfHosting","Sicurezza","Offline"],"date":"2025-07-10"}}
---


# 🛡️ **Backup sovrano con 3 dispositivi e Syncthing**

Non fidarti del cloud.  
Non fidarti dei backup su servizi centralizzati.  
👁️‍🗨️ Qualsiasi piattaforma può chiudere, censurarti o perdere i tuoi dati.

La soluzione?  
📡 Un backup **autonomo e replicato** con 3 dispositivi e [[Ortix/Storage/🔄 Syncthing\|🔄 Syncthing]] in **[[rete mesh\|rete mesh]]**.

---

## 🔧 Come funziona?

📲 Puoi usare **3 telefoni Android**, anche vecchi, per creare un backup robusto:  
- 1 telefono **principale** (quello che usi ogni giorno)  
- 2 telefoni **di riserva** (anche vecchi, inutilizzati, offline finché vuoi)

✅ I dati si sincronizzano **localmente** tra i dispositivi,  
senza bisogno di **cloud** né **internet**,  
**basta che siano connessi alla stessa rete Wi-Fi** 📶

📂 Ogni nodo mantiene una **copia aggiornata dei tuoi dati**,  
che siano file, note Obsidian, chiavi GPG, password KeePass o documenti importanti.

---

## 🎒 Espandi lo spazio facilmente

📦 Se i dispositivi hanno poco spazio interno,  
puoi espandere la memoria con una **microSD economica** da 64/128/256 GB.

💡 Questo ti permette di:

- 📚 Avere una **biblioteca personale di eBook (ePub)** offline  
- 🎧 Ascoltare **musica archiviata localmente**, senza abbonamenti  
- 🖼️ Conservare **foto e video personali** in locale, senza cloud  
- 🛠️ Tenere una **copia dei tuoi backup e dei tuoi file sensibili**  
> ⚠️ Il **limite è solo lo spazio disponibile**, non ci sono vincoli di piattaforma o abbonamento

---

## 📡 Come configurare la rete mesh

1. **Installa Syncthing** su tutti e 3 i telefoni  
   Ti consiglio [F-Droid](https://f-droid.org/en/packages/com.github.catfriend1.syncthingandroid/) per una versione open senza traccianti

2. **Configura le cartelle condivise**  
   Es. una cartella "Vault" con le tue note o backup

3. **Connetti i dispositivi tra loro**  
   Ogni nodo va collegato agli altri due → si forma una **rete mesh**

4. **Accendi i dispositivi periodicamente (almeno due alla volta)**  
   Finché sono sulla stessa Wi-Fi, Syncthing sincronizza i dati in automatico

---

## 🧱 Perché è solido?

🔁 **3 copie ridondanti**  
Se un dispositivo si rompe o viene perso, i dati sono al sicuro sugli altri due.

📡 **Funziona su rete Wi-Fi privata**  
Non serve connessione internet, **ma solo il Wi-Fi locale attivo**

🔒 **Nessun cloud, zero fiducia esterna**  
I tuoi dati **non lasciano mai i tuoi dispositivi**

💸 **Zero abbonamenti**  
Tutto gratuito e open source. Paghi solo una tantum per i telefoni (e, se serve, microSD)

---

## 💰 Costi stimati

| Voce                   | Costo         |
|------------------------|---------------|
| Telefono principale    | già in uso    |
| Telefono vecchio #1    | 0–30€ usato   |
| Telefono vecchio #2    | 0–30€ usato   |
| microSD (opzionale)    | 8–25€ cad.    |
| Totale                 | **0–85€** max |

💡 Telefoni vecchi con schermo rotto o batteria degradata vanno benissimo:  
**serve solo Wi-Fi funzionante e un po’ di spazio (interno o su microSD).**

---

## ✅ Alternativa più robusta

🖥️ Sostituisci uno dei dispositivi con un [[Raspberry Pi\|Raspberry Pi]]  
→ piccolo server casalingo, acceso sempre, con backup automatico.

---

## 🔗 Post correlati

- [[Ortix/Storage/🔄 Syncthing\|🔄 Syncthing]]  
- [[Ortix/Filosofia/🛡️ Sovranità digitale\|🛡️ Sovranità digitale]]

---

📦 Se **il dato è importante**, deve vivere **in più luoghi**, sotto il tuo **esclusivo controllo**.  
Con 3 dispositivi, anche vecchi, puoi creare una **cassaforte digitale decentralizzata**, tutta tua.

#Backup #Syncthing #Obsidian #SovranitàDigitale #Bitcoin
{ #tr-ky99vfz0p}
