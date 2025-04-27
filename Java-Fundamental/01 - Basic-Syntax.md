# 01 - Basic Syntax

## Struktur Program Java

```java
package com.example.app;

public class Main {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```

### Penjelasan:

- `package`: Mengelompokkan file Java ke dalam sebuah namespace.
- `public class Main`: Mendefinisikan class utama.
- `public static void main(String[] args)`: Method yang akan dieksekusi pertama kali saat program berjalan.
- `System.out.println`: Mencetak teks ke konsol.

---

## Package

- Package adalah cara mengatur file Java dalam struktur folder.
- Penulisan package harus diawali di bagian paling atas file.
- Nama package menggunakan huruf kecil.

Contoh:

```java
package com.example.myapp;
```

Jika berada di folder `src/com/example/myapp/Main.java`, maka baris package wajib ditulis.

---

## Class

- Java adalah bahasa pemrograman berbasis **class**.
- Nama file harus **sama** dengan nama `public class`.

Contoh:

```java
public class HelloWorld {
    // isi class
}
```

Disimpan dalam file `HelloWorld.java`.

---

## Method `main`

- Method `main` adalah titik awal program Java berjalan.
- Wajib menggunakan tanda tangan berikut:

```java
public static void main(String[] args)
```

Penjelasan kata kunci:

- `public`: Bisa diakses dari luar.
- `static`: Tidak membutuhkan objek untuk dijalankan.
- `void`: Tidak mengembalikan nilai.
- `String[] args`: Menerima parameter dari command line.

Contoh penggunaan parameter:

```java
public class App {
    public static void main(String[] args) {
        if (args.length > 0) {
            System.out.println("Hello " + args[0]);
        } else {
            System.out.println("Hello World");
        }
    }
}
```

---

## Best Practices

- Gunakan **camelCase** untuk nama variabel dan method.
- Gunakan **PascalCase** untuk nama Class.
- Gunakan **huruf kecil** untuk nama package.
- Simpan file di dalam folder yang sesuai dengan package.

Contoh struktur project:

```
src/
└── com/
    └── example/
        └── app/
            └── Main.java
```

- Selalu berikan komentar pada bagian penting kode.
- Gunakan JavaDoc untuk dokumentasi method dan class.

---
