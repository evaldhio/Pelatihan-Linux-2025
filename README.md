# Pelatihan-Linux-2025

1. Mengunduh program wget, unzip, dan xxd, lalu mempersiapkan sebuah folder baru bernama “artists_who_can_sing” dan masuk ke dalam folder tersebut.
```bash
sudo apt install wget unzip xxd && mkdir artists_who_can_sing && cd artists_who_can_sing
```
2. Mendownload file zip menggunakan wget
```bash
wget "https://drive.google.com/uc?export=download&id=1lV1HVmPTY_BOAK6ToXymRu7V5eVfR0ut" -O tutorials.zip
```
3. unzip ke dalam folder baru yang bernama “singing_tutorials”
```bash
mkdir singing_tutorials && unzip -d singing_tutorials tutorials.zip
```
4. masuk ke dalam folder "singing_tutorials" dan tampilkan list file yang tersembunyi
```bash
cd singing_tutorials && ls && ls -a
```
5. Cari file berisi "opera" oleh "NBAYoungboy", ambil link dalam FLAG{<tulisan>}, lalu simpan ke file bernama flag.txt di direktori "artists_who_can_sing"
```bash
find . -name "*opera*NBAYoungboy*" -exec grep -Ir "FLAG" {} \; > ../flag.txt
```
6. mundur satu folder, dan menggunakan link tersebut untuk download sebuah file baru dengan ketentuan nama “plsrunmeiamnotmalwarefr”
```bash
cd .. && wget "https://files.catbox.moe/9l4qu8" -O plsrunmeiamnotmalwarefr
```
7. Buatlah agar dapat izin untuk execute dan menjalankan program tersebut.
```bash
chmod +x plsrunmeiamnotmalwarefr
```
8. Jalankan menggunakan command di terminal linux.
```bash
./plsrunmeiamnotmalwarefr
```
9. Buat file bernama ransom.moolah, lalu periksa kembali untuk memastikan keberhasilannya.
```bash

