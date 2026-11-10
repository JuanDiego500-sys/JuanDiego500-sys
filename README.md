# Hi, I'm Juan Diego 👋

**Cloud & Automation Engineer** · Systems Engineer (Universidad de Manizales, Dec 2026) · Manizales, Colombia 🇨🇴

I build cloud infrastructure and automation: Infrastructure as Code, CI/CD pipelines, Kubernetes and AI agents.
From April to October 2026 I was an **AI & Automation Engineer intern at Mercedes-Benz** in Germany, working with Azure, Terraform, Kubernetes, Argo CD and AI agents. I went there as a **DAAD scholar** and also did an exchange semester at Ruhr-Universität Bochum.

### 🔭 What I'm working on
- **[azure-db-platform](https://github.com/JuanDiego500-sys/azure-db-platform)**: a GitOps platform on Azure. Terraform builds the infrastructure, GitHub Actions runs it (OIDC, no stored secrets), and Argo CD deploys PostgreSQL with pgvector on k3s. Secrets live in Azure Key Vault.

### ✅ Recently shipped
- **[reservas-espacios-api](https://github.com/JuanDiego500-sys/reservas-espacios-api)**: a REST API for booking university labs, meeting rooms and an auditorium, built in 3 days as a technical challenge (with a requirement change on day 3 and a live code interview without AI).
  - Enforces 8 business rules and creates weekly recurring bookings **all or nothing** in a single transaction.
  - **Concurrency-safe:** overlaps are checked in the service *and* blocked by a PostgreSQL `EXCLUDE USING gist` constraint; status changes use row locks (`SELECT … FOR UPDATE`).
  - Business rules are pure functions with an injected clock, covered by **86 Vitest tests**. Parameterized SQL, no ORM.
  - **CI/CD with GitHub Actions:** type check, tests and build on every push/PR, then a multi-stage Docker image published to GitHub Container Registry.
  - AI use documented critically in a log of key prompts and where the AI was wrong.

  `TypeScript · Astro · PostgreSQL · Docker · GitHub Actions · GHCR · Vitest`

### 🛠️ Tech
**Cloud & IaC:** Azure · Terraform · AWS (basics) · VMware
**DevOps:** Kubernetes · Argo CD · GitHub Actions (CI/CD) · Docker (multi-stage builds, GHCR) · k9s
**Backend:** TypeScript / Node.js · Java / Spring Boot · PostgreSQL (constraints, transactions, locking) · REST API design
**Testing:** Vitest · unit testing of pure business logic
**AI:** AI agents · LLM-assisted development (Claude Code)

### 🌍 Languages
🇪🇸 Spanish: native · 🇬🇧 English: advanced (C1) · 🇩🇪 German: C1 (TestDaF)

### 📫 Contact
[LinkedIn](https://www.linkedin.com/in/juandiegogiraldo-softwaredevelopment)

Open to **Cloud, DevOps, Automation and Backend** roles. I prefer remote work or Medellín.
