# 02 - Tipe Data Number

## Jenis Tipe Data Number di Java

Java menyediakan beberapa tipe data numerik dasar:

- Integer Number (Bilangan Bulat)
- Floating Poin Number (Bilangan Pecahan/Desimal)

# Integer Number

| Tipe Data | Ukuran | Nilai Minimum              | Nilai Maksimum            |
| :-------- | :----- | :------------------------- | :------------------------ |
| `byte`    | 1 byte | -128                       | 127                       |
| `short`   | 2 byte | -32,768                    | 32,767                    |
| `int`     | 4 byte | -2,147,483,648             | 2,147,483,647             |
| `long`    | 8 byte | -9,223,372,036,854,775,808 | 9,223,372,036,854,775,807 |

# Floating Point Number

| Tipe Data | Ukuran | Nilai Minimum | Nilai Maksimum | Default |
| :-------- | :----- | :------------ | :------------- | ------- |
| `float`   | 4 byte | ~±1.4E-45     | ~±3.4E+38      | 0.0     |
| `double`  | 8 byte | ~±4.9E-324    | ~±1.7E+308     | 0.0     |

## Contoh Penggunaan Tipe Data Number

```java
public class NumberExample {
    public static void main(String[] args) {
        int angka = 100;
        
        double desimal = 99.99;

        System.out.println(angka);
        System.out.println(desimal);
    }
}
```

**Output:**

```
100
99.99
```

---

## Literal Bilangan di Java

```java
public class LiteralExample {
    public static void main(String[] args) {
        int binary = 0b1010; // 10 dalam desimal
        int octal = 012;     // 10 dalam desimal
        int hexa = 0xA;      // 10 dalam desimal

        System.out.println(binary);
        System.out.println(octal);
        System.out.println(hexa);
    }
}
```

**Output:**

```
10
10
10
```

---

## Casting Number

```java
public class CastingExample {
    public static void main(String[] args) {
        int angkaInt = 10;
        double angkaDouble = angkaInt; // otomatis

        double nilai = 9.7;
        int nilaiInt = (int) nilai; // manual

        System.out.println(angkaDouble);
        System.out.println(nilaiInt);
    }
}
```

**Output:**

```
10.0
9
```

---

# Selesai untuk Tipe Data Number ✅
