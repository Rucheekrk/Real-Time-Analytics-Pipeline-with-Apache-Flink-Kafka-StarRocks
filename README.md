# 🚀 Real-Time Analytics Pipeline using Apache Flink, Kafka & StarRocks

A fully containerized, real-time data analytics pipeline for clickstream processing. Built with **Apache Flink**, **StarRocks**, **Kafka**, **MySQL**, **Debezium**, **dbt**, and **Docker Compose**.

---

## 📊 Architecture

![Architecture Diagram](./assets/data_pipeline_diagram.png)

**Components:**
- 🐍 **Python Kafka Producer** – Simulates ~10K events/min
- 🛸 **Apache Kafka** – Event streaming backbone
- 🔁 **Apache Flink** – Stream processing with tumbling windows + custom aggregations
- 🐘 **MySQL** – Historical data storage
- 🔁 **Debezium** – Change data capture (CDC) from MySQL into Kafka
- 💎 **StarRocks** – Low-latency OLAP database
- 📦 **dbt** – SQL modeling into star schema

---

## 🧰 Tech Stack

| Layer              | Tools                                  |
|-------------------|----------------------------------------|
| Ingestion          | Python, Kafka, Debezium                |
| Processing         | Apache Flink (v1.17)                   |
| Storage            | StarRocks, MySQL                       |
| Transformation     | dbt (Data Build Tool)                  |
| Orchestration      | Docker, Docker Compose                 |
| Language/Querying  | Python, SQL                            |

---

## ✨ Features

- ⚡ Simulates ~10K clickstream events per minute
- ⏱ Real-time stream processing with <2s end-to-end latency
- 🔄 MySQL CDC via Debezium for historical enrichment
- 💾 StarRocks for fast analytical querying of processed streams
- 🔧 Star schema design with dbt (↓ query complexity by 40%)
- 📦 Fully containerized with Docker Compose

---

## 📂 Directory Structure

