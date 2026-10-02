# DAT TRAN / J.ANDY

> **Software Engineer — mostly .NET, sometimes React, always curious.**

I like building things that are **fast, understandable, and hard to break**.

I work mostly on backend-heavy products: APIs, databases, background jobs, integrations, distributed services, and the occasional frontend when it needs to be done properly.

[![Portfolio](https://img.shields.io/badge/PORTFOLIO-070707?style=for-the-badge&logo=vercel&logoColor=D7FF3F)](https://jayandy.id.vn)
[![GitHub](https://img.shields.io/badge/GITHUB-070707?style=for-the-badge&logo=github&logoColor=D7FF3F)](https://github.com/trandat1114)
[![LinkedIn](https://img.shields.io/badge/LINKEDIN-070707?style=for-the-badge&logo=linkedin&logoColor=D7FF3F)](https://www.linkedin.com/in/tran-phu-dat-526a82288/)

---

## 01 — WHAT I LIKE BUILDING

~~~text
something users touch
        ↓
      API
        ↓
    business logic
        ↓
  data + messaging
        ↓
 background work
        ↓
 "okay, but why is it slow?"
        ↓
 measure → fix → ship
~~~

I enjoy the messy middle of software:

- APIs that have to survive real traffic
- SQL that starts simple and becomes very interesting
- Background jobs and scheduled workflows
- Services talking to other services
- Integrations that were "just a small requirement"
- Finding out why something is slow instead of guessing
- Making production problems easier to see and explain

> **I care about the part after "it works."**

---

## 02 — THE STACK

### Backend

![C#](https://img.shields.io/badge/C%23-070707?style=flat-square&logo=csharp&logoColor=D7FF3F)
![.NET](https://img.shields.io/badge/.NET_10-070707?style=flat-square&logo=dotnet&logoColor=D7FF3F)
![ASP.NET Core](https://img.shields.io/badge/ASP.NET_Core-070707?style=flat-square&logo=dotnet&logoColor=D7FF3F)
![EF Core](https://img.shields.io/badge/EF_Core-070707?style=flat-square&logo=dotnet&logoColor=D7FF3F)
![Dapper](https://img.shields.io/badge/Dapper-070707?style=flat-square&logoColor=D7FF3F)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-070707?style=flat-square&logo=rabbitmq&logoColor=D7FF3F)

**Minimal APIs · REST · CQRS · Event-driven systems · Background processing · Microservices**

### Frontend

![React](https://img.shields.io/badge/React-070707?style=flat-square&logo=react&logoColor=D7FF3F)
![Next.js](https://img.shields.io/badge/Next.js-070707?style=flat-square&logo=nextdotjs&logoColor=D7FF3F)
![TypeScript](https://img.shields.io/badge/TypeScript-070707?style=flat-square&logo=typescript&logoColor=D7FF3F)
![Tailwind](https://img.shields.io/badge/Tailwind-070707?style=flat-square&logo=tailwindcss&logoColor=D7FF3F)

**React · Next.js · TypeScript · Redux · Responsive UI · UX**

### Data

![SQL Server](https://img.shields.io/badge/SQL_Server-070707?style=flat-square&logo=microsoftsqlserver&logoColor=D7FF3F)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-070707?style=flat-square&logo=postgresql&logoColor=D7FF3F)
![Redis](https://img.shields.io/badge/Redis-070707?style=flat-square&logo=redis&logoColor=D7FF3F)

**Query optimization · Indexing · Execution plans · Stored procedures · Caching · Data access**

### Delivery & Observability

![Docker](https://img.shields.io/badge/Docker-070707?style=flat-square&logo=docker&logoColor=D7FF3F)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-070707?style=flat-square&logo=githubactions&logoColor=D7FF3F)
![Azure](https://img.shields.io/badge/Azure-070707?style=flat-square&logo=microsoftazure&logoColor=D7FF3F)
![Linux](https://img.shields.io/badge/Linux-070707?style=flat-square&logo=linux&logoColor=D7FF3F)
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-070707?style=flat-square&logo=opentelemetry&logoColor=D7FF3F)
![Prometheus](https://img.shields.io/badge/Prometheus-070707?style=flat-square&logo=prometheus&logoColor=D7FF3F)
![Grafana](https://img.shields.io/badge/Grafana-070707?style=flat-square&logo=grafana&logoColor=D7FF3F)
![Sentry](https://img.shields.io/badge/Sentry-070707?style=flat-square&logo=sentry&logoColor=D7FF3F)

---

## 03 — HOW I THINK ABOUT A SYSTEM

~~~text
        ┌──────────────────────────┐
        │       React / Next       │
        └────────────┬─────────────┘
                     │
                     ▼
        ┌──────────────────────────┐
        │      ASP.NET Core        │
        │       API / Domain       │
        └─────┬──────────┬─────────┘
              │          │
              ▼          ▼
        ┌──────────┐  ┌──────────┐
        │ SQL / EF │  │ RabbitMQ │
        │  Dapper  │  │  Redis   │
        └────┬─────┘  └────┬─────┘
             │             │
             └──────┬──────┘
                    ▼
            ┌───────────────┐
            │ Workers / Jobs│
            └───────┬───────┘
                    │
                    ▼
          ┌───────────────────┐
          │   Observability   │
          │ OTel · Metrics    │
          │ Logs · Traces     │
          └───────────────────┘
~~~

The tools change. The questions don't:

**Where does the work happen? Where does it fail? Where does it slow down? Can we see it? Can we change it safely?**

---

## 04 — SELECTED WORK

### [.NET Universe](https://github.com/trandat1114/DotnetuniverseProject)

Graduation project exploring search, validation, filtering, pagination, and application structure.

### [Kafka Demo](https://github.com/trandat1114/KafkaDemo)

Small .NET producer/consumer lab with Docker-based Kafka setup. Focused on making asynchronous message flow easy to inspect.

### [C# Load Test Tool](https://github.com/trandat1114/CSharp-Donace-Load-Test-Tool)

A lightweight command-line experiment for repeated HTTP requests and API performance exploration.

### [Ocean IS Portfolio](https://github.com/trandat1114/new-ocean-is-portfolio)

Current portfolio direction: a visual, engineering-focused presentation of how I build and think about systems.

---

## 05 — THINGS I'VE WORKED ON

### Enterprise / Water Billing

**.NET · SQL Server · EF Core · Dapper · Hangfire · IIS · Azure DevOps**

Large data sets, payment and invoice workflows, synchronization, reporting, scheduled jobs, and database performance work.

### Travel / Booking

**.NET · Microservices · CQRS · Event Sourcing · RabbitMQ**

Breaking down business workflows, asynchronous communication, service boundaries, and backend architecture.

### Full-stack Products

**React · Next.js · TypeScript · .NET APIs**

Building interfaces and APIs together so the contract between them stays boring—in a good way.

---

## 06 — CURRENTLY

I'm pushing deeper into the stuff around the application:

~~~text
.NET
 ├── distributed systems
 ├── messaging
 ├── observability
 ├── performance
 ├── security
 └── reliability

Exploring
 ├── Kubernetes
 ├── deeper Azure architecture
 ├── distributed tracing
 └── platform engineering
~~~

The goal is simple:

> **Write less accidental complexity. Understand more of the system.**

---

## 07 — ENGINEERING NOTEBOOK

The profile is also becoming a small public engineering notebook:

- [Dream Architecture](./docs/dream-architecture/README.md) — system designs and trade-offs
- [Engineering Labs](./docs/engineering-labs/README.md) — experiments that should be measured
- [Dev Random](./docs/dev-random/README.md) — short notes from the engineering side of the work

The rule is simple: **show the reasoning, show the evidence, keep the claims honest.**

## 08 — OUTSIDE THE CHECKLIST

I also like making things that don't necessarily belong in a corporate architecture diagram.

Small experiments. Games. Interfaces. Weird prototypes. Trying a new tool just to see what happens.

Some projects work.

Some become useful.

Some teach me exactly what **not** to do.

All of them end up teaching something.

---

## 08 — LEETCODE

[![LeetCode Stats](https://www.readmecodegen.com/api/leetcode-stats?username=TranDat1114&theme=github_dark)](https://leetcode.com/u/TranDat1114/)

---

## 09 — FIND ME

**Portfolio:** https://jayandy.id.vn  
**Email:** dattranphu1114@gmail.com  
**GitHub:** https://github.com/trandat1114  
**LinkedIn:** https://www.linkedin.com/in/tran-phu-dat-526a82288/

<br>

<sub>DAT TRAN / J.ANDY · BUILD · BREAK · MEASURE · REBUILD</sub>
