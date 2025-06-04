# 🏨 Hotel Booking Cancellation Prediction

**Menggunakan Machine Learning untuk Mengidentifikasi Risiko Pembatalan Reservasi Hotel**

![Banner](https://imgur.com/your-custom-banner-image.png) <sub>✨ Prediksi pembatalan reservasi demi strategi bisnis hotel yang lebih cerdas ✨</sub>

---

## 📌 Proyek Ini Tentang Apa?

Proyek ini bertujuan untuk membangun model prediktif yang dapat mengidentifikasi kemungkinan pembatalan pemesanan hotel (**booking cancellation**). Dengan model ini, pihak manajemen hotel dapat mengantisipasi risiko pembatalan dan menyusun strategi bisnis yang lebih efisien, seperti overbooking strategy, manajemen inventori kamar, hingga alokasi sumber daya.

---

## 🧭 Alur Proyek

```mermaid
graph LR
A[Raw Dataset] --> B[Data Cleaning and Preprocessing]
B --> C[Exploratory Data Analysis]
C --> D[Feature Engineering]
D --> E1[Modeling (XGBoost and RF)]
E1 --> F[Model Evaluation]
F --> G[Model Interpretation (SHAP)]
G --> H[Business Insight and Recommendations]
```
]
```

## 🔍 Dataset

Dataset yang digunakan berasal dari data pemesanan hotel fiktif yang merepresentasikan dua jenis hotel (City dan Resort) beserta atribut-atribut penting seperti:

* Lama waktu booking sebelum menginap (lead\_time)
* Jumlah tamu dan anak-anak
* Tipe kamar dan channel pemesanan
* Apakah customer memodifikasi booking
* Dan lainnya…

---

## 📊 Exploratory Data Analysis

Beberapa visualisasi menarik dari proses EDA:

### 1. **Distribusi Pembatalan**

![Cancel Dist](https://imgur.com/your-image1.png)

📌 *36.94% dari total pemesanan dibatalkan.*

### 2. **Top Booking Channel dengan Angka Pembatalan Tertinggi**

![Channel Cancel](https://imgur.com/your-image2.png)

📌 *Channel TA/TO memiliki proporsi pembatalan tertinggi.*

---

## 🤖 Modeling & Evaluation

Dua model utama digunakan:

* 🎯 **XGBoost Classifier**
* 🌳 **Random Forest Classifier**

### 🔥 Best Model Performance (XGBoost)

| Metric    | Not Canceled | Canceled |
| --------- | ------------ | -------- |
| Precision | 0.82         | 0.84     |
| Recall    | 0.93         | 0.65     |
| F1-Score  | 0.87         | 0.73     |

**Overall Accuracy: 82%**

---

## 💡 SHAP Explanation

### 📌 Feature Importance dengan SHAP

![SHAP Beeswarm](https://imgur.com/your-image3.png)

Fitur yang paling memengaruhi prediksi:

* `lead_time`
* `previous_cancellations`
* `booking_changes`
* `room_mismatch_flag`

---

## 🧠 Business Insight

* 🟡 **Lead Time Tinggi = Potensi Pembatalan Lebih Besar**
  Customer yang memesan jauh hari cenderung lebih berisiko membatalkan.

* 🔴 **Booking melalui TA/TO lebih rentan dibatalkan**, dibandingkan channel direct atau online travel agents.

* 🟢 **Model dapat membantu manajemen dalam mengambil keputusan** seperti menetapkan kebijakan overbooking atau memberi promo khusus pada channel tertentu.

---

## 🚀 Teknologi & Tools

* Python (Pandas, Scikit-Learn, XGBoost)
* Matplotlib, Seaborn, SHAP
* Jupyter Notebook / Google Colab
* Git & GitHub

---

## 📂 Akses Proyek

* 📘 [Google Colab Project Link](https://colab.research.google.com/drive/1Y0H-eg1HH3DPUgi3iZu1D7HHPKDJdfnK?usp=drive_link)
* 💻 [GitHub Repository](https://github.com/dhardianto281094)

---

## 👋 Tentang Saya

Hi! Saya **Dimas Hardianto**, seorang data enthusiast dengan latar belakang komunikasi & pengalaman 5+ tahun di industri perbankan dan fintech. Saya bertransformasi menjadi **Data Scientist** untuk menyatukan pemahaman bisnis dan kekuatan data.

📫 [Connect on LinkedIn](https://linkedin.com/in/your-link)
💡 Let's collaborate and bring data-driven strategies to life!

---

## 🌟 Jika kamu suka proyek ini...

Silakan beri ⭐ di repo ini, dan jangan ragu untuk membuka issue atau diskusi jika ada pertanyaan atau ingin berkolaborasi.

---

> *"Great data means great decisions. Let’s build smarter businesses together."* 🧠📊

---

Jika kamu butuh bantuan **membuat banner/visual custom** agar tampil lebih profesional di README, aku juga bisa bantu. Mau?
