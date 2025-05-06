# 04 - Tipe Data Boolean

**Pengertian Tipe Data Boolean** adalah tipe data yang hanya memiliki dua kemungkinan nilai, yaitu `true` (benar) dan `false` (salah). Tipe data ini sangat berguna untuk pengambilan keputusan (percabangan) dalam program.

Di dalam bahasa pemrograman **Java**, tipe data boolean direpresentasikan dengan kata kunci `boolean`, dan nilai default dari tipe data ini adalah `false` jika tidak diinisialisasi secara eksplisit.

---

## Contoh:

```java
public class BooleanExample {
    public static void main(String[] args) {
        boolean mahesPintar = true;
        boolean mahesMalas = false;

        System.out.println("Apakah Mahes Pintar? " + mahesPintar);
        System.out.println("Mahes Pemalas? " + mahesMalas);
    }
}
```

**Output:**

```
Apakah Mahes Pintar? true
Mahes Pemalas? false
```

---

## Operasi Logika dengan Boolean

Tipe data boolean sangat sering digunakan dalam operasi logika, seperti:

- `&&` (AND): akan bernilai `true` jika **kedua** operand bernilai `true`.
- `||` (OR): akan bernilai `true` jika **salah satu** operand bernilai `true`.
- `!` (NOT): membalikkan nilai boolean.

### Contoh:

```java
public class BooleanLogic {
    public static void main(String[] args) {
        boolean a = true;
        boolean b = false;

        System.out.println(a && b);  // false
        System.out.println(a || b);  // true
        System.out.println(!a);      // false
    }
}
```

**Output:**

```
false
true
false
```
