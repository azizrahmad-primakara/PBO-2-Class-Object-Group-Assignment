# 📘 README — Group Assignment Pertemuan 2

## 🎯 Tujuan

* Memahami perbedaan **Class** dan **Object**.
* Membuat class sederhana di Java dengan atribut dan method.
* Bekerja sama menggunakan **branching** dan **pull request** di GitHub.
* Menyusun program utama (`Main.java`) yang dapat **menggunakan semua class** dalam kelompok.

---

## 👥 Struktur Tim

* Setiap tim berisi **3–4 orang**.
* **Peran anggota:**

  * **Class Developer (semua anggota):** masing-masing membuat 1 class berbeda.
  * **Integrator (1 orang):** membuat `Main.java` untuk menggabungkan semua class.

---

## 🧩 Aturan Tema

Setiap kelompok punya **tema berbeda** (ditentukan dosen). Contoh tema:

* Kelompok 1 → **Inventory System**
* Kelompok 2 → **Human Resource**
* Kelompok 3 → **Library System**
* Kelompok 4 → **Course Management**
* Kelompok 5 → **E-Commerce**

Masing-masing anggota membuat class sesuai tema.
Contoh pada tema *Inventory System*:

* `Product.java`
* `Customer.java`
* `Order.java`

---

## 🌿 Workflow GitHub

1. **Accept assignment** via link:
   [👉 Klik untuk masuk GitHub Classroom](https://classroom.github.com/a/4D9ChwrC)
2. **Bentuk tim / gabung ke tim** (gunakan format nama tim yang ditentukan).
3. **Clone repo** ke komputer (pakai GitHub Desktop atau Git CLI).
4. **Buat branch baru** untuk class Anda:

   * Format: `feature/<NamaClass>`
   * Contoh: `feature/Product`, `feature/Customer`.
5. **Coding class Anda** di folder `src/main/java/`.
6. **Commit & Push** ke branch tersebut.
7. **Buat Pull Request (PR)** ke branch `main`.
8. **Review PR anggota lain** sebelum merge.
9. **Integrator:** setelah semua class merge, buat `Main.java` di branch `feature/integration-main`.
10. **Integrator** membuat PR terakhir untuk menggabungkan semua class di `Main`.

---

## 📝 Aturan Kode

* **Setiap class** harus memiliki:

  * Minimal 3 atribut `public`.
  * Minimal 1 method `info()` untuk menampilkan ringkasan data.
* **Contoh Class:**

  ```java
  public class Product {
      public String id;
      public String name;
      public double price;

      public String info() {
          return "[Product] " + id + " - " + name + " : " + price;
      }
  }
  ```
* **Main (oleh Integrator):**

  ```java
  public class Main {
      public static void main(String[] args) {
          Product p = new Product();
          p.id = "P001";
          p.name = "Keyboard";
          p.price = 150000;

          System.out.println(p.info());
          // Tambahkan pemanggilan class lain di sini...
      }
  }
  ```

⚠️ Catatan: atribut sengaja dibiarkan `public` → Minggu depan (Pertemuan 3) akan diubah ke `private` + getter/setter (enkapsulasi).

---

## ✅ Definition of Done (DoD)

* [ ] Tiap anggota membuat 1 class unik (branch + PR).
* [ ] Semua PR class sudah **approved & merged** ke `main`.
* [ ] Integrator berhasil membuat `Main.java` yang menggabungkan semua class.
* [ ] Repo memiliki `README.md` dengan: tema tim, pembagian tugas, cara menjalankan program.

---

## 📦 Struktur Repo

```
/src/main/java/<team>/
   Main.java        // dibuat integrator
   Product.java     // anggota 1
   Customer.java    // anggota 2
   Order.java       // anggota 3
   ...
README.md          // deskripsi tim & tema
```

---

## 🔎 Penilaian (10 poin tim)

* Desain & variasi class sesuai tema → **3 poin**
* Program dapat berjalan & Main menggabungkan semua class → **3 poin**
* Kolaborasi GitHub (branch, PR, review, merge) → **3 poin**
* README jelas & rapi → **1 poin**
