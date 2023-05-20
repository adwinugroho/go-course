# OS X
- download di https://go.dev/dl/
1. Bila pakai Intel processor
    - cari yang go1.20.4.darwin-amd64.pkg (x86-64)
    - langsung di klik saja ketika download telah usai dan ikutin perintah-perintah installernya sampai selesai
2. Bila pakai Apple Silicon Chip
    - cari yang go1.20.4.darwin-arm64.pkg (ARM64)
    - langsung di klik saja ketika download telah usai dan ikutin perintah-perintah installernya sampai selesai

- Untuk verifikasi apakah sudah terinstall atau belum ketikkan perintah
    - go version

# Linux (ubuntu)
1. Bila sudah install **snap**, bisa dengan mudah pakai perintah:
    - sudo snap install go --classic
2. Ketikkan perintah, untuk menginstall GoLang versi terbaru
    - sudo apt-get update
    - sudo apt-get upgrade
    - sudo apt search golang-go
    - sudo apt search gccgo-go
    - sudo apt install golang-go
3. Cara ketiga yakni download langsung di https://go.dev/dl/ cari yang versinya senada dengan OS yang kamu punya, lalu masuk ke terminal di folder di mana kamu men-download GoLang tadi lalu ketikan perintah
    - sudo tar -xvf go1.20.4.linux-amd64.tar.gz
    - lalu cek di folder itu harusnya ada folder baru bernama "go"
    - pindahkan folder "go" tersebut ke /usr/local
        - bisa dengan perintah sudo mv go /usr/local
    - selanjutnya kita set environment-nya dengan menambahkan global variabel ke dalam file ".bashrc" atau ".profile" dengan perintah
        - sudo nano ~/.bashrc
        - scroll sampai paling bawah dan tambahkan ini di baris paling akhir
        ```bash
        # Go Global variables
        export GOROOT=/usr/local/go
        export GOPATH=$HOME/go
        export PATH=$GOPATH/bin:$GOROOT/bin:$PATH
        ```
        - lalu ketikkan perintah
            - source ~/.bashrc

- Untuk verifikasi apakah sudah terinstall atau belum ketikkan perintah
    - go version

# Windows
- Download di https://go.dev/dl/ cari installer untuk Windows OS sesuai dengan tipe OS-nya masing-masing jika 64bit maka cari arch x86-64 apabila 32bit cari arch x86, jalankan installer dan ikuti perintahnya sampai selesai secara otomatis GoLang akan terinstall di "C:\go" dan go path akan otomatis terdaftar di environment variable.

- Untuk verifikasi apakah sudah terinstall atau belum ketikkan perintah
    - go version