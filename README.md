# Tugas-6-SBD-20.D2
<h1> Melakukan <i> backup </i> dan <i> recovery database </i> dengan SQL </h1>
<h3><b> Masuk ke dalam database yang akan kita <i> backup </i> dan <i> recovery </i> </b></h3>
<br>

![T6 - Masuk Database](https://user-images.githubusercontent.com/67790978/172022417-475da8b9-656a-4c3e-9a55-4e8a2f04ac22.png)

![T6 - Masuk Database2](https://user-images.githubusercontent.com/67790978/172022422-2865c016-3250-4226-86b0-6a44406c2934.png)

<h3><b> <i> Backup </i> dan <i> Recovery Database </i> dengan perintah SQL </b></h3>
<br>
<ol>
  <li> Tabel Dokter </li>
  <br>
  
  ![T6 - backup restore - 4](https://user-images.githubusercontent.com/67790978/172022262-5c5bddcc-27f2-4778-a64a-91c9ecd83e48.png)

  <li> Tabel Pasien </li>
  <br>
  
  ![T6 - backup restore - 6](https://user-images.githubusercontent.com/67790978/172022331-33e3f482-7407-477b-904d-95453ba8a304.png)

  <li> Tabel Obat </li>
  <br>
  
  ![T6 - backup restore - 5](https://user-images.githubusercontent.com/67790978/172022505-44347051-6873-4980-bf6f-1c8596fa3a1f.png)
 
  <li> Tabel Berobat </li>
  <br>
  
  ![T6 - backup restore - 3](https://user-images.githubusercontent.com/67790978/172022493-0fd84c11-b77e-4f2a-b45f-e33a6583d24a.png)

  <li> Tabel Resep Obat </li>
  <br>
  
  ![T6 - backup restore - 2](https://user-images.githubusercontent.com/67790978/172022532-5365509e-7500-4967-96f8-f3cae39a779b.png)
  
  <li> Tabel User </li>
  <br>
  
  ![T6 - backup restore - 1](https://user-images.githubusercontent.com/67790978/172022543-6792cb00-8e26-4784-8b55-5a5ec3092b4d.png)

</ol>
Hasil backup

![T6 - File Backup1](https://user-images.githubusercontent.com/67790978/172022694-4554623e-2db6-4b17-8cab-bc719032034b.png)

<h3><b> <i> Backup </i> dan <i> Recovery Database </i> menggunakan SQLDUMP</b></h3>

![T6 - backup restore - mysqldump](https://user-images.githubusercontent.com/67790978/172022701-66c700e3-9a50-44a8-ac76-693ce2e51314.png)

Hasil Backup

![T6 - File Backup2](https://user-images.githubusercontent.com/67790978/172022729-84c58029-0193-4006-9bc4-ef2b0edf5765.png)

<h3><b> Penulisan script <i> cron job <i> untuk melakukan backup otomatis setiap hari minggu jam 12 malam</b></h3>
<b> 0 24 * * 7 mysqldump -u adminklinik -p 312010110 klinik312010110 > wbackup_klinik312010110.sql </b>
