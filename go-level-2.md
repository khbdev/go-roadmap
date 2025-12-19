## 🗓️ 2 OYLIK ROADMAP — KUNLIK REJA  
**(Dushanba–Juma, Dam olish: Shanba–Yakshanba)**  
*Kuniga 6–8 soat: 40% nazariya/docs o‘qish + 60% kod yozish/praktika*  
*Har Juma oxirida: Hafta review + GitHub’ga yangi commit (loyihaga qo‘shish)*

### 📅 1-OY: DEEP ENGINEERING

#### **1-HAFTA: OS + Networking + Go Internals**
- **Dushanba** (OS chuqur)  
  - Linux processes, threads, signals (SIGTERM, SIGKILL, SIGQUIT)  
  - Graceful shutdown real production misollari (Kubernetes PreStop hook)  
  - strace, lsof, ps, top, htop bilan real app trace qilish  
  - Amaliyot: TodoList’ga SIGTERM handler yozing (context cancel + waitgroup)  
- **Seshanba** (OS + tools)  
  - cgroups, namespaces, /proc filesystem  
  - tcpdump, netstat, ss, ip route bilan network debug  
  - Amaliyot: Loyihangizni strace bilan run qilib, system call’larni tahlil qiling  
- **Chorshanba** (Networking chuqur)  
  - TLS handshake (client hello → server hello → key exchange)  
  - HTTP/2 multiplexing, server push, keep-alive  
  - Proxy: nginx reverse proxy, load balancing basics  
  - Amaliyot: Gin app’ga HTTP/2 enforce qiling, nginx config yozing  
- **Payshanba** (Go internals)  
  - Go scheduler (GOMAXPROCS, work stealing, netpoller)  
  - Escape analysis (go build -gcflags="-m")  
  - Stack vs heap allocation  
  - Amaliyot: Loyihada escape analysis qilib, allocation kamaytiring  
- **Juma** (Go profiling)  
  - pprof: CPU, heap, block, mutex profiling  
  - tracing, runtime/trace  
  - Amaliyot: Online Test Platform’da pprof endpoint qo‘shing, real bottleneck toping → GitHub commit + review

#### **2-HAFTA: Databases Mastery**
- **Dushanba** (PostgreSQL queries)  
  - EXPLAIN ANALYZE, slow query log  
  - Index types: B-Tree, Hash, GIN, BRIN  
  - Composite indexes, covering indexes  
  - Amaliyot: Online Test’da slow query topib, index qo‘shing  
- **Seshanba** (PostgreSQL advanced)  
  - Vacuum, autovacuum, bloat  
  - Table partitioning (range/list)  
  - Amaliyot: Katta table yarating, partition qiling  
- **Chorshanba** (Replication)  
  - Streaming replication, logical replication  
  - WAL, slots, failover basics  
  - Amaliyot: docker-compose bilan master-slave setup  
- **Payshanba** (Redis advanced)  
  - Redis Cluster, Sentinel  
  - Eviction policies (allkeys-lru vs volatile-lfu)  
  - Lua scripts, Redis Streams  
  - Amaliyot: TodoList caching’ni Redis Cluster’ga o‘tkazing  
- **Juma** (Consistency)  
  - Cache invalidation patterns (cache-aside, write-through)  
  - Stale reads handling, TTL strategy  
  - Amaliyot: Cache invalidation bug simulate qilib, fix qiling → commit + review

#### **3-HAFTA: Message Brokers**
- **Dushanba** (RabbitMQ advanced)  
  - Quorum queues, streams, lazy queues  
  - Mirroring policy, dead letter exchanges  
  - Amaliyot: TodoList’da quorum queue’ga o‘tish  
- **Seshanba** (Kafka basics)  
  - Topic, partition, replication factor  
  - Producer config (acks, batch.size)  
  - Amaliyot: docker-compose bilan Kafka cluster  
- **Chorshanba** (Kafka consumer)  
  - Consumer group, rebalance, offset management  
  - Exactly-once semantics, idempotent producer  
  - Amaliyot: Go producer + consumer yozing (segmentio/kafka-go)  
- **Payshanba** (Trade-offs + patterns)  
  - RabbitMQ vs Kafka real case’lar  
  - Outbox pattern, Transactional Outbox  
  - CDC basics (Debezium intro)  
  - Amaliyot: TodoList’da outbox pattern qo‘shing  
- **Juma** (Refactor)  
  - TodoList RabbitMQ’ni Kafka bilan refactor prototype  
  - Performance test (throughput, latency)  
  - Commit + review

#### **4-HAFTA: Architecture + System Design Basics**
- **Dushanba** (Clean/Hexagonal deep)  
  - Dependency inversion real misollar  
  - Ports & Adapters pattern  
  - Amaliyot: Online Test’da layer’larni qayta tahlil qiling  
- **Seshanba** (DDD intro)  
  - Entities, Value Objects, Aggregates  
  - Bounded Context  
  - Amaliyot: Bitta service’ga DDD qo‘llang  
- **Chorshanba** (System Design: Rate Limiter)  
  - Token bucket vs Leaky bucket vs Sliding window  
  - Distributed rate limiter (Redis)  
  - Amaliyot: Distributed rate limiter prototype yozing  
- **Payshanba** (System Design: Notification + Idempotency)  
  - Notification system design (email + push)  
  - Idempotent webhook handler  
  - Amaliyot: Idempotency key bilan API yozing  
- **Juma** (Design + diagram)  
  - WebSocket scaling design  
  - Har design’ga draw.io diagram  
  - GitHub’ga qo‘shib review

### 📅 2-OY: ADVANCED + DEVOPS + FINAL

#### **5-HAFTA: Advanced System Design**
- **Dushanba** → Real-time Chat design (WebSocket + Redis Pub/Sub)  
- **Seshanba** → URL Shortener (highload + analytics)  
- **Chorshanba** → Distributed Cache design  
- **Payshanba** → E-commerce Order Service (Saga + Outbox)  
- **Juma** → API Gateway design → har kuni 1 design + diagram + 45 min video record (o‘zingizga)

#### **6-HAFTA: DevOps + Observability**
- **Dushanba** → Docker advanced (multi-stage, scratch, trivy scan)  
- **Seshanba** → Kubernetes basics (minikube: Deployment, Service, Ingress)  
- **Chorshanba** → K8s advanced (ConfigMap, Secret, HPA)  
- **Payshanba** → Observability: Structured logs + trace_id (OpenTelemetry intro)  
- **Juma** → Prometheus + Grafana (custom exporter yozing) + Online Test deploy to minikube

#### **7-HAFTA: API + Security + Payment**
- **Dushanba** → gRPC advanced (streaming, interceptors)  
- **Seshanba** → GraphQL (dataloader, N+1 fix)  
- **Chorshanba** → Security (OWASP Top 10, JWT best practices)  
- **Payshanba** → Payment systems (idempotency key, webhook retry)  
- **Juma** → Fake Payme/Click integratsiyasi + test → commit

#### **8-HAFTA: Testing + Mock + Polish**
- **Dushanba** → Advanced testing (integration, contract, fuzz)  
- **Seshanba** → Load testing (k6 script yozing)  
- **Chorshanba** → Mock interview 1–2 (system design + Go deep)  
- **Payshanba** → Portfolio polish (diagram, README EN, achievements)  
- **Juma** → Rezyume final + behavioral answers tayyorlash + full mock interview

---

Har Juma kechqurun:  
- Hafta nimalarni o‘rganganingizni qisqa yozing  
- GitHub’ga yangi commit/qo‘shimcha  
- Keyingi hafta reja review
