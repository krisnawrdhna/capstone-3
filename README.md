# capstone-3
Capstone 3 purwadhika - Bank Marketing Campaign
# Bussiness Understanding
**Context**

Berikut adalah data dari hasil kampanye pemasaran bank yang dilakukan melalui panggilan telepon langsung untuk menaruh deposit berjangka. Untuk klien yang setuju untuk menaruh deposit, variabel target akan diisi dengan 'yes', jika tidak 'no'

Target: 
* 0 : Tidak menaruh deposit 
* 1 : Menaruh deposit



**Problem Statement**

Proses kampanye penawaran deposit memakan waktu dan biaya, jika bank menargetkan semua nasabah tanpa melakukan penyaringan terlebih dahulu, maka akan ada pemborosan dari segi waktu dan biaya. Bank ingin meningkatkan efisiensi proses kampanye dengan menargetkan ke calon nasabah yang memiliki potensi untuk menaruh deposit.


**Goals**

Berdasarkan permasalahan tersebut, bank ingin memiliki kemampuan untuk memprediksi kemungkinan kandidat nasabah untuk mau menaruh deposit atau tidak, sehingga dapat menargetkan kampanye pada kandidat yang memiliki potensial untuk menaruh deposit.

Dan juga, perusahaan ingin mengetahui kriteria apa saja yang berpengaruh pada kandidat nasabah yang sudah menaruh deposit dan yang tidak menaruh deposit. 


**Analytic Approach**

Yang akan lakukan adalah menganalisis data untuk menemukan pola yang membedakan kandidat nasabah yang akan menaruh deposit atau tidak.

Kemudian, dilanjutkan dengan membangun model klasifikasi yang akan membantu bank untuk dapat memprediksi probabilitas seorang kandidat nasabah akan/ingin menaruh deposit atau tidak.


**Metric Evaluation**

Type 1 error : False Positive  
Konsekuensi: membuang waktu dan biaya kampanye untuk nasabah yang tidak berpotensial menaruh deposit

Type 2 error : False Negative  
Konsekuensi: kehilangan kandidat nasabah potensial

Berdasarkan konsekuensinya, maka sebisa mungkin akan dibuat model yang dapat mengurangi cost kampanye dari bank, tetapi tanpa membuat menjadi kurangnya kandidat nasabah potensial yang dicari oleh bank. Jadi kita ingin sebanyak mungkin prediksi kelas positif yang benar, dengan sesedikit mungkin prediksi false positive. Jadi nanti metric utama yang akan kita gunakan adalah F1 Score.


**Data Understanding**

Note : 
- Dataset tidak seimbang
- Sebagian besar fitur memiliki jenis kategorikal (Nominal dan Ordinal), beberapa dengan kardinalitas tinggi
- Setiap baris data merepresentasikan informasi kandidat nasabah yang sudah pernah menaruh deposit dimasa lalu
