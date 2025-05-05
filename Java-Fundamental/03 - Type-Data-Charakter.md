# 03 - Tipe Data Character

**Pengertian**
**Tipe data `char`** di Java digunakan untuk merepresentasikan satu karakter Unicode. Ukuran `char` adalah 2 byte (16-bit), sehingga dapat menampung kode Unicode dari `\u0000` hingga `\uFFFF` (0 hingga 65.535).

## cContoh:

```java
public class charExample {
    public static void main(String[] args) {
        char huruf = 'A';            // literal karakter
        char angka = '1';            // karakter angka
        char unicode = '\u03A9';    // karakter Unicode (Omega)

        System.out.println(huruf);
        System.out.println(angka);
        System.out.println(unicode);
    }
}
```

**Output:**

```
A
1
Ω
```

## **Kelas Charakter**

Java menyediakan utility class `java.lang.Character` untuk operasi karakter:

| Method                     | Deskripsi                        |
| :------------------------- | :------------------------------- |
| `Character.isLetter(c)`    | Mengecek apakah `c` huruf        |
| `Character.isDigit(c)`     | Mengecek apakah `c` digit angka  |
| `Character.toUpperCase(c)` | Mengubah `c` menjadi huruf besar |
| `Character.toLowerCase(c)` | Mengubah `c` menjadi huruf kecil |

### **Contoh:**

```java
public class CharacterUtil {
    public static void main(String[] args) {
        char c1 = 'm';
        System.out.println(Character.isLetter(c1));
        System.out.println(Character.isDigit(c1));
        System.out.println(Character.toUpperCase(c1));
        System.out.println(Character.toLowerCase('A'));
    }
}
```

**Output:**

```
true
false
M
a
```
