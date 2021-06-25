# API Data Sekolah Seluruh Indonesia
### Assalamualaikum wr.wb
### API gratis untuk Data Sekolah Seluruh Indonesia. Maaf jika kadang-kadang datanya lambat respon karena keseluruhan datanya sangat banyak dan insyallah sangat lengkap, mulai dari jenjang SD, SMP, SMA, SMK di seluruh Indonesia dan mohon maaf sekali jika fitur-fiturnya belum lengkap. insyallah saya akan lebih mengembangkan api ini lebih baik lagi.

### API ini dibuat menggunakan: <br>
<div align="center">
<img alt="Express.js" src="https://img.shields.io/badge/express.js%20-%23404d59.svg?&style=for-the-badge"/>
<img alt="MongoDB" src ="https://img.shields.io/badge/MongoDB-%234ea94b.svg?&style=for-the-badge&logo=mongodb&logoColor=white"/>
</div>

# Penggunaan

BASE Url:
```bash
https://api-sekolah-indonesia.herokuapp.com
```
## - Menampilkan seluruh data-data sekolah namun ada limitnya
Kenapa saya memberi limit ? karena datanya sangat banyak sekali jika ditampilkan semuanya hehehe
```bash
https://api-sekolah-indonesia.herokuapp.com/sekolah/limits
```
Note: Limit berupa integer / number. limit adalah jumlah data yg ingin ditampilkan. Contoh: ```https://api-sekolah-indonesia.herokuapp.com/sekolah/5```

Contoh Response: 
```bash
[
  {
  _id: "60d531f3ec2a980ec2df2432",
  kode_prop: "010000 ",
  propinsi: "Prov. D.K.I. Jakarta",
  kode_kab_kota: "010100 ",
  kabupaten_kota: "Kab. Kepulauan Seribu",
  kode_kec: "010101 ",
  kecamatan: "Kec. Kepulauan Seribu Selatan",
  id: "40C6E595-2BF5-E011-B2F2-796762867641",
  npsn: "20106343",
  sekolah: "SMP NEGERI 241",
  bentuk: "SMP",
  status: "N",
  alamat_jalan: "Jl. Pendidikan",
  lintang: "-5.7985000",
  bujur: "106.5003000"
  }
]
```

## - Menampilkan data sekolah berdasarkan jenjang namun ada limitnya
Kenapa saya memberi limit ? karena datanya sangat banyak sekali jika ditampilkan semuanya hehehe
```bash
https://api-sekolah-indonesia.herokuapp.com/sekolah/bentuk/limits
```
Note: "bentuk" disini maksudnya adalah JENJANG, jenjang hanya SD, SMP, SMA, SMK dan Limit berupa integer / number. limit adalah jumlah data yg ingin ditampilkan. Contoh: ```https://api-sekolah-indonesia.herokuapp.com/sekolah/smk/5```

Contoh Response: 
```bash
[
  {
  _id: "60d531f4ec2a980ec2df2445",
  kode_prop: "010000 ",
  propinsi: "Prov. D.K.I. Jakarta",
  kode_kab_kota: "010100 ",
  kabupaten_kota: "Kab. Kepulauan Seribu",
  kode_kec: "010101 ",
  kecamatan: "Kec. Kepulauan Seribu Selatan",
  id: "8C57BE23-E673-4FC3-A8E0-18A6D68F43EF",
  npsn: "20109165",
  sekolah: "SMKN 61 JAKARTA",
  bentuk: "SMK",
  status: "N",
  alamat_jalan: "PANTAI SELATAN 1 PULAU TIDUNG.",
  lintang: "-5.8023000",
  bujur: "106.5099000"
  }
]
```

### Gunakan free API ini dengan Bijak dan Benar ya :)
### Jika ada kesalahan pada API atau ingin meminta saran bisa hubungi email: alwanrabbae@gmail.com atau lewat issues pada repo ini.<br>Kurang lebihnya mohon maaf, Wassalamualaikum wr.wb
