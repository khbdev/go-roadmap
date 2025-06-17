
- Har bir oy alohida blok sifatida aniqlangan
- Har bir hafta uchun aniq mavzular to'liq tafsilotlari bilan keltirilgan
- Mavzular tartiblangan va chuqurlashtirilgan
- Amaliyotlar real loyiha yoki foydali CLI/Web dastur sifatida belgilangan
- Umumiy struktura yanada ravon, oson o'qish uchun formatlandi

---

# 🚀 Junior Go Backend Developer Uchun 3-Oylik Mukammal Roadmap

## 💡 Maqsad: 
3 oy davomida **Junior Go Backend Developer** darajasiga yetib borish, ya'ni:
- REST API yaratish
- JWT bilan auth
- MySQL, Redis, Docker bilan ishlash
- WebSocket, testlar yozish
- Mikroservis arxitekturasini tushunish
- Portfolio loyihalarini yaratish va GitHubda joylashtirish

---

# 🔵 1-OY: GO TILINING ASOSLARI VA CLI DASTURLAR

## ✅ 1-Hafta: Kirish va Til Asoslari

### Nazariya:
- Go o'rnatish (Go modullar tizimi, `go.mod`)
- O'zgaruvchilar, ma'lumot turlari (`int`, `string`, `bool`, `struct`)
- Operatorlar, `if/else`, `for`, `switch`
- Funksiya sintaksisi, parametrlar, qaytaruvchi qiymatlar
- Pointerlar, receiver funksiyalar
- Slice va massivlar bilan ishlash
- Maplar (kalit-qiymat juftligi)

### Amaliyot:
- Oddiy CLI kalkulyator dasturi
- JSON parsing (masalan, stringdan structga o'tkazish)

---

## ✅ 2-Hafta: Xatolar, Testlar, Interfeyslar

### Nazariya:
- `error` interfeysi va xatoliklarni boshqarish
- `panic`, `recover`, `defer` — xavfsiz kod yozish
- Interfeyslar orqali polimorfizm
- Unit testlar (`go test`, table-driven test)
- Test coverage nima va uning ahamiyati

### Amaliyot:
- Fayllarni o'qish/yozish CLI dasturi
- JSON parserga unit testlar yozish

---

## ✅ 3-Hafta: Gorutinalar, Kanallar, Parallel Ishlovchi Sistemalar

### Nazariya:
- Gorutina nima? `go func()` sintaksisi
- Kanallar: buffered/unbuffered kanallar
- `sync.WaitGroup`, `sync.Mutex`, `sync.RWMutex`
- Race condition va uni oldini olish
- Worker Pool modeli: gorutinani cheklash

### Amaliyot:
- Parallelni fayllarni o'qish/qayta ishlash dasturi
- Oddiy CLI chat (gorutina + kanal asosi)

---

## ✅ 4-Hafta: HTTP Server va Gin Framework Boshlang'ich Daraja

### Nazariya:
- `net/http` paketi bilan server yaratish
- Gin framework asoslari: router, handler, context
- Middleware: logging, recovery, authentication
- JSON marshaling/unmarshaling
- Request validatsiya (masalan, `go-playground/validator`)

### Amaliyot:
- Kitoblar CRUD API (GET, POST, PUT, DELETE)
- Logging middleware yozish

---

# 🔵 2-OY: WEB BACKEND + MYSQL + AUTHENTIKATSIYA

## ✅ 5-Hafta: SQL Asoslari va Go Integratsiyasi

### Nazariya:
- SQL asoslari: SELECT, INSERT, UPDATE, DELETE
- JOIN turlari (INNER, LEFT, RIGHT)
- GROUP BY, subquery, indexlar
- Go dan MySQL ga ulanish (`database/sql`, `go-sql-driver/mysql`)
- Migratsiya vositalari (`golang-migrate/migrate`)
- SQL injectionni oldini olish (prepared statements)

### Amaliyot:
- Foydalanuvchilar uchun CRUD API (MySQL bazasi)
- Auth API: register, login (parol hash qilish)

---

## ✅ 6-Hafta: JWT, Xavfsizlik, Rollar

### Nazariya:
- JWT token yaratish va tekshirish (`dgrijalva/jwt-go`)
- Token lifecycle: expire, refresh token mexanizmi
- CORS, CSRF, XSS, Rate Limiting tushunchalari
- Middleware orqali ro'yxatdan o'tish va rollarni tekshirish

### Amaliyot:
- Blog API: postlar ustida CRUD (JWT bilan himoyalangan)
- Admin va oddiy user rollari bilan kirish cheklovi

---

## ✅ 7-Hafta: Redis, Loglash, Konfiguratsiya

### Nazariya:
- Redis bilan ishlash (`go-redis`)
- Keshlash: tez-tez so'raladigan ma'lumotlarni saqlash
- Loglash vositalari: `logrus`, `zap`
- Konfiguratsiya: `.env`, `Viper` orqali sozlama yuklash
- Health Check, Graceful Shutdown

### Amaliyot:
- E-commerce API: mahsulotlar, savatcha, buyurtma
- Mahsulotlar uchun Redis keshi

---

# 🔵 3-OY: ISHLAB CHIQARISHGA TAYYORLIK + PORTFOLIO

## ✅ 8-Hafta: Docker, CI/CD, Deployment

### Nazariya:
- Dockerfile yozish: Go ilovalarini konteynerga joylash
- Docker Compose: bir nechta servislarni birlashtirish
- GitHub Actions bilan CI/CD pipeline yaratish
- Build pipeline: test → build → deploy
- Monitoring: Prometheus, Grafana integratsiyasi

### Amaliyot:
- Mikroservislar: user-service, product-service, order-service
- API Gateway bilan yagona kirish nuqtasi

---

## ✅ 9-Hafta: Loyiha #1 - Trello Kloni (REST API)

### Funktsiyalar:
- JWT bilan authentifikatsiya
- Tasklar: yaratish, o'zgartirish, o'chirish
- Boardlar, kolonkalar, cardlar
- MySQL orqali ma'lumot saqlash

---

## ✅ 10-Hafta: Loyiha #2 - URL Qisqartiruvchi

### Funktsiyalar:
- JWT bilan auth
- URL qisqartirish, statistikani ko'rish
- Redisda caching qilish
- MySQL bilan bog'lanish

---

## ✅ 11-Hafta: Loyiha #3 - Real-Time Chat

### Funktsiyalar:
- WebSocket orqali real-time aloqa
- Redis pub/sub orqali habar jo'natish/qabul qilish
- JWT bilan authentifikatsiya
- Room-based chat mexanizmi

---

## ✅ 12-Hafta: Intervyu Tuzoqlari, Rezyume, GitHub

### Nazariya:
- Texnik suhbat tayyorgarligi: algoritmlar, test topshiriqlari
- Arxitektura savollari: mikroservislar, cache, DB relatsiya
- GitHub profilini mustahkamlash (README, LICENSE, Dockerfile)
- Rezyume yozish (English hamda O'zbekcha)
- LeetCode / HackerRank masalalarini yechish

### Amaliyot:
- Portfolio loyihalarni GitHubga joylash
- README fayl yozish, loyihalarni tozalash
- Dockerfile, .gitignore qo'shish

---

# 📋 Har Kunlik Ish Rejasi (Maslahat Beriladi)

| Vaqt        | Faoliyat              |
| ----------- | --------------------- |
| 17:00–18:30 | Nazariya o‘rganish    |
| 18:30–20:30 | Kod yozish            |
| 20:30–22:00 | Loyihada ishlash      |
| 22:00–23:00 | Test yozish           |
| 23:00–00:00 | Forum, review, GitHub |

---

# 🎯 Yakuniy Natija (Sentabr Oyigacha Yetish Kerak):

✅ REST API yozish  
✅ JWT bilan authentifikatsiya  
✅ MySQL, Redis, Docker bilan ishlash  
✅ WebSocket bilan real-time aloqa  
✅ Test yozish (unit, integration)  
✅ Mikroservislar yaratish  
✅ GitHub portfolio tayyor  

Agar barcha amaliyotlarni bajarsangiz, siz "Junior Go Backend Developer" sifatida ishga kirishingiz mumkin!

---

# 📚 Tavsiya Etuvchan Manbalar:

- [https://go.dev](https://go.dev) – Rasmiy hujjatlar
- [https://gobyexample.com](https://gobyexample.com) – Praktik misollar
- **Kitob:** *Let's Go* by Alex Edwards – backend uchun ideal
- **YouTube:** Golang Dojo, Anthony GG – video darslar
- **LeetCode / HackerRank** – masala yechish

---

