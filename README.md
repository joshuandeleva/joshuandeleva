<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=26&duration=2500&pause=700&color=36BCF7&center=true&vCenter=true&width=1000&lines=Joshua+Ndeleva;Full-Stack+Engineer;Distributed+Systems+%7C+Architecture+%7C+Microservices;Go+%7C+NestJS+%7C+Kafka+%7C+React+Native;DevOps+%7C+Observability+%7C+Scalability" />

</div>

---

# 👋 About Me

I’m a **full-stack engineer** experienced in designing and building **distributed systems**, **event-driven architectures**, and **scalable platforms**.

I’ve worked across the full evolution of systems — from **monolithic applications** to **modular architectures** and **event-driven microservices** — while delivering **web and mobile applications** using React and React Native (Expo).

My focus is on **architecture, reliability, observability, and long-term scalability**.

---

## 🧠 Core Engineering Focus

- System & Software Architecture  
- Distributed Systems & Event Streaming  
- Monolith → Modular → Microservices  
- Scalability, Performance & Reliability  
- DevOps & Platform Engineering  
- Web & Mobile Frontend Development  

---

## 🛠️ Tech Stack

### Cloud Platforms
- AWS (EC2, S3, Lambda, RDS, DynamoDB, ECS, EKS, SQS, SNS)

### Backend & Core Systems
- Go, NestJS, Node.js, TypeScript

### Messaging & Streaming
- Apache Kafka, RabbitMQ

### Frontend & Mobile
- React, React Native, Expo, Next.js

### DevOps & Infrastructure
- Docker, GitHub Actions, Linux

### Databases
- PostgreSQL, MongoDB

---

## 🏛️ Architecture Evolution

### 🧱 Monolithic Architecture

```mermaid
flowchart TB
    UI[Web / Mobile UI]
    API[Monolithic Backend]
    DB[(Single Database)]

    UI --> API
    API --> DB
```

Characteristics

Simple deployment

Fast initial development

Shared database & tight coupling

🔄 Modular Monolith

```mermaid
flowchart TB
    API[Monolith]
    Auth[Auth Module]
    Orders[Orders Module]
    Payments[Payments Module]

    API --> Auth
    API --> Orders
    API --> Payments
```

Characteristics

Clear domain boundaries

Internal module separation

Easier migration to services

🌐 Event-Driven Microservices

```mermaid
flowchart TB
    FE[React / React Native]
    GW[API Gateway]

    FE --> GW

    GW --> AuthS[Auth Service]
    GW --> OrderS[Order Service]
    GW --> PaymentS[Payment Service]

    OrderS --> Kafka[(Kafka)]
    PaymentS --> Kafka

    Kafka --> NotifyS[Notification Service]
    Kafka --> AnalyticsS[Analytics Service]

    NotifyS --> RabbitMQ[(RabbitMQ)]
```

Design Choices

Kafka for domain events & streaming

RabbitMQ for background jobs

Independent service scaling

Fault isolation & resilience

📱 Mobile Architecture (React Native + Expo)

```mermaid
flowchart TB
    RN[React Native App]
    Expo[Expo Runtime]
    API[Backend APIs]

    RN --> Expo
    RN --> API
```

Cross-platform iOS & Android

Shared business logic

OTA updates & fast iteration

🔍 Observability & Monitoring

Observability Principles

Observability is treated as a first-class concern across all services.

Metrics → What is happening?

Logs → Why did it happen?

Traces → Where did it happen?

🧰 Observability Stack

Prometheus — metrics & alerting

Grafana — dashboards & visualization

OpenTelemetry — distributed tracing

Structured, correlated logging

📈 Metrics Architecture

```mermaid
flowchart TB
    S1[Service A]
    S2[Service B]
    Prom[Prometheus]
    Graf[Grafana]

    S1 --> Prom
    S2 --> Prom
    Prom --> Graf
```

Key Metrics

Request latency & error rates

Kafka consumer lag

RabbitMQ queue depth

CPU / memory usage

Business KPIs

🧭 Distributed Tracing

```mermaid
sequenceDiagram
    participant FE as Frontend
    participant GW as API Gateway
    participant OS as Order Service
    participant PS as Payment Service

    FE->>GW: HTTP Request
    GW->>OS: Forward (trace context)
    OS->>PS: Async call
```

End-to-end request visibility

Context propagation across services

Bottleneck & latency detection

📜 Logging Strategy

```mermaid
flowchart TB
    Service[Microservice]
    Logs[Structured Logs]
    Viewer[Grafana / Log UI]

    Service --> Logs
    Logs --> Viewer
```

JSON structured logs

Trace & request ID correlation

Environment-aware verbosity

🚨 Reliability & Operations

SLO & SLA-driven alerts

Error budget awareness

Low-noise alerting

Proactive incident detection

📊 GitHub Stats
<p align="center"> <img src="https://github-readme-stats.vercel.app/api?username=joshuandeleva&show_icons=true&theme=tokyonight" height="165"/> <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=joshuandeleva&layout=compact&theme=tokyonight" height="165"/> </p>
🤝 Let’s Connect
GitHub: https://github.com/joshuandeleva

Open to backend, distributed systems & platform engineering discussions
