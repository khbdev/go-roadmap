

# **4-haftalik Go Intensive Roadmap — Mustaqil Dasturchi uchun**

## **1-hafta — Go Syntax, Variables, Control Flow, Functions**

**Maqsad:** Go’ning barcha asosiy sintaksis va dasturlash qoidalarini o‘zlashtirish

| Kun | Mavzu                                               | Amaliy                                                     | Tekshiruv / Natija                   |
| --- | --------------------------------------------------- | ---------------------------------------------------------- | ------------------------------------ |
| 1   | Hello World, package main, func main(), go mod init | Hello World chop et, modul yarat, argument bilan print     | `go run main.go` → “Salom, Azizbek!” |
| 2   | Variables, types, constants                         | int, float, string, bool; 5 o‘zgaruvchi chop et            | Qiymatlar va tiplar to‘g‘ri chiqishi |
| 3   | If, Else, Switch                                    | Son musbat/manfiy/0 tekshiruvchi kod; hafta kuni chiqarish | Input 3 → “Chorshanba”               |
| 4   | For loop, Arrays                                    | 1-10 sonni chop etish, array → slice                       | 1..10 sonlar ketma-ket chop etilishi |
| 5   | Slice operations                                    | append, slicing, remove, copy                              | Elementlar kutilgan tartibda         |
| 6   | Map                                                 | map[string]int, existence check                            | “hello” → h:1 e:1 l:2 o:1            |
| 7   | Functions                                           | func, multiple returns, defer                              | SumAndDiff(5,3) → 8,2                |

---

## **2-hafta — Structs, Methods, Packages, File I/O, Error Handling**

**Maqsad:** OOP, modular kod, file va error handling

| Kun | Mavzu                              | Amaliy                                           | Tekshiruv / Natija                   |
| --- | ---------------------------------- | ------------------------------------------------ | ------------------------------------ |
| 8   | Struct                             | User struct yaratish, chop etish                 | User First/Last/Age to‘g‘ri chiqishi |
| 9   | Methods (value & pointer receiver) | FullName() & Birthday()                          | Birthday chaqirilgach Age oshishi    |
| 10  | Nested structs, Slice of structs   | 3 user slice, Address struct qo‘shish            | Barcha userlar chiqarilishi          |
| 11  | Package yaratish                   | mathutils: Add, Sub, test yozish                 | main.go dan import qilganda ishlash  |
| 12  | Multiple files, project structure  | utils.go, store.go, main.go bilan CLI app        | `go run .` → buyruqlar ishlaydi      |
| 13  | File I/O basics                    | users slice → JSON → faylga yozish, qayta o‘qish | Fayl to‘g‘ri JSON, struct tiklanishi |
| 14  | Error handling                     | error type, if err != nil                        | Noto‘g‘ri path → xato chiqishi       |

---

## **3-hafta — Concurrency (Goroutines, Channels, Select, Fan-in/Out)**

**Maqsad:** Go’ning parallel ishlash qudratini o‘rganish

| Kun | Mavzu                       | Amaliy                                       | Tekshiruv / Natija                                    |
| --- | --------------------------- | -------------------------------------------- | ----------------------------------------------------- |
| 15  | Goroutines basics           | 10 goroutine yaratib, 1s kutib print         | Hammasi tugashi va ketma-ket chiqishi                 |
| 16  | WaitGroup & Mutex           | 100 goroutine counter++; mutex bilan xavfsiz | Oxirgi counter to‘g‘ri chiqishi                       |
| 17  | Channels (unbuffered)       | producer → channel → consumer                | Consumer barcha qiymatlarni oladi                     |
| 18  | Buffered channels & closing | make(chan int,5), close(ch)                  | Range bilan barcha qiymatlar o‘qilishi, deadlock yo‘q |
| 19  | Select + timeout            | 2 channel + time.After                       | Maʼlumot kelmasa timeout ishlaydi                     |
| 20  | Fan-in/Fan-out              | 3 producer, 1 consumer aggregator            | Aggregator barcha 15 itemni oladi                     |
| 21  | Mini concurrency project    | Parallel URL pinger yoki task runner         | Barcha tasklar bajarilgan va natija to‘g‘ri           |

---

## **4-hafta — HTTP, API, Database, Yakuniy Mini Loyiha**

**Maqsad:** Backend va full-stack Go mustaqil loyiha

| Kun | Mavzu                      | Amaliy                                                   | Tekshiruv / Natija                         |
| --- | -------------------------- | -------------------------------------------------------- | ------------------------------------------ |
| 22  | HTTP basics                | /hello, /ping JSON                                       | curl localhost:8080/ping → `{status:"ok"}` |
| 23  | POST endpoint + JSON       | /sum POST: {"a":2,"b":3} → {"sum":5}                     | JSON natija to‘g‘ri                        |
| 24  | URL params & router        | /user?id=2                                               | In-memory user JSON qaytadi                |
| 25  | Database/sql introduction  | SQLite/MySQL, `sql.Open`                                 | DB ochilishi va INSERT/SELECT ishlashi     |
| 26  | CRUD endpoints             | POST/GET/PUT/DELETE users                                | CRUD endpointlar ishlaydi                  |
| 27  | Background tasks & testing | Goroutine reminder + unit tests                          | Background ishlaydi, tests muvaffaqiyatli  |
| 28  | Yakuniy mini-loyiha        | Todo API (HTTP + DB + concurrency + file backup + tests) | Barcha endpointlar ishlashi, tests o‘tishi |

---

