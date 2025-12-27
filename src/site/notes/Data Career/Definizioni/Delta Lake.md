---
{"dg-publish":true,"permalink":"/data-career/definizioni/delta-lake/","title":"Cos'è Delta Lake","tags":["DeltaLake","DataEngineering","ACID","BigData","Architettura"]}
---


# 🔺 Cos'è Delta Lake

🛡️ **Affidabilità sul Data Lake**

I [[Data Career/Definizioni/Data Lake\|Data Lake]] tradizionali hanno un problema: se un processo di scrittura fallisce a metà, i dati restano corrotti. Inoltre, modificare un file è difficile.
**Delta Lake** risolve questi problemi portando le caratteristiche dei database relazionali (affidabilità) sullo storage economico del Data Lake.

---

## 🚀 Funzionalità Chiave

1. **Transazioni ACID**: Garantisce che le operazioni siano "tutto o niente". Niente dati parziali o corrotti.
2. **Time Travel**: Puoi interrogare i dati "come erano ieri". Utile per audit e rollback.
3. **Schema Enforcement**: Impedisce di scrivere dati che non rispettano la struttura prevista (evita la "Data Swamp").
4. **Unified Batch & Streaming**: Una sola tabella può ricevere dati sia da flussi continui che da caricamenti batch.

---

## 🏗️ Architettura Medallion

Delta Lake abilita la famosa architettura a medaglione:
- 🥉 **Bronze**: Dati grezzi (Raw), ingestione diretta.
- 🥈 **Silver**: Dati puliti, filtrati, arricchiti.
- 🥇 **Gold**: Dati aggregati, pronti per il business ([[Data Career/Definizioni/Data warehouse\|Data warehouse]] level).

---

## 🎯 Obiettivo

Avere la **flessibilità** del Data Lake con l'**affidabilità** del Data Warehouse. (Il concetto di **Lakehouse**).

#DeltaLake #DataEngineering #ACID #Lakehouse #Architettura
