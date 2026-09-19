# Hi, I'm Yovanny Cenobio 👋
### Infrastructure Engineer & SecOps Specialist | Data Pipeline Architect

I design, build, and optimize high-availability data infrastructure and automated security pipelines. My background combines deep system-level Linux and database engineering with enterprise change management and threat-detection intelligence.

---

## 🚀 Core Architectural Projects

### 💳 1. Autonomous Transaction Ingestion & AML Monitor
* **Core Stack:** MariaDB, SQL Scripting, Linux CLI, Cron, Python (Simulation)
* **The Engineering:** Designed a partitioned Star Schema database ledger that completely decouples transaction logs from operational dimensions. Solved OS-level permission blocks (`Errcode 2`) using globally secure staging vectors.
* **The Analytics:** Implemented a real-time sliding-window calculation utilizing **SQL Window Functions (`LAG() OVER ... PARTITION BY`)** to isolate 20-minute rapid-fire micro-deposit loops ("structuring") designed to evade static reporting limits.
* **Automation:** Wired a custom Bash pipeline directly to the **Linux Cron Daemon** to poll ledger indexes every 60 seconds, outputting violation metrics to an immutable alert ledger.

### ⚡ 2. Asymmetric SIEM Log Ingestion & Distributed Cache
* **Core Stack:** Apache Kafka (KRaft), Redis RAM Cache, MongoDB, Docker, Python
* **The Engineering:** Built an asynchronous message-brokered ingestion network inside an isolated Docker container bridge system to intercept polymorphic JSON security logs (Auth, Firewall, Threat Intel) without data drop.
* **Performance Layer:** Mitigated heavy database disk I/O thrashing by engineering a **Cache-Aside Pattern** via **Redis** with a strict 60-second Time-to-Live (TTL) expiration. 
* **Metrics:** Benchmarked system capacity to successfully process **6,780+ Write operations/sec** and **7,290+ Read operations/sec** directly out of RAM.

### 🔒 3. Cryptographic Infrastructure Auditing & Change Compliance Daemon
* **Core Stack:** Python, SQLite/MariaDB, Cryptography, Linux Cron, Diff-Parsing
* **The Engineering:** Developed an immutable, tamper-proof background auditing daemon. Every logged configuration snapshot is calculated by hashing the current file state *combined* with the string hash of the **previous database record**, creating a secure cryptographic chain.
* **State Management:** Integrated an in-memory string difference analyzer to extract line-by-line unified delta paths (`+` and `-` modifications), avoiding duplicate file clutter and conserving disk space.

### 🏛️ 4. LAPD Crime Dataset ETL & Analytics Pipeline
* **Core Stack:** MariaDB, SQL, Systems Security, Data Normalization
* **The Engineering:** Processed over 1,004,894 rows of messy data. Engineered a secure data stream bypass via `LOAD DATA LOCAL INFILE` to clear modern database sandboxing walls (`Errcode 13: Permission Denied`).
* **Normalization:** Normalized unstructured datetime strings in-place using tokenized `STR_TO_DATE()` conversions with zero truncated rows or cell data distortion.

---

## 🛠️ Technical Matrix

* **Databases & Cache:** MariaDB / MySQL, Aerospike NoSQL, MongoDB, Redis, SQLite
* **Streaming & Automation:** Apache Kafka, Linux Shell Scripting (Bash/Zsh), Linux Cron Daemon, Python
* **Security & Infrastructure:** Splunk Enterprise (SPL), Suricata IDS, Wireshark, Docker Containerization, Access Control
* **Methodologies:** ITIL Change Management, ITSM (ServiceNow), Disaster Recovery Site Replication, Root-Cause Diagnostics
