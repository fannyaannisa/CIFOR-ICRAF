# DAS Sepaku Land Cover Mapping (2018)

Technical test submission for This repository contains my technical exercise submission for the Remote Sensing Assistant Technical Test for CIFOR-ICRAF Indonesia. The task focuses on replicating the land cover mapping workflow from the paper:
"A national-scale land cover reference dataset from local crowdsourcing initiatives in Indonesia"
DOI: 10.1038/s41597-022-01689-5

Author: Fannya Rachma Annisa

---

## 📌 Your Plan  

1️⃣ **Review paper + code**  
- Memahami alur kerja paper:  
  > Hadi et al. (2022) *A national-scale land cover reference dataset from local crowdsourcing initiatives in Indonesia*  
  > DOI: [10.1038/s41597-022-01689-5](https://doi.org/10.1038/s41597-022-01689-5)

2️⃣ **Area of Interest (AOI)**  
- Fokus di **DAS Sepaku**
- AOI sementara diwakili bounding box

3️⃣ **Data satellite**  
- Landsat 8 SR 2018 (cloud mask, median composite, indeks NDVI, NDWI, NDBI, MSAVI)

4️⃣ **Data referensi**  
- Dataset Figshare nasional
- Filter dengan `.filterBounds(aoi)` di GEE saat training  

5️⃣ **Machine Learning**  
- Random Forest (100 trees)
- Prediktor: B2, B3, B4, B5, B6, B7, NDVI, NDWI, NDBI, MSAVI  

6️⃣ **Output**
- Peta klasifikasi tutupan lahan DAS Sepaku tahun 2018
- Kode GEE + dokumentasi  

---

## 📌 Steps Taken  

00:00 - 00:30 → Review paper + cek kode referensi  
00:30 - 01:00 → Definisikan AOI + koleksi citra Landsat 8  
01:00 - 01:30 → Masking awan, composite, tambah indeks spektral  
01:30 - 02:00 → Upload Figshare ke GEE + sampling  
02:00 - 02:30 → Latih Random Forest + klasifikasi  
02:30 - 03:00 → Dokumentasi + finalisasi kode  

---

## 📌 Challenges Encountered  

⚠️ Upload data Figshare cukup besar → butuh waktu  
⚠️ AOI menggunakan bounding box, belum shapefile presisi  
⚠️ Distribusi kelas Figshare nasional → perlu filter di GEE  

---

## 📌 Proposed Solutions  

💡 Filter training data pakai `.filterBounds(aoi)`  
💡 Clip hasil klasifikasi ke AOI  
💡 Gunakan shapefile DAS Sepaku pada tahap lanjut  

---

## 📌 Next Steps  

🚀 Validasi hasil klasifikasi  
🚀 Perbaikan AOI dengan shapefile resmi DAS  
🚀 Export hasil klasifikasi untuk analisis lanjut  

---

## 📌 Files  

