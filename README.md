# 🕹️ Real-Time Ubisoft Game Updates Pub-Sub System

This project is a real-time **Publish-Subscribe (Pub-Sub)** system designed for streaming live **Ubisoft game updates** using **Kafka**, **Python**, **Docker**, and a revamped event-driven architecture. The system supports **low-latency**, **high-throughput**, and **scalable** messaging optimized for **distributed architectures**.

---

## 🚀 Features

- ✅ Real-time event publishing and consumption using **Apache Kafka**
- 🐍 Built with **Python** and **Flask** for streamlined API interaction
- 🐳 **Dockerized** environment for easy deployment and isolation
- 💾 **MySQL** backend for robust subscriber management
- 🔀 **Rendezvous-based routing** for efficient message delivery
- ⚡ Event-driven design for improved scalability and fault tolerance

---

## 🧱 Architecture

 ┌──────────┐       ┌──────────────┐       ┌──────────────┐
 │ Producer │──────▶│   Kafka Bus  │──────▶│  Subscriber  │
 └──────────┘       └──────────────┘       └──────────────┘
                       ▲          ▲
              ┌────────┘          └───────┐
              │       Flask API           │
              └────▶ MySQL DB ◀───────────┘




---

## 🛠️ Tech Stack

| Technology     | Purpose                                      |
|----------------|----------------------------------------------|
| **Python**     | Core business logic and Kafka interaction   |
| **Apache Kafka** | Distributed event streaming               |
| **Flask**      | REST API for managing subscribers            |
| **MySQL**      | Persistent storage for subscriber data       |
| **Docker**     | Containerization of the entire ecosystem     |

---

## 📂 Project Structure

ubisoft-pubsub/
├── producer/             # Game event producers
├── consumer/             # Game update subscribers
├── api/                  # Flask API for subscription management
├── db/                   # MySQL schema and init files
├── docker-compose.yml    # Multi-service Docker config
├── requirements.txt
