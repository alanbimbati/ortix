---
{"dg-publish":true,"permalink":"/data-career/definizioni/data-lake/","title":"Cos'è un Data Lake","tags":["DataLake","BigData","Storage","Architettura","Definizioni"],"dg-note-properties":{"title":"Cos'è un Data Lake","tags":["DataLake","BigData","Storage","Architettura","Definizioni"],"date":"2025-08-01","summary":"Un Data Lake è un repository centralizzato che permette di archiviare tutti i dati strutturati e non strutturati su qualsiasi scala. I dati vengono salvati nel formato grezzo originale."}}
---


# 🌊 Cos'è un Data Lake

📥 **Il bacino di raccolta universale**

A differenza del [[Data Career/Definizioni/Data warehouse\|Data warehouse]] (che è come un magazzino ordinato), il **Data Lake** è come un lago naturale: ci confluiscono fiumi di dati da ogni fonte, nel loro stato originale.

---

## ⚙️ Caratteristiche

- **Schema-on-Read**: Non devi definire la struttura *prima* di salvare i dati (come nel DB classico). La definisci quando li *leggi*.
- **Flessibilità**: Accetta tutto (JSON, CSV, Immagini, Log, Video).
- **Costo**: Generalmente economico (basato su Object Storage come S3 o Azure Blob).

---

## 🆚 Data Lake vs Data Warehouse

| Caratteristica | Data Lake 🌊 | Data Warehouse 🏢 |
| :--- | :--- | :--- |
| **Dati** | Grezzi, non strutturati | Puliti, strutturati |
| **Utenti** | Data Scientists, Engineers | Business Analysts |
| **Schema** | On-Read (flessibile) | On-Write (rigido) |
| **Agilità** | Alta | Bassa |

---

## ⚠️ Il Rischio "Data Swamp"

Se butti tutto nel lago senza catalogarlo, diventa una palude.
Per questo serve:
- **[[Data Career/Definizioni/Data Governance\|Data Governance]]**
- **[[Data Career/Tips/🗂️ Metadati e Data Lineage\|🗂️ Metadati e Data Lineage]]**
- Strati di affidabilità come **[[Data Career/Definizioni/Delta Lake\|Delta Lake]]**

---

## 🎯 Obiettivo

Avere un posto unico dove atterrano *tutti* i dati aziendali, pronti per essere esplorati o trasformati successivamente.

#DataLake #BigData #Storage #Architettura #Definizioni
