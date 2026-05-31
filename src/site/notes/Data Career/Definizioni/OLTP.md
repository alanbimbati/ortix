---
{"dg-publish":true,"permalink":"/data-career/definizioni/oltp/","title":"OLTP vs OLAP","tags":["OLTP","OLAP","Database","Architettura","Definizioni"],"dg-note-properties":{"title":"OLTP vs OLAP","tags":["OLTP","OLAP","Database","Architettura","Definizioni"],"date":"2025-08-01","summary":"Differenza tra sistemi transazionali (OLTP) progettati per l'operatività quotidiana e sistemi analitici (OLAP) progettati per l'analisi dei dati e il reporting."}}
---


# ⚡ OLTP vs OLAP: Due modi di usare i dati

Nel mondo dei database, esistono due grandi famiglie di sistemi, ottimizzati per scopi opposti.

---

## 🛒 OLTP (Online Transaction Processing)

**"Il sistema operativo"**
È il database che fa funzionare l'applicazione.

- **Scopo**: Gestire transazioni quotidiane veloci (Insert, Update, Delete).
- **Esempio**: Quando paghi alla cassa, il sistema registra la vendita, scala l'inventario e aggiorna il saldo.
- **Caratteristiche**:
  - Molte piccole transazioni concorrenti.
  - Dati normalizzati (per evitare ridondanze).
  - Integrità dei dati critica.
  - **Database tipici**: PostgreSQL, MySQL, Oracle.

---

## 📊 OLAP (Online Analytical Processing)

**"Il sistema decisionale"**
È il database per analizzare i dati ([[Data Career/Definizioni/Data warehouse\|Data warehouse]]).

- **Scopo**: Rispondere a domande complesse su grandi volumi di dati storici.
- **Esempio**: "Qual è stato il prodotto più venduto in Lombardia negli ultimi 5 anni?"
- **Caratteristiche**:
  - Poche query, ma molto pesanti (lettura di milioni di righe).
  - Dati denormalizzati (schema a stella/fiocco di neve) per velocità di lettura.
  - Aggiornamenti batch (es. notturni via [[Data Career/Definizioni/ETL\|ETL]]).
  - **Database tipici**: Snowflake, BigQuery, Redshift, ClickHouse.

---

## 🆚 Il Confronto

| | OLTP 🛒 | OLAP 📊 |
| :--- | :--- | :--- |
| **Focus** | Operatività (Scrittura) | Analisi (Lettura) |
| **Dati** | Correnti, dettagliati | Storici, aggregati |
| **Utenti** | Applicazioni, Clienti | [[Data Career/Job definition/Data Analyst\|Data Analyst]], Manager |
| **Velocità** | Millisecondi | Secondi/Minuti |

---

## 🎯 Obiettivo

Non usare un OLTP per fare analisi (bloccheresti l'app!).
Non usare un OLAP per gestire le transazioni (sarebbe troppo lento!).
Usa l'[[Data Career/Definizioni/ETL\|ETL]] per spostare i dati da OLTP a OLAP.

#OLTP #OLAP #Database #Architettura #Definizioni
