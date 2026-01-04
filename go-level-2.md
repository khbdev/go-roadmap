📅 2 OYLIK (8 HAFTA) ROADMAP


---

## **1-HAFTA — GO CORE & CONCURRENCY (RECALL + NEW)**

**Maqsad:** Go’ni **ishlataman** emas, **tushunaman + advanced**

### Avval o‘rganilgan + yangilanish:

- Goroutines & scheduler
    
- Channel internals
    
- Context (`context.Context`)
    
- Race conditions + data races
    
- Pointers & memory model
    
- Stack vs Heap, escape analysis
    
- Garbage Collector
    
- Graceful shutdown
    

### Mini-project:

- **Parallel Worker Pool**: RabbitMQ consumer simulator
    
- **Context & timeout**: HTTP request with cancellation
    

---

## **2-HAFTA — DATABASE SYSTEMS (RECALL + NEW)**

**Maqsad:** DB bilan ishlashda **design + performance**

### SQL (MySQL / PostgreSQL)

- Schema design, normalization/denormalization
    
- Indexing (B-Tree, Hash)
    
- Query planner, EXPLAIN
    
- JOIN types
    
- Transaction + isolation level + deadlock
    
- Migration strategy, versioning
    

### NoSQL (MongoDB)

- Document modeling, embedding vs referencing
    
- Aggregation pipeline
    
- Indexing & performance
    

### Redis

- Cache-aside pattern
    
- TTL & expiration
    
- Rate limiting
    
- Distributed lock
    
- Pub/Sub
    

### File Storage

- Local vs Object (S3-style)
    
- Streaming upload/download
    
- Signed URLs / pre-signed links
    

### Mini-projectlar:

1. SQL + Mongo hybrid service
    
2. Redis caching + rate limiter
    
3. File upload service (local & Redis key mapping)
    

---

## **3-HAFTA — MESSAGE BROKERS & ASYNC SYSTEMS (NEW + RECALL)**

**Maqsad:** Systemni **non-blocking, high-load capable** qilish

### RabbitMQ

- Exchanges (direct, topic, fanout)
    
- Routing keys
    
- Ack/Nack, retry
    
- Dead letter queues
    
- Idempotency patterns
    

### Kafka

- Topic / partition / consumer group
    
- Offset management
    
- Delivery semantics (at-least-once, exactly-once)
    
- Event ordering
    

### Mini-projectlar:

1. Email notification queue
    
2. Event-driven user activity log (Kafka)
    
3. Background worker pool with retries
    

---

## **4-HAFTA — API & COMMUNICATION PROTOCOLS (RECALL + NEW)**

**Maqsad:** API’larni **industry standard** asosida qurish

### REST API

- Versioning, filtering, pagination
    
- Error standard, idempotency
    
- Validation middleware
    

### gRPC

- Unary / streaming RPC
    
- Proto design
    
- Interceptors
    
- Error codes
    

### GraphQL

- Schema design
    
- Resolver, caching, N+1 problem
    

### API Gateway

- Auth, JWT verification
    
- Rate limiting
    
- Request aggregation
    

### Mini-projectlar:

1. REST CRUD service
    
2. gRPC UserService + Gateway
    
3. GraphQL Product API
    
4. Gateway routing + rate limit
    

---

## **5-HAFTA — ARCHITECTURE & SYSTEM DESIGN (RECALL + NEW)**

**Maqsad:** Qaysi joyda qaysi arxitektura kerakligini bilish

### Architecture Patterns

- Monolith / Modular Monolith
    
- Microservices
    
- Event-driven architecture
    

### System Design

- Scalability / Availability / Consistency
    
- CAP theorem
    
- Caching strategy
    
- Saga / Choreography
    
- Service isolation + failure handling
    

### Mini-projectlar:

1. Monolith → microservices refactor
    
2. Event-driven order processing system
    
3. Cache layer + fallback
    

---

## **6-HAFTA — DESIGN PATTERNS & CLEAN CODE (RECALL + NEW)**

**Maqsad:** Kodni **expandable + readable + maintainable** qilish

### Design Patterns

- Factory / Strategy / Adapter / Observer
    
- Repository / Decorator / Circuit Breaker
    

### Clean Code

- SOLID principles
    
- Dependency Injection
    
- Layered Architecture vs Clean Architecture
    
- Anti-patternlar
    

### Mini-projectlar:

1. Service using Repository + Factory
    
2. Adapter example: external API integration
    
3. Logging middleware + centralized error
    

---

## **7-HAFTA — TESTING & BEST PRACTICES (RECALL + NEW)**

**Maqsad:** Productionga **ishonch bilan chiqarish + resilient code**

### Testing

- Unit test
    
- Table-driven test
    
- Mocking
    
- Integration test
    
- Benchmarking
    

### Best Practices

- Logging / Error handling / Retry & backoff
    
- Graceful shutdown / Health check
    
- Config management / Secrets
    

### SDLC

- Requirement → Design → Develop → Test → Deploy → Monitor
    

### Mini-projectlar:

1. Full test coverage REST + gRPC service
    
2. Retry + backoff simulation
    
3. Health check + graceful shutdown
    

---

## **8-HAFTA — DEVOPS, CLOUD & FINAL SYSTEM (NEW)**

**Maqsad:** **End-to-End Go Engineer**

### DevOps

- Docker (multi-stage build)
    
- docker-compose
    
- CI/CD (GitHub Actions / GitLab CI)
    

### Cloud & Infrastructure

- VPS / Nginx / SSL
    
- Reverse proxy
    
- Env & secrets management
    
- Basic monitoring (metrics, logs)
    

### Final Project

- Production-grade Go system:
    
    - API Gateway
        
    - Auth
        
    - DB + Cache + Queue
        
    - Worker services
        
    - Monitoring + CI/CD
        

---

