# FinLedger
Personal finance management platform built with Java, Spring Boot, and microservices


                    ┌─────────────────┐
                    │   API Gateway   │
                    └────────┬────────┘
                             │
             ┌───────────────┼───────────────┐
             ↓               ↓               ↓
       User Service     Expense Service   Budget Service
             │               │               │
             └───────────────┼───────────────┘
                             ↓
                           Kafka
                             │
                    ┌────────┴────────┐
                    ↓                 ↓
             Notification       Analytics
                Service           Service
                    │                 │
                  Redis          PostgreSQL
