---
{"dg-publish":true,"permalink":"/data-career/definizioni/data-warehouse/","title":"🏢 Cos'è un Data Warehouse: l'archivio centrale dei dati","tags":["DataEngineering","DataWarehouse","Dati","ETL","Analisi","Metafora"],"dg-note-properties":{"title":"🏢 Cos'è un Data Warehouse: l'archivio centrale dei dati","tags":["DataEngineering","DataWarehouse","Dati","ETL","Analisi","Metafora"],"aliases":["Data Warehouse","Data warehouse"],"date":"2025-07-15"}}
---


# 🏢 **Cos'è un Data Warehouse: l'archivio centrale dei dati**

📦 Un **Data Warehouse** è un **magazzino digitale centralizzato** dove finiscono tutti i dati puliti, ordinati e pronti all’uso.  

💡 È come un **archivio cartaceo** ben etichettato: ogni documento ha il suo posto, ogni scaffale è ordinato per categoria, e chi ci entra può trovare esattamente ciò che cerca, velocemente.

---

## 🔄 Come ci finiscono i dati?

📍 Con una pipeline [[Data Career/Definizioni/ETL\|ETL]] (Extract – Transform – Load) o **ELT**:

1. **Extract**: prendo i dati da più fonti (siti, database, app...)
2. **Transform**: li pulisco, li rendo coerenti, li strutturo
3. **Load**: li carico nel **Data Warehouse**, pronti per analisi 📊

---

## 🧠 A cosa serve un Data Warehouse?

- 📊 **Report e dashboard** per il business
- 🧪 **Analisi storica dei dati**
- 🔁 **Tracciabilità delle decisioni**
- 🧮 **Query veloci** anche su milioni di righe
- 🔐 **Controllo centralizzato e versionato** dei dati

---

## 🧰 Esempi di Data Warehouse

| Nome             | Tipo          | Note principali                    |
|------------------|---------------|------------------------------------|
| Amazon Redshift  | Cloud         | Scalabile, integrato con AWS       |
| Google BigQuery  | Cloud         | Query SQL su enormi dataset        |
| Snowflake        | Cloud-native  | Multi-cloud, performante           |
| PostgreSQL DW    | Locale        | Per piccoli progetti o test locali |

---

## 🚿 Metafora: il centro di smistamento dei pacchi 📦

Immagina che ogni dato sia un pacco che arriva da mittenti diversi: e-commerce, logistica, clienti, app...  

🎯 Il **Data Warehouse è come il magazzino Amazon centrale**:  
- i pacchi vengono **confezionati e etichettati**
- messi negli **scaffali giusti**  
- pronti per essere cercati e consegnati a chi ne ha bisogno  

👨‍💼 I manager, data analyst o sviluppatori sono i corrieri: trovano il pacco giusto (dato giusto), lo leggono, e agiscono di conseguenza.

---

## 🚫 Quando NON va usato

❌ Se i dati cambiano di continuo (real-time → meglio i [[Data Career/Definizioni/Data Lake\|Data Lake]] o i database [[Data Career/Definizioni/OLTP\|OLTP]])  
❌ Se hai poca quantità di dati (usa un database classico)  
❌ Se vuoi risparmiare: i Data Warehouse sono **costosi se mal progettati**

---

## ✅ Quando serve DAVVERO

✔️ Se hai più fonti di dati  
✔️ Se vuoi fare **analisi, BI o report su anni di storia**  
✔️ Se ti serve **velocità e struttura** nel reperire le informazioni  


#DataWarehouse #Dati #ETL #Analisi #Architettura #Metafora