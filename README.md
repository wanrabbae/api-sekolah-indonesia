# API Data Sekolah Seluruh Indonesia v2.0
### Assalamualaikum wr.wb
### API gratis untuk Data Sekolah Seluruh Indonesia v2.0. Jenjang SD, SMP, SMA, SMK di seluruh Indonesia. Insyallah lengkap...

### API ini dibuat menggunakan: <br>
<div align="center">
<img alt="Express.js" src="https://img.shields.io/badge/express.js%20-%23404d59.svg?&style=for-the-badge"/>
<img alt="MongoDB" src ="https://img.shields.io/badge/MongoDB-%234ea94b.svg?&style=for-the-badge&logo=mongodb&logoColor=white"/>
</div>

### Apa yg baru dari API ini ?
- Pagination API!
- Search sekolah berdasarkan nama sekolah!

# Penggunaan

BASE URL:
```bash
https://api-sekolah-indonesia.vercel.app
```
## - Menampilkan seluruh data-data sekolah

```bash
/sekolah?page=1&perPage=5
```
Note: ```page``` dan ```perPage``` berupa integer / number.

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

## - Menampilkan data sekolah berdasarkan jenjang

```bash
/sekolah/SMK?page=1&perPage=5
```
Note: jenjang hanya SD, SMP, SMA, SMK. ```page``` dan ```perPage``` berupa integer / number.

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

## - Search data sekolah berdasarkan nama sekolah

```bash
/sekolah/s?sekolah=NAMA_SEKOLAH
```
Contoh: ``` /sekolah/s?sekolah=smks informatika ```

Contoh Response: 
```bash
[
  {
    kode_prop: "010000 ",
    propinsi: "Prov. D.K.I. Jakarta",
    kode_kab_kota: "016300 ",
    kabupaten_kota: "Kota Jakarta Selatan",
    kode_kec: "016302 ",
    kecamatan: "Kec. Pasar Minggu",
    id: "67EEF23E-FBF3-44CD-8DA1-97ACD5E1EB3D",
    npsn: "20109266",
    sekolah: "SMKS INFORMATIKA YASMA",
    bentuk: "SMK",
    status: "S",
    alamat_jalan: "JL. JERUK PURUT",
    lintang: "-6.3094000",
    bujur: "106.8143000"
  },
  {
    kode_prop: "020000 ",
    propinsi: "Prov. Jawa Barat",
    kode_kab_kota: "020500 ",
    kabupaten_kota: "Kab. Bogor",
    kode_kec: "020507 ",
    kecamatan: "Kec. Ciomas",
    id: "E25B4F76-B0CA-417C-A5C7-262DE59EC79A",
    npsn: "20232431",
    sekolah: "SMKS INFORMATIKA BINA GENERASI BOGOR",
    bentuk: "SMK",
    status: "S",
    alamat_jalan: "JL.CIKERTI NO.12",
    lintang: "-6.6004000",
    bujur: "106.7656000"
  },
]
```

## - Filter query parameter data berdasarkan `kode provinsi`, `atau kode kabupaten/kota`, atau `kode kecamatan`

### - By provinsi
```
/sekolah?provinsi=071700&page=1&perPage=5
```
```
/sekolah/smp?provinsi=071700&page=1&perPage=5
```

### - By kabupaten/kota
```
/sekolah?kab_kota=071700&page=1&perPage=5
```
```
/sekolah/sd?kab_kota=071700&page=1&perPage=5
```

### - By kecamatan
```
/sekolah?kec=071700&page=1&perPage=5
```
```
/sekolah/smk?kec=071700&page=1&perPage=5
```

### Gunakan free API ini dengan Bijak dan Benar ya :)
### Jika ada kesalahan pada API atau ingin meminta saran bisa hubungi email: alwanrabbae@gmail.com atau lewat issues pada repo ini.<br>Kurang lebihnya mohon maaf, Wassalamualaikum wr.wb
