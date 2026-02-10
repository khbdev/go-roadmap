

# 📅 11-FEVRAL — 20-MART (KUNMA-KUN)

## FEVRAL

### **11-fevral — Slice start**

**25m tushunish:** slice, `len`, `append`, index
**25m daftarga code:**

* `nums := []int{}`
* `Add(num int)` (append)
* `PrintAll()` (for loop)

---

### **12-fevral — Struct**

**25m tushunish:** `struct`, field, init (literal)
**25m daftarga code:**

* `type User struct { ID int; Name string; Email string }`
* 2 ta user yaratib print

---

### **13-fevral — Slice + Struct**

**25m tushunish:** `[]User`, loop bilan qidirish
**25m daftarga code:**

* `users := []User{}`
* `AddUser(u User)`
* `ListUsers() []User`

---

### **14-fevral — Kichik funksiyalar**

**25m tushunish:** funksiyani mayda bo‘lak qilish (SRP)
**25m daftarga code:**

* `FindByID(id int) (User, bool)`
* `FindIndexByID(id int) int` (topmasa `-1`)

---

### **15-fevral — Delete (slice remove)**

**25m tushunish:** slice’dan o‘chirish pattern: `append(a[:i], a[i+1:]...)`
**25m daftarga code:**

* `DeleteByID(id int) bool` (o‘chsa true)

---

### **16-fevral — Map**

**25m tushunish:** `map`, `ok` idiom, qachon map kerak
**25m daftarga code:**

* `byEmail := map[string]User{}`
* `AddToMap(u User)`
* `GetByEmail(email string) (User, bool)`

---

### **17-fevral — Error**

**25m tushunish:** `error`, `errors.New`, `fmt.Errorf`, return err
**25m daftarga code:**

* `GetByID(id int) (User, error)`
* `ErrNotFound := errors.New("user not found")`

---

### **18-fevral — Pointer qachon kerak**

**25m tushunish:** pointer update, value vs reference
**25m daftarga code:**

* `UpdateName(id int, name string) error`
* `UpdateEmail(id int, email string) error`
  (Topilganda `users[i].Name = name`)

---

### **19-fevral — Interface**

**25m tushunish:** interface, abstraction, nega kerak
**25m daftarga code:**

* `type UserStorage interface { Add(User) error; Delete(int) error; Get(int)(User,error); List()([]User,error) }`

---

### **20-fevral — InMemory implement**

**25m tushunish:** interface implement, struct storage
**25m daftarga code:**

* `type InMemoryStorage struct { users []User }`
* interface methodlarini yozib chiq

---

### **21-fevral — File save (text)**

**25m tushunish:** file write basics (`os.Create`, `defer Close`)
**25m daftarga code:**

* `SaveToFile(path string) error`
* format: `id|name|email\n`

---

### **22-fevral — File load (text)**

**25m tushunish:** file read (`os.Open`, scanner)
**25m daftarga code:**

* `LoadFromFile(path string) error`
* parse qilib `users`ni to‘ldir

---

### **23-fevral — JSON encode/decode**

**25m tushunish:** `encoding/json`, tag `json:"name"`
**25m daftarga code:**

* `SaveJSON(path string) error` (usersni JSON qilib yoz)
* `LoadJSON(path string) error`

---

### **24-fevral — CLI (os.Args)**

**25m tushunish:** CLI command pattern: `add/list/get/delete`
**25m daftarga code:**

* `main()`da: `add`, `list`, `get`, `delete`
* usage chiqarsin

---

### **25-fevral — Mini yakun: user-manager**

**25m tushunish:** hammasini bir flowga keltirish
**25m daftarga code:**

* `user-manager` ishlaydigan demo:

  * add 2 user
  * list
  * save/load
  * delete

---

## HTTP BLOK (Backendni his qilish)

### **26-fevral — HTTP server start**

**25m tushunish:** `net/http`, handler nima
**25m daftarga code:**

* `GET /ping` → “pong”

---

### **27-fevral — Request/Response**

**25m tushunish:** query params, `r.URL.Query()`
**25m daftarga code:**

* `GET /echo?msg=salom` → JSON `{ "msg": "salom" }`

---

### **28-fevral — Status code**

**25m tushunish:** `w.WriteHeader`, `http.Status...`
**25m daftarga code:**

* `GET /users?id=1`

  * topilsa `200` + JSON
  * topilmasa `404`

---

## MART

### **1-mart — POST JSON body**

**25m tushunish:** `json.NewDecoder(r.Body).Decode(&x)`
**25m daftarga code:**

* `POST /users` body: `{name,email}`
* response: created user JSON

---

### **2-mart — Validation**

**25m tushunish:** minimal validation: empty, email contains `@`
**25m daftarga code:**

* `POST /users`

  * name/email bo‘sh bo‘lsa `400` + error JSON

---

### **3-mart — Router (oddiy)**

**25m tushunish:** `http.HandleFunc` bilan path ajratish
**25m daftarga code:**

* `/users` (GET/POST)
* `/users/` bilan id parse (soddaroq: query bilan ham bo‘ladi)

---

### **4-mart — Storage’ni HTTPga ulash**

**25m tushunish:** handler ichida storage ishlatish
**25m daftarga code:**

* `GET /users` → list
* `POST /users` → add
  (InMemoryStorage)

---

## DATABASE BLOK

### **5-mart — SQL tushunchasi**

**25m tushunish:** table, primary key, insert/select/update/delete
**25m daftarga code:**

* daftarda schema yoz: `users(id SERIAL PK, name, email)`
* SQL: INSERT va SELECT misol

---

### **6-mart — database/sql connect (kod skeleti)**

**25m tushunish:** `sql.Open`, `db.Ping`
**25m daftarga code:**

* `ConnectDB(dsn string) (*sql.DB, error)`
* `Ping` tekshir

---

### **7-mart — INSERT user**

**25m tushunish:** `Exec`, `QueryRow` + returning id (DBga bog‘liq)
**25m daftarga code:**

* `CreateUser(name,email) (int, error)`

---

### **8-mart — SELECT by id**

**25m tushunish:** `QueryRow().Scan()`
**25m daftarga code:**

* `GetUser(id int) (User, error)`

---

### **9-mart — SELECT list**

**25m tushunish:** `rows.Next()` loop
**25m daftarga code:**

* `ListUsers() ([]User, error)`

---

### **10-mart — UPDATE**

**25m tushunish:** update + affected rows
**25m daftarga code:**

* `UpdateUser(id, name, email) error`

---

### **11-mart — DELETE**

**25m tushunish:** delete + not found holati
**25m daftarga code:**

* `DeleteUser(id int) error`

---

### **12-mart — HTTP + DB CRUD birlashtirish**

**25m tushunish:** handler → repository (db)
**25m daftarga code:**

* `GET /users?id=` DBdan
* `POST /users` DBga
  (status code to‘g‘ri)

---

## CONCURRENCY BLOK (Go kuchi)

### **13-mart — Goroutine**

**25m tushunish:** goroutine nima, qachon ishlatiladi
**25m daftarga code:**

* 3 ta goroutine “job” print qilsin
* main tugab ketmasin (sleep yoki wg keyinroq)

---

### **14-mart — WaitGroup**

**25m tushunish:** `wg.Add`, `wg.Done`, `wg.Wait`
**25m daftarga code:**

* 5 job parallel
* wg bilan kutib yakunla

---

### **15-mart — Channel**

**25m tushunish:** send/receive, blocking
**25m daftarga code:**

* producer: 1..10 yuboradi
* consumer: yig‘indisini chiqaradi

---

### **16-mart — Worker pool (channel + wg)**

**25m tushunish:** job queue + N worker
**25m daftarga code:**

* `jobs chan int`
* 3 worker jobni `square` qilib `results`ga tashlasin

---

### **17-mart — Mutex**

**25m tushunish:** race condition, `sync.Mutex`
**25m daftarga code:**

* `counter++` ni 1000 marta parallel
* mutex bilan to‘g‘rilash

---

### **18-mart — Parallel ishlash (real)**

**25m tushunish:** parallel file/process ideyasi
**25m daftarga code:**

* `[]string` (log lines)
* 4 worker `map[string]int` count (mutex bilan birlashtir)

---

## REAL TASKLAR (intervyuda “mana task” bosqichi)

### **19-mart — URL Shortener (mini)**

**25m tushunish:** shortener: longURL → code, redirect
**25m daftarga code:**

* `map[string]string` (code→url)
* `POST /shorten` → code qaytar
* `GET /r?code=...` → redirect (`302`)

---

### **20-mart — 3ta Real Task (mini)**

**25m tushunish:**

* Rate limiter nima (per IP/ per second)
* In-memory queue nima
* Worker system nima

**25m daftarga code (skelet + ishlaydigan mini):**

1. **Rate limiter (soddasi):**

   * `map[string]int` + `time.Now().Unix()`
   * 1 sekundda 5 tadan oshsa `429`
2. **In-memory queue:**

   * `type Queue struct { items []int; mu sync.Mutex }`
   * `Enqueue`, `Dequeue`
3. **Worker system:**

   * queue’dan job olib worker bajaradi (channel + wg)

---

