# 06 - Variabel

**Pengertian Variabel** adalah identitas yang merepresentasikan lokasi pada memori untuk menyimpan nilai data selama program dijalankan. Dengan variabel, kita dapat memberi nama pada data, menyimpannya, dan mengolahnya sesuai kebutuhan program.

**Contoh:**

```java
public class variableExample {
    public static void main(String[] args) {

        // Deklarasi variabel tanpa inisialisasi
        String name;
        // Inisialisasi
        name = "Kiki Mahesta";

        System.out.println(name);

        // Deklarasi sekaligus inisialisasi
        int age = 21;
        String address = "Indonesia";

        System.out.println(age);
        System.out.println(address);

        // Mengubah data - otomatis yang dipakai data terakhir
        name = "Hana Rima"
        System.out.println(name);
    }
}
```

**Output:**

```
Kiki Mahesta
21
Indonesia
```

## Aturan Penamaan Variabel (Identifier)

1. Dimulai dengan huruf, underscore `_`, atau tanda dolar `$` (disarankan huruf).
2. Tidak boleh mengandung spasi.
3. Bersifat case-sensitive (`nama` ≠ `Nama`).
4. Gunakan camelCase untuk multi-kata: `nilaiAwal`, `jumlahSiswa`.
5. Hindari penggunaan kata kunci Java sebagai nama variabel.

## **Kata kunci Var**

- Sejak Java 10, dapat menggunakan `var` untuk inferensi tipe otomatis.
- Hanya bisa digunakan pada variabel lokal (di dalam method).

```java
public class varExample {
    public static void main(String[] args) {

        var class;// akan Error
        // dianggap String
        var name = "Kiki";

        // dianggap int
        var age = 21;

        System.out.println(name);
        System.out.println(age);
    }
}
```

**Output:**

```
Kiki
21
```

## **Kata kunci Final**

Dalam Java, setiap variabel secara default nilainya dapat diubah-ubah. Jika kita ingin membuat variabel yang nilainya tetap dan tidak boleh diubah setelah pertama kali diinisialisasi(konstan), gunakan kata kunci `final`. Variabel yang dideklarasikan `final` sering disebut juga konstanta.

```java
public class finalExample {
    public static void main(String[] args) {

        final String application = "Belajar AI"

        // bila ingin diubah akan Error
        application = "Belajar Java"

        System.out.println(application);
    }
}
```

**Output:**

```
Belajar AI
```
