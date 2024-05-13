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

![Unzip](/assets/1-1_unzip_app-zip)

**2. cd app/ vi Dockerfile**

![cd app/](/assets/1-2_cd-app)

![vi Dockerfile](/assets/1-3_vi)

**3. docker build**

![Docker Build](/assets/1-4_Dbuild)

**4. docker run**

![Docker run](/assets/1-5_drun3000)

**5. Di cek**

![check](/assets/1-6_check)

## Updating Source Code (Updating Our Application)

**1. masuk Ke editor**

![Editor](/assets/1_editor)

![before](/assets/1_sebelum)

![after](/assets/1_sesudah)

**2. docker build**

![Dbuild](/assets/2-2_Dbuild)

**3. docker build (terjadi error)**

![DrunError](/assets/2-3_DrunError)

**4. docker stop, rm dan mulai lagi**

![DrunError](/assets/2-4_Drestart)

**5. Hasil**

![DrunError](/assets/2-5_hasil)

## Creating a repo (Sharing Our Application)

**1. masuk ke Dockerhub di Repository dan Create Repository**

![Create](/assets/3-1_create)
![Action](/assets/3-1_createAction)
![Hub](/assets/3-1_hub)

**2. Push image error (terjadi karena image tidak ditemukan)**

![Push Error](/assets/3-2_pushError)

**3. Lakukan Tag ke repo dan Push (acces dednied karena belum login)**

![Tag & Push Denied](/assets/3-3_tag&push(denied))

**4. login dan Push ulang**

![Login](/assets/3-4_login)
![Re-push](/assets/3-4_pushUlang)

**5. Run**

![Run](/assets/3-5_dockerRun(restartdlu))

  
## Contain FileSystem (persisting our DB)

**1. masuk ke Dockerhub di Repository dan Create Repository**

![RunUbuntu](/assets/4-1_DrunUbuntu)

**2. Eksekusi data.txt (harusnya mengeluarkan random number)**

![RunUbuntu](/assets/4-2_dockerExec)

**3. jalankan Ubuntu lain (data.txt tidak muncul)**

![RunUbuntu](/assets/4-3_ubuntuContainer)

**4. lakukan Docker rm -f <id>**

![RunUbuntu](/assets/4-4_Rmcontainer)

**Menggunakan Volume Create**

**1. Volume Create**

![VolumeCreate](/assets/4-5_volumecreate)

**2. Isi TODO**

![VolumeCreate](/assets/4-6_isiTODO)

**3. Stop Hapus Mulai ulang**

![VolumeCreate](/assets/4-7_stop-hapus-mulai)

**4. hasil reload**

![VolumeCreate](/assets/4-8_jalankanlagi)


## Quick Volume Type Comparison (Using Bind Mounts)

**STARTING DEV-MODE CONTAINER**

**1. pastikan semua docker-101 telah nonaktif**

![QuickVolume](/assets/5-1_mematikanDocker-101)
   
**2. Jalankan Script**

![QuickVolume](/assets/5-2_Script)

-dp 3000:3000: Flag ini menentukan pemetaan port, di mana port 3000 pada host dipetakan ke port 3000 pada kontainer.

-w /app: Ini mengatur direktori kerja di dalam kontainer menjadi /app, artinya semua perintah berikutnya akan dieksekusi dari direktori ini.

node:10-alpine: Ini adalah gambar Docker yang akan digunakan. Ini adalah gambar Node.js yang ringan berbasis Alpine Linux, yang sering digunakan untuk kontainerisasi karena ukurannya yang kecil.

sh -c "yarn install && yarn run dev": Perintah ini memulai sebuah shell (sh) di dalam kontainer dan kemudian menjalankan dua perintah yang dipisahkan oleh &&. Pertama, ia menjalankan yarn install untuk menginstal dependensi proyek yang ditentukan di package.json. Kemudian, ia menjalankan yarn run dev, yang biasanya memulai server pengembangan menggunakan nodemon, sebuah alat yang secara otomatis me-restart server ketika file berubah
    

**3. Buka Docker log**

![QuickVolume](/assets/5-3_dockerLogs)

**4. Edit file src/static/js/app.js di line 109**

![QuickVolume](/assets/5-4_before)

![QuickVolume](/assets/5-4_after)

**5. Hasil**

![QuickVolume](/assets/5-5_hasil)

*Feel free to make any other changes you'd like to make. When you're done, stop the container and build your new image using docker build -t docker-101 .


## Container Networking (Multi-Container Apps)

**Starting A SQL**

**1. create TODO app**

![Multi-Container Apps](/assets/6-1_networkCreate)

**2. Start dan Hubungkan Ke MY SQl (script)**

![Multi-Container Apps](/assets/6-2_startdanAttachMySQL)

**3. Masuk ke MYSQl**

![Multi-Container Apps](/assets/6-3_masukMYSQL)

**4. Show DATABASE**

![Multi-Container Apps](/assets/6-4_showdatabase)



**Connecting To MYSQl**

**1. menghubungkan ke nikolaka/netshoot**

![Multi-Container Apps](/assets/6-5_mencobamasukkenikolakanetshoot)

**2. dig mysql**

![Multi-Container Apps](/assets/6-6_digmySQL)


**lihat data (setelah Show Database)**

**1. lihat isi Item yang di input di TODO**

![Multi-Container Apps](/assets/6-7_lihat-isi-item)



## Installing Docker Compose (Using Docker Compose)

**1. melihat isi docker version dan membuat file Docker-compose.yml**

![Multi-Container Apps](/assets/7-1_Dockerver)

**2. Isi Docker-compose.yml**

![Multi-Container Apps](/assets/7-2_isi-Script)

**3. Docker compose**

![Multi-Container Apps](/assets/7-3_docker-compose)



