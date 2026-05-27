# ✅ Generate Business Diagrams with Mermaid Using ChatGPT — Step-by-Step (20 Examples)

Mermaid lets you **draw diagrams from text**. That makes it perfect to co-create visual assets with ChatGPT: you describe the scenario; ChatGPT returns **Mermaid code**; you paste it into Markdown/Docs/Wikis/Notion, etc.

Important Links:

* **Mermaid Official Site, Diagramming and Charting Tool Link:** <https://mermaid.js.org/>
* **Diagram Generation and Creation Portal Link:** <https://app.diagrams.net/>

Below you’ll get:

* A **repeatable workflow** + reusable prompts
* **20 common business diagrams** across departments
* For each: a **copy-paste prompt** and **Mermaid code** (ready to render)

---

## ☑️ A) Quick Workflow

1. **Pick diagram type** (flowchart, sequence, gantt, journey, etc.).
2. **List entities/steps** (actors, lanes, dates, owners).
3. Ask ChatGPT with the **Diagram Request Prompt** below.
4. Paste the returned code into a Markdown block:

   ````
   ```mermaid
   ...code...
   ```
   ````
5. **Iterate** (add lanes, colors, milestones) with the **Revise Prompt** below.
6. **Validate** (IDs unique, short labels, orientation set).

### 🔰 Reusable prompts

**Diagram Request Prompt**

```
Create a Mermaid <DIAGRAM_TYPE> for the scenario below.
Rules:
- Output Mermaid code ONLY (no prose).
- Orientation: <TB|BT|LR|RL>.
- Use short node IDs (no spaces); labels in [brackets].
Scenario:
<<<your bullets/entities/steps>>>
```

**Revise / Improve Prompt**

```
Revise the last diagram:
- Add <lane/actor/milestone/node>.
- Style <nodeIDs> using classDef (colors).
- Keep orientation <LR/TB>. Ensure unique IDs.
Return Mermaid code only.
```

---

## ☑️ B) Case Study

🔴 **Prompt:** ```Please generate a complete documentation to mention all the step by step in details required to conduct a large recruitment drive phase wise organized by a major manufacturing company. Please consider all the conditional states in this recruitment drive.```

🔴 **Prompt:** ```Can you generate a complete Mermaid Code to generate a complete Flow Chart of these processes and sub-processes to understand it better?```

🔴 **Prompt:** ```Against this Mermaid Code execution at https://app.diagrams.net/ web portal following error message is being obtained. Please revise the Mermaid code once. Please keep the layout of the flowchart in Top-Down - ERROR MESSAGE...```

---

## ☑️ C) 20 Common Business Diagrams (Prompts + Mermaid Code)

> Tip: You can paste each Mermaid block directly into your doc to render.

### 🔰 1) Sales — Lead-to-Cash Flow (Flowchart)

**Prompt**

```
Mermaid flowchart (LR) for Lead→Qualify→Proposal→Negotiate→Closed Won/Closed Lost; include "Disqualify".
Code only.
```

```
flowchart LR
  A[Lead] --> B[Qualify]
  B -->|Qualified| C[Proposal]
  B -->|Disqualified| X[Archive]
  C --> D[Negotiate]
  D --> E[Closed Won]
  D --> F[Closed Lost]
  classDef win fill:#e6ffe6,stroke:#0a0;
  class E win;
```

<img width="1127" height="287" alt="image" src="https://github.com/user-attachments/assets/a9420827-b366-43eb-873e-6f3f2999f641" />

---

### 🔰 2) HR — Hiring (Swimlanes via Subgraphs)

**Prompt**

```
Flowchart (LR) with lanes HR, Manager, Candidate: Post→Screen→Interview→Offer→Accept/Reject.
Use subgraphs as lanes. Code only.
```

```
flowchart LR
  subgraph HR[HR]
    A[Post Job]
    D[Prepare Offer]
  end
  subgraph HM[Hiring Manager]
    B[Screen CVs]
    C[Interviews]
  end
  subgraph CAND[Candidate]
    E[Accept]
    F[Reject]
  end
  A --> B --> C --> D
  D --> E
  D --> F
```

<img width="1295" height="461" alt="image" src="https://github.com/user-attachments/assets/c097e6b1-078c-4714-be3b-50fb8c40611c" />

---

### 🔰 3) Marketing — Campaign Workflow (Flowchart)

**Prompt**

```
Flowchart (LR): Brief→Assets→Approvals→Launch→Measure→Optimize.
Code only.
```

```
flowchart LR
  B[Brief] --> A[Create Assets] --> P[Approvals] --> L[Launch]
  L --> M[Measure Results] --> O[Optimize]
```

<img width="1337" height="101" alt="image" src="https://github.com/user-attachments/assets/99719390-f86c-4aa2-b0ff-c9f895c627f8" />

---

### 🔰 4) Product — Feature Delivery Timeline (Gantt)

**Prompt**

```
Gantt for feature delivery: Discovery(1w), Build(2w), UAT(1w), Launch(1d milestone). Start 2025-09-01.
Code only.
```

```
gantt
  title Feature Delivery
  dateFormat  YYYY-MM-DD
  section Discovery
  Research    :done,   d1, 2025-09-01, 5d
  section Build
  Dev Sprint  :active, b1, 2025-09-08, 10d
  section UAT
  Test Cycle  :        u1, 2025-09-22, 5d
  section Launch
  Go-Live     :milestone, g1, 2025-09-29, 0d
```

<img width="1456" height="206" alt="image" src="https://github.com/user-attachments/assets/83b4dc57-c2de-4a85-9ab0-8a577b29c480" />

---

### 🔰 5) Support — Escalation Path (State Diagram)

**Prompt**

```
State diagram: New→Triage→In Progress→Waiting on Customer→Resolved/Closed. Include Escalated.
Code only.
```

```
stateDiagram-v2
  [*] --> New
  New --> Triage
  Triage --> InProgress
  InProgress --> Waiting
  Waiting --> InProgress
  InProgress --> Escalated
  InProgress --> Resolved
  Resolved --> Closed
```

<img width="1526" height="606" alt="image" src="https://github.com/user-attachments/assets/5edc5394-e8c3-4bd7-b16d-9cf4699c4d71" />

---

### 🔰 6) Finance — Invoice to Cash (Flowchart)

**Prompt**

```
Flowchart (TB): Create Invoice→Send→Receive Payment→Reconcile→Close Period.
Add "Overdue Notice" branch. Code only.
```

```
flowchart TB
  A[Create Invoice] --> B[Send]
  B --> C[Receive Payment]
  C --> D[Reconcile]
  D --> E[Close Period]
  B -->|No Payment| X[Overdue Notice] --> B
```

<img width="1526" height="635" alt="image" src="https://github.com/user-attachments/assets/969d1790-7905-49db-856f-b0c37022c8e8" />

---

### 🔰 7) IT — System Context (Components & Integrations)

**Prompt**

```
Flowchart (LR): Browser→Frontend→Backend→DB/Warehouse; integrations: Payment, Email, SSO. Group with subgraphs.
Code only.
```

```
flowchart LR
  subgraph Client
    U[Browser]
  end
  subgraph App[Web App]
    FE[Frontend]
    BE[Backend API]
  end
  subgraph Data[Data Layer]
    DB[(OLTP DB)]
    WH[(Warehouse)]
  end
  subgraph Ext[External]
    PAY[Payment]
    EM[Email]
    SSO[SSO]
  end
  U --> FE --> BE --> DB
  BE --> WH
  BE --> PAY
  BE --> EM
  BE --> SSO
```

<img width="1561" height="617" alt="image" src="https://github.com/user-attachments/assets/38129196-5453-404e-9ca5-1cf355a75e26" />

---

### 🔰 8) Analytics — Data Pipeline (Sequence)

**Prompt**

```
SequenceDiagram: Source→ETL→Warehouse→BI; events: extract→transform→load→query→dashboard.
Code only.
```

```
sequenceDiagram
  participant S as Source
  participant E as ETL
  participant W as Warehouse
  participant B as BI Tool
  S->>E: Extract
  E->>E: Transform
  E->>W: Load
  B->>W: Query
  W-->>B: Result Set
  B-->>User: Dashboard
```

<img width="1541" height="516" alt="image" src="https://github.com/user-attachments/assets/32d7167a-0233-43fc-8a57-7040d923f85e" />

---

### 🔰 9) CX — Customer Journey (Journey)

**Prompt**

```
Journey for SaaS: Awareness, Trial, Onboarding, Adopt, Renew (scores).
Code only.
```

```
journey
  title SaaS Customer Journey
  section Awareness
    Ad Click: Customer:3
    Landing Page: Customer:4
  section Trial
    Sign-up: Customer:4
    First Dash: Customer:5
  section Onboarding
    Tutorial: Customer:4
    First Value: Customer:5
  section Adopt
    Daily Use: Customer:4
  section Renew
    Renewal: Customer:3
```

<img width="1532" height="423" alt="image" src="https://github.com/user-attachments/assets/93f85066-690c-47e5-9b07-3bcef4466660" />

---

### 🔰 10) Sales — Funnel (Flowchart TB)

**Prompt**

```
Flowchart (TB): Visitors→Leads→MQL→SQL→Opportunity→Won; widths implied by nodes.
Code only.
```

```
flowchart TB
  V[Visitors] --> L[Leads] --> M[MQL] --> S[SQL] --> O[Opportunity] --> W[Won]
```

<img width="1532" height="657" alt="image" src="https://github.com/user-attachments/assets/67906159-72aa-404c-a8ed-d30c7e9a6624" />

---

### 🔰 11) Supply Chain — SIPOC (Flowchart with Groups)

**Prompt**

```
Flowchart (LR) showing SIPOC: Suppliers→Inputs→Process→Outputs→Customers. Use subgraphs.
Code only.
```

```
flowchart LR
  subgraph S[Suppliers]
    S1[Vendor A]
    S2[Vendor B]
  end
  subgraph I[Inputs]
    I1[Materials]
    I2[Specs]
  end
  subgraph P[Process]
    P1[Assemble]
    P2[QA]
  end
  subgraph O[Outputs]
    O1[Finished Goods]
  end
  subgraph C[Customers]
    C1[Retail]
    C2[Wholesale]
  end
  S1 --> I1
  S2 --> I2
  I1 --> P1 --> P2 --> O1 --> C1
  O1 --> C2
```

<img width="1295" height="289" alt="image" src="https://github.com/user-attachments/assets/176ce7af-ce5a-477e-8812-b6b4c2c2a76e" />

---

### 🔰 12) Compliance — Requirements Traceability (Requirement Diagram)

**Prompt**

```
Requirement diagram: reqs R1,R2; tests T1,T2; design D1 satisfies R1; T1 verifies R1; T2 verifies R2.
Code only.
```

```
flowchart LR
  R1([Requirement R1: Encrypt at rest])
  R2([Requirement R2: Retain logs 90 days])
  D1[[Design D1: KMS + AES-256]]
  T1([Test T1: Validate encryption])
  T2([Test T2: Verify retention])

  D1 -- satisfies --> R1
  T1 -- verifies  --> R1
  T2 -- verifies  --> R2
```

<img width="1231" height="368" alt="image" src="https://github.com/user-attachments/assets/f13e53e8-5525-4104-9aa9-c652fcaec541" />

---

### 🔰 13) Data — ER Model (erDiagram)

**Prompt**

```
erDiagram: CUSTOMER, ORDER, ITEM, PRODUCT with PK/FK; relationships shown.
Code only.
```

```
erDiagram
  CUSTOMER ||--o{ ORDER : places
  ORDER ||--|{ ITEM : contains
  PRODUCT ||--o{ ITEM : refers
  CUSTOMER {
    string customer_id PK
    string name
    string email
  }
  ORDER {
    string order_id PK
    date   order_date
    float  total
    string customer_id FK
  }
  ITEM {
    string order_id FK
    string product_id FK
    int    qty
    float  price
  }
  PRODUCT {
    string product_id PK
    string name
    float  unit_price
  }
```

<img width="1281" height="493" alt="image" src="https://github.com/user-attachments/assets/4c14258c-acef-4699-afd1-2d618ac77d2b" />

---

### 🔰 14) Strategy — OKR Tree (Mindmap)

**Prompt**

```
Mindmap: Company OKR: Objective + 3 Key Results; each KR has 2 initiatives.
Code only.
```

```
mindmap
  root((Increase ARR 25%))
    KR1 Grow Trials
      Init Paid Ads
      Init SEO Revamp
    KR2 Improve Conversion
      Init A/B Pricing
      Init Checkout UX
    KR3 Reduce Churn
      Init Success Playbooks
      Init NPS Loop
```

<img width="1536" height="452" alt="image" src="https://github.com/user-attachments/assets/10734288-06d2-49c3-8d05-c3cb75b0c7bd" />

---

### 🔰 15) Exec — Q4 Roadmap (Timeline)

**Prompt**

```
Timeline: Kickoff, Beta, UAT, Launch, GA from Oct–Dec 2025. Code only.
```

```
timeline
  title Q4 Roadmap
  2025-10-01 : Kickoff
  2025-10-15 : Beta
  2025-11-01 : UAT
  2025-11-15 : Launch
  2025-12-01 : GA
```

<img width="1151" height="268" alt="image" src="https://github.com/user-attachments/assets/8c70bb0f-9794-40ea-b69c-aa5857336de8" />

---

### 🔰 16) Risk — Probability vs Impact (Quadrant Chart)

**Prompt**

```
Quadrant chart: x=Probability Low→High, y=Impact Low→High; plot 5 risks.
Code only.
```

```
quadrantChart
  title Risk Heatmap
  x-axis Low Prob --> High Prob
  y-axis Low Impact --> High Impact
  quadrant-1 Monitor
  quadrant-2 Reassess
  quadrant-3 Accept
  quadrant-4 Mitigate
  VendorDelay: [0.7, 0.8]
  SecBreach: [0.4, 0.9]
  PerfIssue: [0.6, 0.6]
  BudgetCut: [0.5, 0.7]
  HiringLag: [0.3, 0.5]
```

<img width="1161" height="560" alt="image" src="https://github.com/user-attachments/assets/3334f353-8675-411d-b05d-9a21801e7a96" />

---

### 🔰 17) Ops — Incident Runbook (Flowchart with Decisions)

**Prompt**

```
Flowchart (TB): Detect→Classify Sev→Notify→Mitigate→Validate→Close; include rollback branch if validate fails.
Code only.
```

```
flowchart TB
  D[Detect] --> C[Classify Severity]
  C --> N[Notify On-Call]
  N --> M[Mitigate]
  M --> V[Validate]
  V -->|Pass| CL[Close]
  V -->|Fail| RB[Rollback] --> M
```

<img width="1212" height="705" alt="image" src="https://github.com/user-attachments/assets/f5cca454-990d-4584-ac37-759d253629d0" />

---

### 🔰 18) HR — Onboarding Journey (Journey)

**Prompt**

```
Journey: Day 0, Day 1, Week 1, Month 1 with employee sentiment scores.
Code only.
```

```
journey
  title New Hire Onboarding
  section Day 0
    Offer Letter: Employee:4
    Pre-reads: Employee:3
  section Day 1
    Orientation: Employee:4
    IT Setup: Employee:3
  section Week 1
    Meet Team: Employee:5
    First Task: Employee:4
  section Month 1
    Check-in: Employee:4
    Training: Employee:5
```

<img width="1107" height="293" alt="image" src="https://github.com/user-attachments/assets/6242983e-f06d-4062-9855-ae68d96c3dce" />

---

### 🔰 19) Engineering — Service Interaction (Sequence)

**Prompt**

```
Sequence: Client→API→Cache→DB; path: request→cache miss→DB→cache set→response.
Code only.
```

```
sequenceDiagram
  participant C as Client
  participant A as API
  participant K as Cache
  participant D as DB
  C->>A: GET /items
  A->>K: Lookup
  K-->>A: Miss
  A->>D: Query
  D-->>A: Rows
  A->>K: Set Cache
  A-->>C: 200 OK
```

<img width="1510" height="663" alt="image" src="https://github.com/user-attachments/assets/bf0acdcc-17eb-4c8c-bbbb-65cdd0c44585" />

---

### 🔰 20) PMO — Program Plan (Gantt Multi-Tracks)

**Prompt**

```
Gantt: Workstreams A (2w), B (3w), C (2w), shared UAT(1w), Release milestone. Start 2025-10-06.
Code only.
```

```
gantt
  title Program Plan
  dateFormat  YYYY-MM-DD
  section A
  A Sprint      :a1, 2025-10-06, 10d
  section B
  B Delivery    :b1, 2025-10-06, 15d
  section C
  C Build       :c1, 2025-10-06, 10d
  section UAT
  Shared UAT    :u1, after a1, 5d
  section Release
  Release       :milestone, r1, after u1, 0d
```

<img width="1356" height="209" alt="image" src="https://github.com/user-attachments/assets/79b65d1c-b560-436f-8dbc-211224b697f9" />

---

## ☑️ D) Styling & Tips

* **Orientation:** `flowchart LR` (left→right) or `TB` (top→bottom).
* **IDs:** short, unique (`A1`, `QA_Lead`); **labels** go in `[brackets]`.
* **Swimlanes:** use `subgraph` blocks.
* **Colors:** define classes and apply:

  ```mermaid
  flowchart LR
    A[Start] --> B[Review] --> C[Done]
    classDef ok fill:#e6ffe6,stroke:#0a0;
    class C ok;
  ```
* **Gantt:** always set `dateFormat`.
* **Sequence:** declare `participant`s first.
* **Validate:** if render fails, ask ChatGPT to “**return corrected Mermaid code only**.”

---

## ☑️ E) Fast Customizations (Prompt Snippets)

* **Add a lane/node:**
  “Add a **Finance** subgraph with node **BudgetApproval** after **Offer** (LR). Code only.”
* **Highlight critical path:**
  “Style nodes **Dev Sprint**, **Test Cycle**, **Go-Live** with red border, light red fill using `classDef`. Code only.”
* **Shorten labels:**
  “Limit labels to ≤18 chars; abbreviate sensibly. Code only.”
* **Swap orientation:**
  “Change to **TB** orientation; keep layout readable. Code only.”

---

## ☑️ F) Quality checklist & common fixes

* **Node IDs:** `A1`, `Mgr_Mkt` (no spaces). Labels go in `[brackets]`.
* **Orientation:** `flowchart LR` (left→right) or `TB` (top→bottom).
* **Subgraphs:** single-line titles only.
* **Unique IDs:** don’t reuse IDs across lanes.
* **Gantt:** always set `dateFormat`.
* **Sequence:** declare `participant` lines first.
* **Output control:** ask for **Mermaid code only** to avoid extra text breaking previews.

**Syntax-only check prompt**

```
Validate the Mermaid code for syntax errors only.
If errors exist, return a corrected version (code only). Otherwise, return the original.
```

---

### 🔰 Final tip

Start with the **simplest valid diagram**, then iterate: lanes → colors → dependencies → milestones. The tighter your prompt (entities, order, owners, dates), the cleaner the diagram Mermaid—and ChatGPT—will produce.

---
