# AID - Aerial Scene Classification

**Proje amacı**: Havadan çekilmiş görüntülerden sahne sınıfı tahmini yapmak (30 sınıf).

**Veri seti**: AID dataset (Kaggle/HuggingFace). Klasör yapısı: train/, val/, test/

**Kullanılan yöntemler**:
- Veri ön işleme: Resize(128/224), normalization
- Data augmentation: rotation, flip, color jitter (opsiyonel)
- Model: Basit CNN veya Transfer Learning (ResNet50)
- Eğitim: EarlyStopping

**Değerlendirme**:
- Accuracy & Loss grafikleri
- Confusion Matrix
- Örnek tahmin görselleştirmeleri

**Kaggle Notebook**: (Kaggle notebook linkinizi buraya yapıştırın)
