📅 2 OYLIK (8 HAFTA) ROADMAP



---

## **1-HAFTA — Concurrency + Testing Basics**

**Maqsad:** Goroutine va channel asoslarini tushunish, parallelism va testing bilan tanishish

### Nazariya
	
- `go func() {...}()` sintaksisi
    
- Goroutine yengilligi
    
- Channel (buffered/unbuffered), send/receive bloklanish, close semantics
    
- Select + timeout
    
- Fan-in / Fan-out pattern
    
- `sync.Mutex` va `WaitGroup`
    
- Race condition oddiy misollar
    
- Table-driven test va benchmark konseptlari
    

### Amaliy

- Parallel fayl o‘qish (goroutine + WaitGroup + channel)
    
- Buffered vs unbuffered channel test
    
- JSON parser + table-driven test
    
- Benchmarking `testing.B`
    
- Oddiy fan-out/fan-in worker pool
    
- Select + timeout misoli (goroutine cancel)
    

---

## **2-HAFTA — Database Systems (SQL / NoSQL / Redis / File Storage)**

**Maqsad:** Database bilan ishlash va basic caching

### SQL (PostgreSQL)

- CRUD + simple JOIN
    
- Primary key, foreign key
    
- Transaction basics + commit/rollback
    
- Mini-task: Go + SQL CRUD API
    

### NoSQL (MongoDB)

- Document modeling
    
- Embedding vs referencing
    
- CRUD API bilan amaliy mashqlar
    

### Redis

- Cache-aside pattern
    
- TTL / expire
    
- Simple rate limiter
    
- Pub/Sub overview
    

### File Storage

- Local vs Object storage
    
- Upload / download
    
- Redis mapping for file paths
    

### Mini-projectlar

1. SQL + Mongo hybrid service
    
2. Redis caching + rate limiter
    
3. File upload service (local + Redis key mapping)
    

---

## **3-HAFTA — Message Brokers & Async Systems**

**Maqsad:** Non-blocking, high-load capable system yaratish

### RabbitMQ

- Exchanges (direct, topic, fanout)
    
- Routing keys
    
- Ack/Nack + retry
    
- Dead letter queues
    
- Idempotency patterns
    

### Kafka

- Topic / partition / consumer group
    
- Offset management
    
- Delivery semantics (at-least-once, exactly-once)
    
- Event ordering
    

### Mini-projectlar

1. Email notification queue
    
2. Event-driven user activity log (Kafka)
    
3. Background worker pool with retries
    

---

## **4-HAFTA — API & Communication Protocols**

**Maqsad:** Industry standard API’larni ishlab chiqish

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
    

### Mini-projectlar

1. REST CRUD service
    
2. gRPC UserService + Gateway
    
3. GraphQL Product API
    
4. Gateway routing + rate limit
    

---

## **5-HAFTA — Architecture & System Design**

**Maqsad:** Qaysi arxitektura qayerda ishlatishni bilish

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
    

### Mini-projectlar

1. Monolith → microservices refactor
    
2. Event-driven order processing system
    
3. Cache layer + fallback
    

---

## **6-HAFTA — Design Patterns & Clean Code**

**Maqsad:** Kodni expandable, readable va maintainable qilish

### Design Patterns

- Factory / Strategy / Adapter / Observer
    
- Repository / Decorator / Circuit Breaker
    

### Clean Code

- SOLID principles
    
- Dependency Injection
    
- Layered vs Clean Architecture
    
- Anti-patternlar
    

### Mini-projectlar

1. Service using Repository + Factory
    
2. Adapter example: external API integration
    
3. Logging middleware + centralized error
    

---

## **7-HAFTA — Testing & Best Practices**

**Maqsad:** Production-ready, resilient code

### Testing

- Unit test / Table-driven test
    
- Mocking
    
- Integration test
    
- Benchmarking
    

### Best Practices

- Logging / Error handling / Retry & backoff
    
- Graceful shutdown / Health check
    
- Config management / Secrets
    

### SDLC

- Requirement → Design → Develop → Test → Deploy → Monitor
    

### Mini-projectlar

1. Full test coverage REST + gRPC service
    
2. Retry + backoff simulation
    
3. Health check + graceful shutdown
    

---

## **8-HAFTA — DevOps, Cloud & Final System**

**Maqsad:** End-to-End Go Engineer

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
