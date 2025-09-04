# 🎵 Spotify Churn Dashboard  

## 📖 Business Context  
Customer churn (berhentinya pelanggan) adalah tantangan besar bagi bisnis berbasis subscription seperti Spotify.  
Dengan memahami faktor-faktor yang memengaruhi churn, perusahaan dapat merancang strategi retensi yang lebih efektif, mengurangi kehilangan pelanggan, dan meningkatkan loyalitas pengguna.  

Proyek ini bertujuan untuk:  
- Mengidentifikasi pola perilaku user yang berhubungan dengan churn  
- Mengembangkan insight bisnis dari data streaming Spotify  
- Menyajikan hasil analisis dalam bentuk **dashboard interaktif** untuk pengambilan keputusan  

---

## 📂 Dataset Overview  
- **Source:** Synthetic dataset from Kaggle  
- **Format:** CSV  
- **Unit of Analysis:** 1 row = 1 user Spotify  
- **Target Variable:** `Churn` (Yes = churned, No = retained)  

**Key Columns**  
- `avg_daily_minutes` → Rata-rata menit mendengarkan musik per hari  
- `playlists_created` → Jumlah playlist yang dibuat user  
- `skips` → Jumlah rata-rata skip lagu per hari  
- `support_tickets` → Jumlah tiket komplain user  
- `days_since_last_login` → Lama tidak login (hari)  
- `subscription_type` → Free / Premium / Family / Student  
- `tenure` → Lama berlangganan (bulan)  
- `Churn` → Variabel target  

---

## 🔍 Key Insights  

1. **Engagement**  
   - User churn memiliki waktu dengar musik harian lebih rendah.  
   - Engagement rendah = risiko churn lebih tinggi.  

2. **Playlist Behavior**  
   - User churn rata-rata hanya punya 0–1 playlist.  
   - Non-churn lebih sering membuat banyak playlist.  

3. **Skips per Day**  
   - Churn users memiliki skip rate lebih tinggi → tanda rekomendasi musik tidak sesuai preferensi.  

4. **Support Tickets**  
   - Banyak tiket support berhubungan dengan churn yang tinggi → pengalaman buruk.  

5. **Days Since Last Login**  
   - Non-churn login ≤ 5 hari terakhir, churn rata-rata tidak login 20–50 hari.  

6. **Subscription Type**  
   - Free users lebih rentan churn dibanding Premium/Family.  

---

## ✅ Business Recommendations  

1. **Tingkatkan Engagement**  
   - Fitur *Daily Mix* / *For You Playlist* untuk user engagement rendah.  

2. **Dorong Pembuatan Playlist**  
   - Gamifikasi: reward untuk user yang membuat playlist populer.  

3. **Kurangi Skip Rate**  
   - Optimalkan algoritma rekomendasi musik + feedback button untuk skip.  

4. **Perbaiki Customer Support**  
   - Tingkatkan respon komplain, analisis tiket untuk deteksi masalah berulang.  

5. **Retensi User Tidak Aktif**  
   - Kirim notifikasi/email promo untuk user tidak login >14 hari.  
   - Berikan voucher premium trial untuk menarik kembali user.  

6. **Konversi Free → Premium**  
   - Edukasi benefit premium + buat promo upgrade untuk free users.  

---

## 📊 Dashboard  

Visualisasi insight churn Spotify tersedia dalam bentuk dashboard:  

- **Notebook Analisis:** [analisis-spotify-customer-churn.ipynb](https://github.com/xxvlrapss/spotify-churn-dashboard/blob/main/analisis-spotify-customer-churn.ipynb)  

---

## 📎 References  
- Kaggle: [Spotify Customer Churn Dataset]([https://www.kaggle.com/](https://www.kaggle.com/datasets/abdulwadood11220/spotify-customer-churn-dataset/)  
- Kaggle Notebook: [Analisis Spotify Customer Churn](https://www.kaggle.com/code/dimasprayoga/analisis-spotify-customer-churn)  
