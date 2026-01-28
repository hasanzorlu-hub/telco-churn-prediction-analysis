# 📊 Telco Customer Churn Prediction Project

## 🎯 Proje Amacı
Bu proje, bir telekomünikasyon şirketinin müşteri verilerini kullanarak, hangi müşterilerin hizmeti terk etme (Churn) riski taşıdığını tahmin etmeyi amaçlar. 
İstatistiksel analizler ve Makine Öğrenmesi (Logistic Regression) kullanılarak "müşteri kaybını önleme" stratejilerine veri odaklı destek sağlanmıştır.

## 🛠️ Kullanılan Teknolojiler ve Yöntemler
* **Python:** Pandas, NumPy, Scikit-learn
* **SQL:** SQLite ile veri manipülasyonu ve filtreleme
* **İstatistik:** Normallik Testleri (Shapiro-Wilk), Hipotez Testleri (Bağımsız iki örneklem t testi)
* **Veri Görselleştirme:** Seaborn, Matplotlib (Heatmap, ROC Curve)
* **Model Deployment:** Joblib ile modelin serileştirilmesi

## 📈 Temel Bulgular ve Sonuçlar
1.  **İstatistiksel Fark:** Terk eden müşterilerin aylık fatura ortalamalarının, kalan müşterilere göre istatistiksel olarak anlamlı derecede farklı olduğu kanıtlandı.
2.  **Dengesiz Veri (Imbalanced Data) Çözümü:** Veri setindeki dengesizlik (%75 Kalıcı / %25 Giden) nedeniyle modelin başta yaşadığı "Accuracy Tuzağı" (Recall=0) tespit edildi.
3.  **Performans Artışı:** `Class Weighting` stratejisi uygulanarak, riskli müşterileri yakalama oranı (**Recall**) %0'dan **%53'e** çıkarıldı.

