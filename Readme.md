
```markdown
# Proot Distro Management Script

Script ini membantu Anda mengelola distribusi Linux menggunakan `proot-distro` di Termux.

## Instalasi

### Prasyarat

1. Install Termux dari situs resminya atau melalui F-Droid.
2. Update paket dan install `proot-distro`:

   ```sh
   pkg update
   pkg install proot-distro -y
   ```

### Menggunakan Script

1. Simpan script berikut dengan nama `proot_distro.sh`.
2. Berikan izin eksekusi:

   ```sh
   chmod +x proot_distro.sh
   ```

3. Jalankan script dengan:

   ```sh
   ./proot_distro.sh
   ```

## Pilihan Menu

1. Install a distribution
2. List available distributions
3. Login to a distribution
4. Backup a distribution
5. Restore a distribution
6. Remove a distribution
7. Setup a distribution
8. Exit

## Cara Menginstal Distribusi

### Supported Distributions

- **Alpine Linux**
  - Alias: `alpine`
  - Comment: Rolling release branch (edge).

- **Arch Linux**
  - Alias: `archlinux`
  - Comment: Currently available only AArch64 and ARM ports.

- **Artix Linux**
  - Alias: `artix`
  - Comment: Currently available only for AArch64.

- **Debian (bookworm)**
  - Alias: `debian`
  - Comment: Stable release.

- **Debian (bullseye)**
  - Alias: `debian-oldstable`
  - Comment: Old stable release.

- **deepin**
  - Alias: `deepin`
  - Comment: Supports only 64-bit CPUs.

- **Fedora**
  - Alias: `fedora`
  - Comment: Version 39. Supports only 64-bit CPUs.

- **Manjaro**
  - Alias: `manjaro`
  - Comment: Currently available only for AArch64.

- **OpenKylin**
  - Alias: `openkylin`
  - Comment: Version 'nile'. Supports only 64-bit CPUs.

- **OpenSUSE**
  - Alias: `opensuse`
  - Comment: Rolling release (Tumbleweed).

- **Pardus**
  - Alias: `pardus`
  - Comment: Version 'yirmibir'. Not available for ARM 32 bit.

- **Ubuntu (24.04)**
  - Alias: `ubuntu`
  - Comment: LTS release (noble). Not available for x86 32-bit (i686) CPUs.

- **Ubuntu (22.04)**
  - Alias: `ubuntu-oldlts`
  - Comment: Previous LTS release (jammy). Not available for x86 32-bit (i686) CPUs.

- **Void Linux**
  - Alias: `void`

### Contoh Instalasi

#### Debian (bookworm)

Untuk menginstal Debian (bookworm), jalankan perintah berikut:

```sh
proot-distro install debian
```

Setelah instalasi selesai, Anda bisa login ke distribusi tersebut dengan perintah:

```sh
proot-distro login debian
```

### Menggunakan Script untuk Instalasi

Jalankan script `proot_distro.sh` dan pilih opsi yang sesuai untuk menginstal distribusi:

1. Pilih opsi `1` untuk "Install a distribution".
2. Masukkan alias distribusi yang ingin diinstal, misalnya `debian`.

```sh
./proot_distro.sh
```

Ikuti instruksi di layar untuk melanjutkan instalasi.

## Backup, Restore, Remove, dan Setup

Script ini juga mendukung opsi berikut:

- **Backup a distribution**
  - Pilih opsi `4` dan ikuti instruksi untuk melakukan backup.
  
- **Restore a distribution**
  - Pilih opsi `5` dan ikuti instruksi untuk melakukan restore dari file backup.

- **Remove a distribution**
  - Pilih opsi `6` untuk menghapus distribusi yang diinginkan.

- **Setup a distribution**
  - Pilih opsi `7` untuk melakukan setup distribusi yang diinginkan.

## Lisensi

Proot Distro Management Script dilisensikan di bawah [MIT License](LICENSE).
```

Simpan konten di atas dalam file bernama `README.md` dan upload ke repositori GitHub Anda bersama dengan script `proot_distro.sh`.
