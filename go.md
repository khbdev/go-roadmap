
---

## 🔵 1-OY: Go Asoslari + CLI + REST API

### ✅ 1-Hafta: Go Asoslari va CLI

### 📘 Nazariya:

#### 1. Go O‘rnatish va Boshlang‘ich Tuzilish

* `go install`, `go run`, `go build`, `go mod init`
* Fayl tuzilmasi: `package main`, `import`, `func main()`

#### 2. O‘zgaruvchilar va Data Types

* `var`, `:=` shorthand
* Data types: `int`, `float64`, `string`, `bool`
* Constants: `const`

#### 3. Chiqarish va Formatlash

* `fmt.Println`, `fmt.Printf`, `fmt.Sprintf`

#### 4. Operatorlar

* Aritmetik: `+`, `-`, `*`, `/`, `%`
* Taqqoslash: `==`, `!=`, `>`, `<`, `>=`, `<=`
* Mantiqiy: `&&`, `||`, `!`

#### 5. Shart Operatorlari

* `if`, `else`, `else if`
* `switch`, `case`, `default`

#### 6. Takrorlash Operatorlari

* `for`, `for range`

#### 7. Funksiyalar

* Oddiy funksiya, parametrlar va qaytarish
* `return`, `multiple return`
* Rekursiya

#### 8. Pointerlar

* `*` va `&` operatorlari bilan ishlash
* Value vs Reference

#### 9. Struct

* Struct yaratish, fieldlar, struct ichida methodlar

#### 10. Interface

* Interface yaratish, struct bilan ishlatish

#### 11. Map

* Map yaratish, o‘zgartirish, o‘qish, o‘chirish

#### 12. Error Handling

* `error` tipi, `errors.New`, `fmt.Errorf`, custom error

#### 13. Time Moduli

* `time.Now()`, `time.Format()`, `time.Sleep()`

#### 14. Fayllar Bilan Ishlash

* `os.Open`, `ioutil.ReadFile`, `bufio.NewReader`
* Faylga yozish: `os.Create`, `WriteString`

#### 15. JSON Parsing

* `encoding/json`: `json.Unmarshal`, `json.Marshal`
* Struct bilan ishlatish

#### 16. Packages

* Custom package yaratish va ulardan foydalanish

---

### 🧪 Amaliyot:

#### 1. CLI Kalkulyator

* Foydalanuvchidan ikki son va operator olish
* Amalni bajarib natijani chiqarish

#### 2. JSON Parser

* JSON fayldan ma’lumot o‘qish
* Structga parse qilish
* Struct ma’lumotlarini chiqarish
---

### ✅ 2-Hafta: Gorutinalar, Channel, Test

**Nazariya:**

* `go func()`, gorutinalar va channel
* Buffered/unbuffered channel, `select`
* `sync.Mutex`, `WaitGroup`
* Unit test, table-driven test, benchmark

**Amaliyot:**

* Parallel fayl o‘qish dasturi
* Unit test bilan JSON parser

---

### ✅ 3-Hafta: HTTP Server, Gin Framework, REST

**Nazariya:**

* `net/http`, routing, handler
* Gin framework, middleware, logging
* JSON request/response, validatsiya
* CRUD REST API (memoryda vaqtincha saqlash)

**Amaliyot:**

* Kitob CRUD API (Gin framework)
* Logging va validatsiya middleware

---

### ✅ 4-Hafta: MySQL + ORM + Relationship

**Nazariya:**

* SQL asoslari: SELECT, INSERT, UPDATE, DELETE
* MySQL + Go (`gorm.io/gorm`)
* One-to-One, One-to-Many, Many-to-Many
* JOIN, foreign key, migrate qilish
* SQL injectiondan himoyalanish

**Amaliyot:**

* User, Post, Comment CRUD (MySQL bilan)
* User-Post (1\:M), Post-Tag (M\:M) relation

---

## 🔵 2-OY: JWT, Redis, Queue, Docker, Loyihalar

### ✅ 5-Hafta: Auth + JWT + Role

**Nazariya:**

* JWT nima, qanday ishlaydi
* `github.com/golang-jwt/jwt`
* Access/refresh token, expiry, middleware
* Role-based access: admin/user

**Amaliyot:**

* Auth API (register, login, refresh)
* Blog API JWT orqali himoya

---

### ✅ 6-Hafta: Redis + Caching + Session

**Nazariya:**

* Redis tushunchasi va Go bilan ishlash (`go-redis`)
* Caching patternlar: read-through, write-through
* Session saqlash, TTL, expire
* Rate limit qilish

**Amaliyot:**

* Redis bilan product caching
* Session-based login tizimi

---

### ✅ 7-Hafta: Queue + Job + Email

**Nazariya:**

* Background jobs: nima va nima uchun
* `asynq`, `go-workers`, `rabbitmq`
* Retry, delay, priority, dead letter queue
* Email yuborish (`gomail`)

**Amaliyot:**

* Signup -> email yuboruvchi background job
* Asynq bilan task queue

---

### ✅ 8-Hafta: Docker + CI/CD

**Nazariya:**

* Dockerfile yozish, konteyner tushunchasi
* Docker Compose: API + Redis + DB
* GitHub Actions bilan test/build
* CI/CD pipeline: test -> build -> deploy

**Amaliyot:**

* Full API ni docker-compose bilan ishga tushirish
* GitHub Action orqali CI/CD pipeline qilish

---

## 🔵 3-OY: Mikroservis, gRPC, Monitoring, Portfolio

### ✅ 9-Hafta: Mikroservis arxitekturasi

**Nazariya:**

* Monolit vs mikroservis
* Service-to-service kommunikatsiya
* API Gateway, Service Discovery

**Amaliyot:**

* User-service, Product-service, Order-service
* API Gateway (Gin bilan)

---

### ✅ 10-Hafta: gRPC + Protobuf

**Nazariya:**

* gRPC nima, qachon kerak
* Protobuf yozish, compile qilish
* gRPC server/client yozish

**Amaliyot:**

* User-service ni gRPC qilish
* Frontend bilan REST, ichki aloqa gRPC

---

### ✅ 11-Hafta: GraphQL + Monitoring

**Nazariya:**

* GraphQL nima, RESTdan farqi
* Schema, query, mutation
* Prometheus, Grafana monitoring

**Amaliyot:**

* Product GraphQL API
* Prometheus bilan API monitoring

---

### ✅ 12-Hafta: Portfolio + GitHub + Rezyume

**Nazariya:**

* GitHub profiling, README yozish
* Portfolio loyihalarni tayyorlash
* Rezyume tayyorlash (EN va UZ)

**Amaliyot:**

* 3 ta loyiha: Auth API, Todolist, blog mikroservis
* GitHub’ga joylash, README, Dockerfile

---

## 📋 Kunlik Tavsiya Reja

| Vaqt        | Faoliyat              |
| ----------- | --------------------- |
| 17:00–18:00 | Nazariya              |
| 18:00–20:00 | Kod yozish, API       |
| 20:00–21:30 | Loyihada ishlash      |
| 21:30–22:30 | GitHub, qayta ko‘rish |

---

## 📚 Tavsiya Manbalar:

* [https://go.dev](https://go.dev) — rasmiy hujjat
* [https://gobyexample.com](https://gobyexample.com) — misollar
* Kitob: "Let’s Go" – Alex Edwards
* YouTube: Golang Dojo, Hussein Nasser
* GitHub: real loyihalarni o‘rganish

---

