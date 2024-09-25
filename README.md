## Tugas 6 Sistem Operasi

Nama: Raihan Faiz Ramadhan

NIM: 09011182328093

Kelas: SK3C

MK: Sistem Operasi (Praktikum)

# Praktikum 5 Job Control

1. Eksekusi seluruh profile yang ada :
a. Edit file profile /etc/profile dan tampilkan pesan sebagai berikut :
echo “Profile dari /etc/profile”
![1](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(1%20A-1).png)
![2](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(1%20A-2).png)
![3](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(1%20A-3).png)

b. Asumsi nama anda stD02001, maka edit semua profile yang ada yaitu :

/home/stD02001/.bash_profile

/home/. stD02001/.bash_login

/home/mahasiswa/.profile

/home/mahasiswa/.bashrc

Ganti nama /home/mahasiswa dengan nama anda sendiri. Pada setiap
file tersebut, cantumkan instruksi echo, misalnya pada /home/ mahasiswa/.bash_profile :
echo “Profile dari .bash_profile”
Lakukan hal yang sama untuk file lainnya, sesuaikan tampilan dengan nama file yang
bersangkutan.
![4](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(1%20B).png)
![5](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(1%20B-1).png)
![6](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(1%20B-3).png)
![7](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(1%20B-4).png)
![8](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(1%20B-5).png)


c. Jalankan instruksi subtitute user, kemudian keluar dengan perintah exit sebagai berikut:
$ su mahasiswa
$ exit
kemudian gunakan opsi – sebagai berikut :
Jelaskan perbedaan kedua utilitas tersebut.
![9](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(1%20C).png)

2. Prompt String (PS)
a. Edit file .bash_profile, ganti prompt PS1 dengan ‘>’. Instruksi export diperlukan dengan
parameter nama variable tersebut, agar perubahan variable PS1 dikenal oleh semua shell
PS1=‟> „
export PS1
![10](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(2%20A).png)

b. Eksperimen hasil PS1 :
PS1=“\! > “
69 > PS1=”\d > “
Mon Sep 23 > PS1=”\t > “
10:10:20 > PS1=”Saya=\u > “
Saya=mahasiswa > PS1=”\w >”
~ > PS1=\h >”
![11](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(2%20B).png)

3. Logout
Edit file .bash_logout, tampilkan pesan dan tahan selama 5 detik, sebelum eksekusi logout
Echo “Terima kasih atas sesi yang diberikan”
Sleep 5
Clear
![12](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(3).png)
![13](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(3.1).png)

4. Bash script

a. Buat 3 buah script p1.sh, p2.sh, p3.sh dengan isi masing-masing :
p1.sh
#! /bin/bash
echo “Program p1”
ls –l
p2.sh
#! /bin/bash
echo “Program p2”
who
p3.sh
#! /bin/bash
echo “Program p3”
ps x

b. Jalankan script tersebut sebagai berikut :
$ ./p1.sh ; ./p3.sh ; ./p2.sh
$ ./p1.sh &
$ ./p1.sh $ ./p2.sh & ./p3.sh &
$ ( ./p1.sh ; ./p3.sh ) &
![14](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(4).png)
![15](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(4.1).png)
![16](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(4.1.1).png)
![17](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(4.1.2).png)
![18](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(4.1.3).png)
![19](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(4.2).png)
![20](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(4.3).png)
![21](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(4.4).png)


5. Jobs

a. Buat shell-script yang melakukan loop dengan nama pwaktu.sh,
setiap 10 detik, kemudian menyimpan tanggal dan jam pada file hasil.
#!/bin/bash
while [ true ]
do
date >> hasil
sleep 10
done
![22](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(5.1).png)

b. Jalankan sebagai background; kemudian jalankan satu program (utilitas find) di background
sebagai berikut :
$ jobs
$ find / -print > files 2>/dev/null &
$ jobs
c. Jadikan program ke 1 sebagai foreground, tekan ^Z dan kembalikan program tersebut ke
background
$ fg %1
$ bg
![23](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(5%20B%20C).png)

d. Stop program background dengan utilitas kil
$ ps x
$ kill [Nomor PID]
![24](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(5.4).png)
![25](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(5.4.1).png)
![26](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(5.4.2).png)


6. History

a. Ganti nilai HISTSIZE dari 1000 menjadi 20
$ HISTSIZE=20
$ h
![27](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(6.1).png)

b. Gunakan fasilitas history dengan mengedit instruksi baris ke 5 dari instruksi yang terakhir
dilakukan
$ !-5

c. Ulangi instruksi yang terakhir. Gunakan juga ^P dan ^N untuk bernavigasi pada history bufer
$ !!
![28](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(6.2).png)

d. Ulangi instruksi pada history bufer nomor 150
$ !150
![29](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(6.3).png)
![30](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(6.3.1).png)
![31](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(6.3.2).png)

e. Ulangi instruksi dengan prefix “ls”
$ !ls
![32](https://github.com/RaihanFaiz165/Raihan-Faiz-Ramadhan_09011182328093_SK3C_Tugas-6_-Sistem-Operasi/blob/main/Screenshot%20tugas%206/(6.4).png)

