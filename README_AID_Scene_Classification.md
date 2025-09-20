# 🌍 AID Scene Classification - Derin Öğrenme Projesi

## 📌 Proje Hakkında
Bu proje, Akbank Derin Öğrenme Bootcamp kapsamında verilen *AID (Scene Classification)* veri seti üzerinde gerçekleştirilmiştir.  
Amaç, farklı sahneleri (örneğin havaalanı, park, köprü, yerleşim alanı vb.) görüntülerden otomatik olarak sınıflandırabilen bir derin öğrenme modeli geliştirmektir.

---

## 🗂 Kullanılan Veri Seti
- *Dataset*: AID Scene Classification
- *Kaynak*: Kaggle dataset
- *Klasör yapısı*: train/, val/, test/ alt dizinlerinde sınıf bazlı ayrım mevcuttur.

---

## ⚙ Kullanılan Yöntemler
- *Veri Ön İşleme*:
  - ImageDataGenerator ile tüm resimler yeniden ölçeklendirildi (128x128).
  - Train/Validation/Test ayrımı yapıldı.
- *Model*:
  - Basit CNN modeli kuruldu (Conv2D + MaxPooling + Dense).
  - Adam optimizer, categorical_crossentropy loss fonksiyonu kullanıldı.
- *Eğitim*:
  - Model belirli epoch sayısı boyunca eğitildi.
  - Eğitim ve doğrulama doğruluk/loss grafikleri çıkarıldı.

---

## 📊 Sonuçlar
- Eğitim / Doğrulama *Accuracy & Loss grafikleri* elde edildi.
- *Confusion Matrix* oluşturuldu → hangi sınıfların karıştırıldığını görselleştirdi.
- *Classification Report* alındı → precision, recall ve f1-score değerleri incelendi.
- (Not: Grad-CAM bu projede uygulanmamıştır.)

---

## 📂 Çıktılar
- Model .h5 formatında kaydedildi.
- Accuracy & Loss grafik ekran görüntüleri.
- Confusion Matrix görselleştirmesi.
- Classification Report çıktısı.

---

## 🚀 Çalıştırma Adımları
1. Kaggle Notebook açın. Kaggle notebook linki: https://www.kaggle.com/code/enesgleryz/havasina  
2. Dataset yolunu şu şekilde ayarlayın:  
   ```python
   base_path = "/kaggle/input/aid-scene-classification-datasets/AID"
