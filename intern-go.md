
---

## 🗓 3 OYLIK (12 HAFTALIK) REAL JUNIOR GO BACKEND DEVELOPER ROADMAP

### 🎯 Maqsad:
Oxirgi oy oxirida **CRUD API** bilan to'la ishlaydigan backend loyiha yaratish, uni deploy qilish va GitHubda o'z portfolio sifatida namoyish etish.

---

## 🗓 1–2-HAFTA: OS, INTERNET VA ASOSIY TUSHUNCHALAR

✅ **Keraklilik**: Backend dasturchi server bilan ishlashi kerak. Buning uchun Linux asoslari muhim.

- ✅ **Linux / Terminal**:
  - Fayl sistemasi (`/home`, `/etc`, `/var`)
  - Terminal komandalar: `ls`, `cd`, `mkdir`, `rm`, `cp`, `mv`, `cat`, `nano`
  - `grep`, `ps`, `top`, `chmod`, `chown`
- ✅ **Backend nima?**
  - Client-server modeli
  - HTTP/HTTPS, portlar, TCP vs UDP (soddaroq misollar bilan)
- ✅ **HTTP protokoli**:
  - GET, POST, PUT, DELETE
  - Status kodlar: 200, 404, 500, 400, 401, 403
- ✅ **REST API & JSON**:
  - RESTning ma’nosi, resurslar ustida CRUD
  - JSON formati: obyekt, massiv, kalit-qiymat
- ✅ **Git & GitHub**:
  - Git o’rnatish, `git config --global`
  - `init`/`clone`, `add`, `commit`, `push`, `pull`
  - `.gitignore`, `README.md`, branch boshqaruvi (`main` → `dev` → `feature`)
  - GitHub repo yaratish, commit history ko'rish

💡 **Amaliyot**: Oddiy HTML + static server (masalan, Python bilan) so'rash orqali HTTP so'rovni tekshirish.

---

## 🗓 3–4-HAFTA: GO SINTAKSISI VA ASOSLAR

✅ **Keraklilik**: Backend logikani yozish uchun tilni mukammal bilish kerak.

- ✅ **Go o’rnatish**:
  - `go version`, `go env`
  - `go mod init`, `go run`, `go build`
- ✅ **Asosiy sintaksis**:
  - `package main`, `import`, `fmt.Println`, `func main()`
- ✅ **O‘zgaruvchilar va tur aniqlash**:
  - `var`, `:=`, tur uzatish
- ✅ **Boshqaruv strukturalari**:
  - `if`, `else if`, `else`
  - `for` loop (faqat bitta shart bilan ham)
  - `switch` (case, default)
- ✅ **Tur tizimi**:
  - `int`, `string`, `bool`, `float64`, `byte`, `rune`
- ✅ **Funksiyalar**:
  - Parametrlar, return qiymatlar
  - Nomlangan return (named return values)

💡 **Amaliyot**: Konsol ilovasi — masalan, "To-do list"ni faqat konsolda ishlatish.

---

## 🗓 5–6-HAFTA: MA'LUMOT TUZILMALARI VA XATOLIK BOSHQARUVI

✅ **Keraklilik**: Backendda ma'lumotlar bilan ishlash eng muhim qism.

- ✅ **Array**, **Slice**, **Map**:
  - Yaratish, o'zgartirish, iteratsiya
  - `append`, `make`, `len`, `cap`
- ✅ **Struct**:
  - Maydonlar, nesting, metodlar
- ✅ **Error handling**:
  - `error` interfeysi
  - `errors.New`, `fmt.Errorf`
  - `panic` va `recover` haqiqiy xatolik holatlari uchun
- ✅ **Package yaratish**:
  - Alohida faylda funksiyalar yozish, import qilish

💡 **Amaliyot**: Foydalanuvchi ma'lumotlarini saqlash uchun struct yaratish va slice ichida ularga CRUD amaliyotlarini qo'llash.

---

## 🗓 7–8-HAFTA: HTTP SERVER VA JSON INTEGRATSIYA

✅ **Keraklilik**: Backend server yaratish imkonini beradi.

- ✅ **`net/http` paketi**:
  - `http.HandleFunc`, `http.ListenAndServe`
  - Routing, handler funksiya yaratish
- ✅ **Query params, path params**:
  - `r.URL.Query()`, `mux.Vars()` (mux routerdan keyin)
- ✅ **JSON marshaling/unmarshaling**:
  - `json.Marshal`, `json.Unmarshal`
- ✅ **In-memory CRUD API**:
  - `GET /items`
  - `POST /items`
  - `GET /items/{id}`
  - `PUT /items/{id}`
  - `DELETE /items/{id}`

💡 **Amaliyot**: Postman yoki curl bilan test qilish.

---

## 🗓 9–10-HAFTA: MYSQL INTEGRATSIYA

✅ **Keraklilik**: Real backendda ma'lumotlarni saqlash uchun DB kerak.

- ✅ **MySQL o’rnatish**:
  - Ubuntu/MacOS uchun `mysql-server` o'rnatish
  - CLI bilan ishlash: `mysql -u root -p`
- ✅ **SQL asoslari**:
  - `SELECT`, `INSERT`, `UPDATE`, `DELETE`
  - `JOIN`, `WHERE`, `ORDER BY`, `LIMIT`
- ✅ **Database schema yaratish**:
  - Jadval yaratish, primary key, foreign key
- ✅ **Go’da DB integratsiya**:
  - `database/sql` paketi
  - MySQL driver: `github.com/go-sql-driver/mysql`
  - `sql.DB`, `QueryRow`, `Exec`, `Prepare`
- ✅ **Migrations**:
  - Oddiy `.sql` fayllar bilan migratsiya qilish
- ✅ **CRUD API’ni DB ga ulash**:
  - Oldingi “items” misolini MySQL bilan qayta yozish

💡 **Amaliyot**: Items jadvalini yaratish va Postman orqali API ni test qilish.

---

## 🗓 11-HAFTA: CONCURRENCY VA TESTING

✅ **Keraklilik**: Hozirdagi backend so'rovlarni parallel qabul qilishi kerak.

- ✅ **Goroutine**:
  - `go func()` bilan yaratish
  - Sync goroutinelar: `sync.WaitGroup`
- ✅ **Channel’lar**:
  - `chan int`, send/receive
  - Buffered vs unbuffered channel
- ✅ **Select statement**:
  - Bir nechta channellarni kuzatish
- ✅ **Unit testing**:
  - `testing` paketi
  - Table-driven testlar
- ✅ **Mocking DB**:
  - Interface yordamida fake DB yaratish

💡 **Amaliyot**: Goroutine bilan birga 10 ta requestni paralel jo'natish.

---

## 🗓 12-HAFTA: LOYIHA TUZILISHI, CONFIGURATION VA DEPLOY

✅ **Keraklilik**: Ishlab chiqilgan loyihani serverga joylash kerak.

- ✅ **Project structure**:
  - `cmd/` — main funksiya
  - `internal/` — biznes logika
  - `pkg/` — umumiy foydalaniladigan paketlar
- ✅ **Configuration**:
  - `.env` fayli, `godotenv` bilan yuklash
- ✅ **Logging**:
  - `log` paketi yoki `logrus` bilan level based logging
- ✅ **Build & Deploy**:
  - `go build` → binarni yaratish
  - Serverga joylash (Ubuntu VPS)
  - `systemd` servis yaratish
  - MySQL service bilan bog'lash
- ✅ **README.md**:
  - Loyiha tavsifi
  - Qanday ishga tushirish
  - API dokumentatsiya (masalan, Swagger emas, lekin oddiy izohlar bilan)

💡 **Amaliyot**: DigitalOcean, Linode yoki AWS Free Tier’dagi serverga deploy qilish.

---

## ✨ Natija (3 oy oxirida):

- ✅ To'liq ishlaydigan CRUD API yaratishingiz mumkin.
- ✅ GitHubda o'z loyihangiz bor bo'ladi.
- ✅ Go tilini mukammal bilasiz.
- ✅ MySQL bilan ishlashingiz mumkin.
- ✅ Testing, concurrency, deploy jarayonlarini o'zlashtirasiz.

---

## 📌 Takliflar:

- ✅ Har bir haftaning oxirida **mini-loyiha** yaratish.
- ✅ GitHub profiliga loyiha qo'shish, **portfolio** sifatida foydalanish.
- ✅ Telegram bot, Docker, Swagger kabi narsalarni keyingi bosqichda o'rganish.

---

