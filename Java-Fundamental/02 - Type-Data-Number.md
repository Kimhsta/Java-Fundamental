# 02 - Tipe Data Number

#### **Jenis Tipe Data Number di Java**

Java menyediakan beberapa tipe data numerik dasar:

- Integer Number (Bilangan Bulat)
- Floating Poin Number (Bilangan Pecahan/Desimal)

## **Integer Number**

| Tipe Data | Ukuran | Nilai Minimum              | Nilai Maksimum            |
| :-------- | :----- | :------------------------- | :------------------------ |
| `byte`    | 1 byte | -128                       | 127                       |
| `short`   | 2 byte | -32,768                    | 32,767                    |
| `int`     | 4 byte | -2,147,483,648             | 2,147,483,647             |
| `long`    | 8 byte | -9,223,372,036,854,775,808 | 9,223,372,036,854,775,807 |

## Contoh:

```java
public class IntegerNUmber {
    public static void main(String[] args) {
        byte iniByte = 100;
        short iniShort = 1000;
        int angka = 10000000;
        long iniLong = 1000000000;
        long iniLong2 = 1000000000L; //Khusus Long make L

        double desimal = 99.99;

        System.out.println(angka);
        System.out.println(desimal);
    }
}
```

**Output:**

```
10000000
99.99
```

---

## **Floating Point Number**

| Tipe Data | Ukuran | Nilai Minimum | Nilai Maksimum | Default |
| :-------- | :----- | :------------ | :------------- | ------- |
| `float`   | 4 byte | ~±1.4E-45     | ~±3.4E+38      | 0.0     |
| `double`  | 8 byte | ~±4.9E-324    | ~±1.7E+308     | 0.0     |

## Contoh:

```java
public class IntegerNumber {
    public static void main(String[] args) {
        float iniFloat = 10.10F;
        double iniDouble =10.10;

        System.out.println(iniFloat);
        System.out.println(iniDouble);
    }
}
```

**Output:**

```
10.1
10.1
```

---

## Literal

```java
public class Literal {
    public static void main(String[] args) {
        int decimalInt = 25; // Pecahan biasa
        int hexaDecimal = 0xFFFFF;     // Pecahan 16
        int binaryDecimal = 0b10101010;

        System.out.println(decimalInt);
        System.out.println(hexaDecimal);
        System.out.println(binaryDecimal);
    }
}
```

**Output:**

```
25
1048575
170
```

---

## Underscore

```java
public class Underscode {
    public static void main(String[] args) {
        long amount = 1_000_000_000;
        int sum = 60_000_000;



        System.out.println(amount);
        System.out.println(sum);
    }
}
```

**Output:**

```
1000000000
60000000
```

---

# Konversi Tipe Data Number

Dalam Java, konversi antar tipe data number dibagi menjadi dua jenis:

- **Widening Casting (Otomatis)**  
  Konversi dari tipe data kecil ke tipe data yang lebih besar:  
  `byte → short → int → long → float → double`

- **Narrowing Casting (Manual)**  
  Konversi dari tipe data besar ke tipe data yang lebih kecil:  
  `double → float → long → int → char → short → byte`
