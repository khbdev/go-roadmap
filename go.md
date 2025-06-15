
---

# 🚀 Yangilangan: Sentabrgacha Go Backend Dasturchi Bo'lish Yo'l Xaritasi (MySQL bilan)

## 🎯 Maqsad: Ishga tayyor **Junior Go Backend Dasturchi**

---

## 📅 **Optimallashtirilgan 3 Bosqichli Reja**

| Davr             | Yo‘nalish                        | Amaliy Ko‘nikmalar                                                     |
| ---------------- | -------------------------------- | ---------------------------------------------------------------------- |
| **Iyun 15–30**   | Go asoslari + CLI dasturlar      | Go sintaksisi, concurrency, test yozish                               |
| **Iyul**         | Web backend + ma’lumotlar bazasi | REST API, **MySQL**, autentifikatsiya                                 |
| **Avgust 1–15**  | Ishlab chiqarishga tayyor        | Docker, deployment, portfolio to‘plash                                |
| **Avgust 16–30** | Ishga tayyor                     | Intervyu tayyorgarligi, real loyihalar                                |

---

## 🔥 **1-Bosqich: Go Asoslari + CLI Dasturlar (2 hafta)**

### 🎯 1-Hafta: Go Asoslari

#### O‘rganiladigan mavzular:

- ✅ Go o‘rnatish (`go mod`, `go run`, `go build`)
- ✅ O‘zgaruvchilar, turlar, konstantalar, funksiyalar
- ✅ Shart operatorlari: `if`, `else`, `switch`, `for` loop
- ✅ Massivlar, slices, maps, structs
- ✅ Ko‘rsatkichlar (Pointers)
- ✅ Paketlar va importlar

#### Amaliy loyihalar:

1. **CLI Kalkulyator**
2. **Fayl menejeri**
3. **JSON Parser**

---

### 🎯 2-Hafta: Kengaytirilgan Go

#### O‘rganiladigan mavzular:

- ✅ Gorutinalar va kanallar
- ✅ Interfeyslar
- ✅ Xatoliklarni boshqarish
- ✅ Test yozish (`go test`)
- ✅ Sync paketi (Mutex, WaitGroup)

#### Amaliy loyihalar:

1. **Parallel fayl protsessori**
2. **Worker Pool**
3. **CLI Chat**

---

## 🔥 **2-Bosqich: Web Backend + MySQL (4 hafta)**

### 🎯 3-Hafta: HTTP Server va Marshrutlash

#### O‘rganiladigan mavzular:

- ✅ `net/http`
- ✅ Gin framework
- ✅ Middleware, kontekst
- ✅ JSON marshalling/unmarshalling
- ✅ Validatsiya

#### Loyiha:

**Kitoblar API**

```
GET    /books          - barcha kitoblar
POST   /books          - yangi kitob qo‘shish
GET    /books/:id      - aniq kitobni olish
PUT    /books/:id      - kitobni tahrirlash
DELETE /books/:id      - kitobni o‘chirish
```

---

### 🎯 4-Hafta: MySQL bilan integratsiya

#### O‘rganiladigan mavzular:

- ✅ MySQL o'rnatish (XAMPP/standalone)
- ✅ SQL asoslari: `SELECT`, `INSERT`, `UPDATE`, `JOIN`, `GROUP BY`, `HAVING`
- ✅ Go dan MySQL ga ulanish (`database/sql`, `mysql driver`)
- ✅ ORM vs raw SQL farqi
- ✅ Migratsiyalar (`golang-migrate/migrate`)
- ✅ Connection pooling
- ✅ SQL injectiondan himoya

#### Loyiha:

**Foydalanuvchi boshqaruvi (MySQL bilan)**

* Ro‘yxatdan o‘tish / Kirish
* Parolni bcrypt orqali xeshlash
* CRUD amallari

---

### 🎯 5-Hafta: Avtorizatsiya va xavfsizlik

#### O‘rganiladigan mavzular:

- ✅ JWT avtorizatsiya
- ✅ CORS sozlamalari
- ✅ Rate limiting
- ✅ Validatsiya (validator kutubxonasi)
- ✅ XSS/CSRF himoyalari

#### Loyiha:

**Xavfsiz Blog API**

* JWT orqali kirish
* Faqat avtorizatsiyadan o'tganlar foydalanishi
* Rollar (admin, oddiy foydalanuvchi)

---

### 🎯 6-Hafta: Kengaytirilgan backend

#### O‘rganiladigan mavzular:

- ✅ Log yozish (logrus, zap)
- ✅ Konfiguratsiya (viper, .env)
- ✅ Graceful shutdown
- ✅ Health check
- ✅ Redis bilan kesh qilish

#### Loyiha:

**E-commerce API**

* Mahsulotlar, kategoriyalar
* Savat
* Buyurtma boshqaruvi
* Redis bilan tezkorlik

---

## 🔥 **3-Bosqich: Ishlab chiqarishga tayyor (2 hafta)**

### 🎯 7–8-Haftalar: DevOps va Deployment

#### O‘rganiladigan mavzular:

- ✅ Docker
- ✅ Docker Compose
- ✅ GitHub Actions (CI/CD)
- ✅ Muhitlarni boshqarish
- ✅ Monitoring va loglash

#### Loyiha:

**Mikroxizmatlar arxitekturasi**

* Foydalanuvchi xizmati
* Mahsulot xizmati
* Buyurtma xizmati
* API Gateway

---

### 🎯 9–10-Haftalar: Portfolio va intervyu tayyorlov

#### Portfolio loyihalari:

1. **Vazifa boshqaruv API** (Trello kloni)
2. **URL qisqartiruvchi** (bit.ly kloni)
3. **Real-time Chat API** (WebSocket bilan)

#### Intervyu tayyorlov:

- ✅ GitHub portfolio tayyorlash
- ✅ Rezyume yozish
- ✅ Texnik savollar
- ✅ Arxitektura savollari
- ✅ Mashq suhbatlar

---

## 🕓 Har Kunlik Optimal Rejim (17:00–00:00)

| Vaqt        | Faoliyat                              |
| ----------- | ------------------------------------- |
| 17:00–18:30 | Nazariya o‘rganish                    |
| 18:30–20:30 | Kod yozish                            |
| 20:30–22:00 | Loyihada ishlash                      |
| 22:00–23:00 | Test yozish                           |
| 23:00–00:00 | Kod ko‘rish, forumda ishtirok etish  |

---

## 🛠 Zaruriy Vositalar

### Ish muhit:
- VS Code + Go extension
- MySQL (phpMyAdmin, DBeaver)
- Postman / Insomnia
- Git + GitHub

### Resurslar:
- [go.dev](https://go.dev)
- [Go by Example](https://gobyexample.com)
- "Let's Go" kitobi — Alex Edwards
- YouTube: Anthony GG, Golang Dojo

---

## ✅ Haftalik Yutuqlar

| Hafta     | Natija                                                         |
|-----------|----------------------------------------------------------------|
| 1–2       | Go asoslari, gorutina, test                                   |
| 3–4       | REST API, MySQL bilan ishlash                                 |
| 5–6       | Xavfsizlik, Redis, validatsiya                                |
| 7–8       | Docker, CI/CD                                                 |
| 9–10      | Portfolio, intervyu                                           |

---

## 🚨 Muvaffaqiyat Kalitlari

✅ Har kuni kod yozing  
✅ GitHub’ga commit qiling  
✅ Test yozing  
✅ Qiyinchiliklarni izlab boring  

❌ Faqat video ko'rish  
❌ Ideal kodga intilish  
❌ Barchasini bir o'tkazish

---

## 🏆 Yakuniy Portfolio Loyihalari

1. **Auth bilan REST API** (JWT, CRUD, MySQL)
2. **Mikroxizmatlar** (Docker, gRPC)
3. **Real-time dastur** (WebSocket, Redis)
4. **CLI dastur** (real vosita)

---

## 🎯 Sentabr natijasi

Siz **Junior Go Backend Dasturchi** deb aytishingiz mumkin, agar:

✅ REST API tuza olasiz  
✅ MySQL sxemalarini loyihalaysiz  
✅ JWT avtorizatsiyani joriy qilasiz  
✅ Concurrent dasturlar yaratasiz  
✅ Test yozasiz  
✅ Ilovani deploy qilasiz  
✅ Production xatolarni hal qilasiz  
✅ Arxitekturaviy qarorlaringizni tushuntira olasiz

---
