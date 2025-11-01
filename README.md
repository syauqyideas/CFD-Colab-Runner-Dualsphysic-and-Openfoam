<div align="center"><img src="https://www.google.com/search?q=https://placehold.co/100x100/10b981/ffffff%3Ftext%3DCFD%2BRunner" alt="CFD Runner Logo" style="border-radius: 50%;"><h1>🌊🔥 CFD Colab Runners: DualSPHysics & OpenFOAM</h1><p><i>Mendemokratisasi Simulasi Fluida di Cloud.</i></p><p align="center"><!-- LINK NOTEBOOK DUALSPHYSICS --><a href="https://colab.research.google.com/github/syauqyideas/DualSPHysic_Colab_Notebook_Runner/blob/main/DualSPHPhysic_Fixed_Public.ipynb" target="_blank"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open DualSPHysics in Colab"/></a>&nbsp;<!-- LINK NOTEBOOK OPENFOAM --><a href="https://www.google.com/search?q=https://colab.research.google.com/github/syauqyideas/DualSPHysic_Colab_Notebook_Runner/blob/main/OpenFoam_COLAB_Public%2520(1).ipynb" target="_blank"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open OpenFOAM in Colab"/></a></p><hr></div>Halo! Mari Berkenalan Lebih Jauh! 👋Saya Syauqy Ideas (atau panggil saja Syauqy!), seorang yang memiliki hasrat besar terhadap dunia Computational Fluid Dynamics (CFD) dan simulasi numerik. Bagi saya, CFD bukan hanya tentang angka dan persamaan, tetapi tentang seni menerjemahkan realitas fisika ke dalam kode—dan membuatnya dapat diakses oleh semua orang.Repositori ini lahir dari semangat itu. Saya menyajikan sepasang notebook Google Colab yang siap pakai untuk mendemokratisasi akses ke solver CFD canggih: DualSPHysics (Metode SPH) dan OpenFOAM (Metode FVM).Tujuan saya? Membuat Anda dapat menjalankan simulasi berbasis partikel yang kompleks dan simulasi FVM skala industri langsung dari peramban web Anda, memanfaatkan kekuatan cloud computing Google Colab.Jika Anda tertarik pada inovasi open-source, simulasi fluida, atau mencari rekan kolaborasi untuk proyek teknis, Anda berada di tempat yang tepat!<div align="center"><h3>✨ Mari Terhubung dan Ciptakan Inovasi Bersama! ✨</h3></div>🛠️ Alat CFD dalam Genggaman Anda (DualSPHysics vs. OpenFOAM)Dua notebook ini mewakili dua pendekatan fundamental dalam simulasi CFD <br>

Metode SPH menggunakan DualSPHysics  & Metode FVM menggunakan  OpenFOAM  <br><br>

Fokus Utama yang dapat diselesaikan oleh <strong>Openfoam</strong> : <br> Aliran permukaan bebas (Free-Surface Flow), interaksi fluida-struktur, dan dinamika yang sangat non-linear. Berbagai masalah Mekanika Fluida, Perpindahan Panas, dan Reaksi Kimia (standar industri). <br><br>
Fokus Utama yang dapat diselesaikan oleh <strong>Dualsphysic</strong> : <br> Pendekatan Berbasis Lagrangian (partikel bergerak).Berbasis Eulerian (elemen volume tetap).Platform ini ideal untuk menggunakan GPU Colab.Berjalan optimal di CPU multi-core Colab.<br><hr><hr>📝 Panduan Penggunaan Detail<br><br>Pastikan Anda telah mengkloning kasus simulasi Anda (baik DualSPHysics XML/input files atau folder kasus OpenFOAM) ke Google Drive atau GitHub sebelum memulai<br><br> <hr>.🌊 Panduan untuk DualSPHysics Runner (SPH)Notebook ini memanfaatkan akselerasi GPU Colab dan ideal untuk kasus free-surface flow.
<ol><li><b>Koneksi & Setup Dasar</b><ul><li>Buka notebook <code>DualSPHPhysic_Fixed_Public.ipynb</code>.</li>
  <li>Jalankan sel di bawah judul "Google Drive Connect" untuk menghubungkan penyimpanan Anda.</li>
  <li>Jalankan sel di bawah judul "Setting Environment" (menginstal driver/dependensi).</li></ul></li>
  <li><b>Konfigurasi Kasus</b><ul><li>Di sel kode pertama (dengan banyak variabel), atur:
    <ul>
      <li><code>name</code>: Nama kasus Anda.</li>
      <li><code>DualsphysicsVersion</code>: Pilih versi yang Anda gunakan (misalnya, <code>5.2.2</code>).</li>
      <li>Konfigurasi detail proyek GitHub Anda (<code>github_project</code>, <code>github_username</code>, <code>personal_project_repo</code>).</li>
    </ul></li></ul></li>
  <li><b>Instalasi & Kloning</b><ul>
    <li>Jalankan sel di bawah judul "Github Download Dualsphysic and clone your own project".</li>
    <li>Jalankan sel di bawah judul "Setting Runner Environment, copy file to RUN_DIRECTORY" untuk menyiapkan direktori kerja.</li>
    <li>Secara default notebook ini menggunakan github dan menggunakan personal access token</li></ul></li>
  <li><b>Eksekusi Simulasi</b><ul>
    <li>Arahkan ke sel di bawah judul "Run using the internal bash command line".</li>
    <li><b>Penting:</b> Hapus tanda komentar (<code>#</code>) pada baris perintah yang ingin Anda jalankan (misalnya, <code>!$pathsph/$gencase ...</code> untuk pre-processing, <code>!$pathsph/$DualSPHysics -gpu ...</code> untuk solver, dan <code>!$pathsph/$vtk ...</code> untuk post-processing).</li>
    <li>Jalankan sel tersebut. Hasil akan disimpan ke Google Drive Anda secara otomatis pada akhir sel.</li>
  </ul>
  </li></ol>
  
  
  <br><hr><br> 
    
Panduan untuk OpenFOAM Runner (FVM)Notebook ini menyediakan environment FVM dan mendukung komputasi paralel menggunakan CPU Colab.
<ol>
  <li><b>Koneksi & Setup Dasar</b>
    <ul>
      <li>Buka notebook <code>OpenFoam_COLAB_Public.ipynb</code>.</li>
      <li>Jalankan sel di bawah judul "Connect Google Drive" untuk menghubungkan penyimpanan Anda.</li>
      <li>Jalankan sel di bawah judul "Install OpenFOAM" untuk menginstal versi OpenFOAM yang Anda pilih.</li>
    </ul>
  </li>
  <li><b>Konfigurasi Kasus</b>
    <ul>
      <li>Di sel kode pertama (di bawah judul "Set Up Your Case"), atur:<ul><li><code>name</code>: Nama folder kasus OpenFOAM Anda.</li>
      <li><code>CaseClassification</code> dan solver terkait (misalnya, <code>rhoPimpleFoam</code>).</li>
      <li><code>OpenFoamVersion</code>: Pilih versi yang diinstal.</li>
      <li>Pastikan <code>is_gdrive_based = True</code> dan atur <code>OpenFoamDrivePath</code> yang benar (secara default anda hanya perlu membuat direktori /Openfoam pada google drive anda, dan mengupload case ke dalam case tesebut (nama file menjadi variable "name").</li>
      <li>Pastikan solver problem yang anda pilih tepat (compressible, incompresible, multiphase, dll), lalu pastikan juga solver yang anda pilih dari masing-masing problem sesuai dengan solver yang anda upload ke google drive </li> 
    </ul>
  </li></ul></li>
  <li><b>Setup Kasus</b>
      <ul>
        <li>Jalankan sel di bawah judul "Set Up your OpenFoam Case" untuk menyalin kasus Anda dari Drive/GitHub ke direktori Colab.</li>
      </ul>
  </li>
  <li><b>Eksekusi Simulasi</b>
     <ul>
       <li><b>Untuk Kasus Serial:</b> Langsung jalankan perintah solver tanpa <code>-parallel</code> di bagian "Run Simulation".</li>
        <li><b>Untuk Kasus Paralel (Direkomendasikan):</b>
          <ol type="a">
            <li>Jalankan <code>setFields</code> (jika multiphase).</li>
            <li>Jalankan sel di bagian "DecomposePar - to Run multiprocessor" (<code>!decomposePar -force</code>).</li>
            <li>Jalankan sel di bagian "Run Simulation" yang menggunakan <code>mpirun</code> (<code>!mpirun --allow-run-as-root --oversubscribe -n 2 $solver -parallel</code>).</li>
          </ol>
        </li>
      </ul>
  </li>
  <li><b>Pasca-pemrosesan & Pengarsipan</b>
    <ul>
      <li>Setelah simulasi paralel selesai, Anda dapat merapihkan case sebelum di upload kembali ke google drive sel di bagian "reconstructPar" untuk menggabungkan hasil prosesor (<code>reconstructPar</code>).
      </li>
      <li>Hasil akan dicadangkan ke Google Drive atau dapat diunduh dengan menjalankan sel sel "Download Simulation Files".
  </li>
</ul>
</li>
</ol>
          <hr>
          
🤝 Mari Terhubung dan Berkolaborasi!<div style="padding: 15px; border: 2px solid #10b981; border-radius: 10px; background-color: #f7fdee; text-align: center;"><p style="font-size: 1.1em; margin-bottom: 10px;">Simulasi numerik adalah perjalanan tanpa akhir, dan saya selalu mencari ide-ide baru dan tantangan teknis. Jika Anda memiliki proyek keren, ingin berdiskusi tentang SPH/FVM, atau sekadar ingin bertukar pikiran, mari terhubung!</p><p style="margin-top: 15px;"><strong><a href="https://github.com/syauqyideas" target="_blank">🔗 GitHub</a></strong>&nbsp; | &nbsp;<strong><a href="https://www.linkedin.com/in/syauqy-ahmad-b586601b8/" target="_blank">💼 LinkedIn</a></strong>&nbsp; | &nbsp;<strong><a href="mailto:[syauqyalfarakani@gmail.com]">📧 Email</a></strong></p><p style="font-style: italic; margin-top: 10px;">Saya antusias untuk melihat apa yang bisa kita ciptakan bersama!</p></div>
