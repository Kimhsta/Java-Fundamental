# Setup Lingkungan Java di Arch Linux

Berikut langkah-langkah mengatur lingkungan Java pada Arch Linux:

## 1. Perbarui Sistem

Pastikan paket sistem terkini:

```bash
sudo pacman -Syu
```

## 2. Instalasi JDK

Pasang OpenJDK dari repositori resmi:

```bash
sudo pacman -S jdk-openjdk
```

Verifikasi instalasi:

```bash
java -version
javac -version
```

## 3. Memasang IDE

Beberapa pilihan IDE populer:

- **VS Code**:
  ```bash
  sudo pacman -S code
  ```
- **IntelliJ IDEA Community Edition**:
  ```bash
  sudo pacman -S intellij-idea-community-edition
  ```

## 4. Konfigurasi Variabel Lingkungan (Opsional)

Jika diperlukan, tambahkan di `~/.bashrc` atau `~/.zshrc`:

```bash
export JAVA_HOME=/usr/lib/jvm/java-17-openjdk
export PATH=$PATH:$JAVA_HOME/bin
```

Kemudian muat ulang konfigurasi shell:

```bash
source ~/.bashrc   # atau source ~/.zshrc
```

