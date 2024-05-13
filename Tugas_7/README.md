# TUGAS 5

# Disusun Oleh

| NAMA | NRP |
| ---- | --- |
| [Leody Zelvon Herliansa](https://github.com/Leodyz)| 3122500010 | 

**DAFTAR ISI**

1. [Getting App into PWD](#getting-app-into-pwd-our-application)
2. [Updating Source Code](#updating-source-code-updating-our-application)
3. [Creating a repo](#creating-a-repo-sharing-our-application)
4. [Contain Filesystem](#contain-filesystem-persisting-our-db)
5. [Quick Volume Type Comparison](#quick-volume-type-comparison-using-bind-mounts)
6. [Container Networking](#container-networking-multi-container-apps)
7. [Installing Docker compose](#installing-docker-compose-using-docker-compose)


## getting App into PWD (Our Application)

**1. Download Zip (app.zip) drag n Drop dan Unzip**

![Unzip](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/1-1_unzip_app-zip.jpg)

**2. cd app/ vi Dockerfile**

![cd app/](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/1-2_cd-app.jpg)

![vi Dockerfile](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/1-3_vi.jpg)

**3. docker build**

![Docker Build](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/1-4_Dbuild.jpg)

**4. docker run**

![Docker run](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/1-5_Drun3000.jpg)

**5. Di cek**

![check](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/1-6_check.jpg)

## Updating Source Code (Updating Our Application)

**1. masuk Ke editor**

![Editor](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/1_editor.jpg)

![before](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/1_sebelum.jpg)

![after](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/1_sesudah.jpg)

**2. docker build**

![Dbuild](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/2-2_Dbuild.jpg)

**3. docker build (terjadi error)**

![DrunError](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/2-3_DrunError.jpg)

**4. docker stop, rm dan mulai lagi**

![DrunError](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/2-4_Drestart.jpg)

**5. Hasil**

![DrunError](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/2-5_hasil.jpg)

## Creating a repo (Sharing Our Application)

**1. masuk ke Dockerhub di Repository dan Create Repository**

![Create](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/3-1_create.jpg)
![Action](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/3-1_createAction.jpg)
![Hub](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/3-1_hub.jpg)

**2. Push image error (terjadi karena image tidak ditemukan)**

![Push Error](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/3-2_pushError.jpg)

**3. Lakukan Tag ke repo dan Push (acces dednied karena belum login)**

![Tag & Push Denied](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/3-3_tag&push(denied).jpg)

**4. login dan Push ulang**

![Login](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/3-4_login.jpg)
![Re-push](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/3-4_pushUlang.jpg)

**5. Run**

![Run](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/3-5_dockerRun(restartdlu).jpg)

  
## Contain FileSystem (persisting our DB)

**1. masuk ke Dockerhub di Repository dan Create Repository**

![RunUbuntu](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/4-1_DrunUbuntu.jpg)

**2. Eksekusi data.txt (harusnya mengeluarkan random number)**

![RunUbuntu](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/4-2_dockerExec.jpg)

**3. jalankan Ubuntu lain (data.txt tidak muncul)**

![RunUbuntu](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/4-3_ubuntuContainer.jpg)

**4. lakukan Docker rm -f <id>**

![RunUbuntu](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/4-4_Rmcontainer.jpg)

**Menggunakan Volume Create**

**1. Volume Create**

![VolumeCreate](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/4-5_volumecreate.jpg)

**2. Isi TODO**

![VolumeCreate](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/4-6_isiTODO.jpg)

**3. Stop Hapus Mulai ulang**

![VolumeCreate](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/4-7_stop-hapus-mulai.jpg)

**4. hasil reload**

![VolumeCreate](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/4-8_jalankanlagi.jpg)


## Quick Volume Type Comparison (Using Bind Mounts)

**STARTING DEV-MODE CONTAINER**

**1. pastikan semua docker-101 telah nonaktif**

![QuickVolume](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/5-1_mematikanDocker-101.jpg)
   
**2. Jalankan Script**

![QuickVolume](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/5-2_Script.jpg)

-dp 3000:3000: Flag ini menentukan pemetaan port, di mana port 3000 pada host dipetakan ke port 3000 pada kontainer.

-w /app: Ini mengatur direktori kerja di dalam kontainer menjadi /app, artinya semua perintah berikutnya akan dieksekusi dari direktori ini.

node:10-alpine: Ini adalah gambar Docker yang akan digunakan. Ini adalah gambar Node.js yang ringan berbasis Alpine Linux, yang sering digunakan untuk kontainerisasi karena ukurannya yang kecil.

sh -c "yarn install && yarn run dev": Perintah ini memulai sebuah shell (sh) di dalam kontainer dan kemudian menjalankan dua perintah yang dipisahkan oleh &&. Pertama, ia menjalankan yarn install untuk menginstal dependensi proyek yang ditentukan di package.json. Kemudian, ia menjalankan yarn run dev, yang biasanya memulai server pengembangan menggunakan nodemon, sebuah alat yang secara otomatis me-restart server ketika file berubah
    

**3. Buka Docker log**

![QuickVolume](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/5-3_dockerLogs.jpg)

**4. Edit file src/static/js/app.js di line 109**

![QuickVolume](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/5-4_before.jpg)

![QuickVolume](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/5-4_after.jpg)

**5. Hasil**

![QuickVolume](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/5-5_hasil.jpg)

*Feel free to make any other changes you'd like to make. When you're done, stop the container and build your new image using docker build -t docker-101 .


## Container Networking (Multi-Container Apps)

**Starting A SQL**

**1. create TODO app**

![Multi-Container Apps](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/6-1_networkCreate.jpg)

**2. Start dan Hubungkan Ke MY SQl (script)**

![Multi-Container Apps](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/6-2_startdanAttachMySQL.jpg)

**3. Masuk ke MYSQl**

![Multi-Container Apps](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/6-3_masukMYSQL.jpg)

**4. Show DATABASE**

![Multi-Container Apps](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/6-4_showdatabase.jpg)



**Connecting To MYSQl**

**1. menghubungkan ke nikolaka/netshoot**

![Multi-Container Apps](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/6-5_mencobamasukkenikolakanetshoot.jpg)

**2. dig mysql**

![Multi-Container Apps](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/6-6_digmySQL.jpg)


**lihat data (setelah Show Database)**

**1. lihat isi Item yang di input di TODO**

![Multi-Container Apps](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/6-7_lihat-isi-item.jpg)



## Installing Docker Compose (Using Docker Compose)

**1. melihat isi docker version dan membuat file Docker-compose.yml**

![Multi-Container Apps](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/7-1_Dockerver.jpg)

**2. Isi Docker-compose.yml**

![Multi-Container Apps](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/7-2_isi-Script.jpg)

**3. Docker compose**

![Multi-Container Apps](https://github.com/Leodyz/W-A-J/blob/main/Tugas_7/assets/7-3_docker-compose.jpg)



