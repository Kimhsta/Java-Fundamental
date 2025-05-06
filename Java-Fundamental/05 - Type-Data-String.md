# 05 - Tipe Data String

## Pengertian

- Tipe data **String** di Java digunakan untuk merepresentasikan urutan karakter (teks).
- Di Java, `String` adalah **kelas** (bukan tipe primitif) yang tersedia di `java.lang.String`.
- `String` bersifat **immutable**, artinya isi `String` tidak bisa diubah setelah dibuat.

---

## Deklarasi dan Inisialisasi

```java
public class StringExample {
    public static void main(String[] args) {
        String pesan = "Halo, Dunia!";
        String kosong = "";// nilai default null
        String gabungan = "Halo" + ", " + "Java";

        System.out.println(pesan);
        System.out.println(kosong);
        System.out.println(gabungan);
    }
}
```

**Output:**

```
Halo, Dunia!

Halo, Java
```

---

## Operasi Umum pada String

- **Concatenation** (penggabungan): menggunakan `+` atau `concat()`
- **Length**: `length()` untuk mendapatkan jumlah karakter
- **Substring**: `substring(beginIndex, endIndex)`
- **Equality**: `equals()` dan `equalsIgnoreCase()` untuk membandingkan konten
- **Contains**: `contains()` untuk memeriksa apakah teks tertentu ada di dalam String

### Contoh:

```java
public class StringOperations {
    public static void main(String[] args) {
        String s = "Java Programming";

        System.out.println("Length: " + s.length());
        System.out.println("Substring(0,4): " + s.substring(0, 4));
        System.out.println("Contains 'Pro': " + s.contains("Pro"));
        System.out.println("Uppercase: " + s.toUpperCase());
        System.out.println("Replace: " + s.replace("Java", "Kotlin"));
    }
}
```

**Output:**

```
Length: 16
Substring(0,4): Java
Contains 'Pro': true
Uppercase: JAVA PROGRAMMING
Replace: Kotlin Programming
```

---

## StringBuilder dan StringBuffer

- Untuk manipulasi teks yang sering diubah-ubah, gunakan `StringBuilder` (non-synchronized) atau `StringBuffer` (synchronized).
- Lebih efisien daripada membuat banyak objek `String` baru.

### Contoh StringBuilder:

```java
public class BuilderExample {
    public static void main(String[] args) {
        StringBuilder sb = new StringBuilder();
        sb.append("Halo");
        sb.append(", ");
        sb.append("StringBuilder");

        System.out.println(sb.toString());
    }
}
```

**Output:**

```
Halo, StringBuilder
```
