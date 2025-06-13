# EduBot - AI Eğitim Asistanı

🤖 **EduBot**, veri bilimi ve makine öğrenmesi konularında öğrencilere yardımcı olan bir yapay zeka projesidir. Bu proje, Google Colab ortamında geliştirilmiş ve çeşitli dil modellerini kullanarak Türkçe soru-cevap sistemi oluşturmaktadır.

## 📋 Proje İçeriği

### 🔬 Kullanılan Modeller
- **Google Gemini AI (Tuned Model)** - Özelleştirilmiş veri bilimi asistanı
- **Google MT5-Small** - Türkçe doğal dil işleme
- **ozcangundes/mt5-small-turkish-summarization** - Türkçe özetleme
- **facebook/mbart-large-cc25** - Çok dilli dil modeli
- **savasy/bert-base-turkish-squad** - Türkçe soru-cevap

### 📁 Dosya Yapısı
```
EduBot/
├── dataset/                   # Veri Seti
│   └── 499satır.xlsx         # Eğitim veri seti (499 soru-cevap)
├── models/                    # AI Modelleri
│   ├── 10satırdemo.ipynb     # Gemini AI model eğitimi ve test
│   └── hugingface.ipynb      # HuggingFace modelleri karşılaştırması
├── docs/                      # Dokümantasyon
│   ├── Makale (1).pdf        # Proje makalesi
│   ├── Sunum.pdf             # Sunum dosyası
│   └── read me.pdf           # Proje açıklama dosyası
└── README.md                  # Bu dosya
```

## 🚀 Özellikler

### ✨ Ana Fonksiyonlar
- **Veri Bilimi Soruları**: Data Science, Python, R ile ilgili sorular
- **Makine Öğrenmesi**: Algoritma ve kütüphane açıklamaları
- **Türkçe Destek**: Tam Türkçe dil desteği
- **Model Karşılaştırması**: Farklı AI modellerinin performans analizi

### 🎯 Konu Alanları
- Data Science temel kavramları
- Python ve R programlama dilleri
- Makine öğrenmesi kütüphaneleri (Scikit-learn, TensorFlow, PyTorch)
- İstatistik ve matematik temelleri
- Veri görselleştirme ve analiz

## 💻 Kurulum ve Kullanım

### Gereksinimler
```python
# Google Colab ortamında çalışır
import google.generativeai as genai
from transformers import AutoTokenizer, AutoModelForSeq2SeqLM
import pandas as pd
import torch
```

### Hızlı Başlangıç
1. **Google Colab'da açın**: `models/10satırdemo.ipynb` dosyasını Google Colab'da çalıştırın
2. **API Anahtarı**: Google Gemini API anahtarınızı ekleyin
3. **Veri Seti**: `dataset/499satır.xlsx` dosyasını kullanın
4. **Model Eğitimi**: Veri setiyle modeli eğitin
5. **Test**: Sorularınızı test edin

```python
# Örnek kullanım
response = tuned_model.generate_content("Data Science nedir?")
print(response.text)
```

## 📊 Model Performansları

| Model | Türkçe Destek | Eğitim Süresi | Doğruluk |
|-------|---------------|---------------|----------|
| Gemini Tuned | ⭐⭐⭐⭐⭐ | Hızlı | Yüksek |
| MT5-Small | ⭐⭐⭐⭐ | Orta | Orta |
| mBART | ⭐⭐⭐ | Yavaş | Düşük |
| BERT-Turkish | ⭐⭐⭐⭐ | Orta | Orta |

## 🎓 Eğitim Veri Seti

Proje, **499 soru-cevap çifti** içeren özelleştirilmiş bir veri seti kullanmaktadır:
- Veri bilimi temel kavramları
- Python/R programlama soruları
- Makine öğrenmesi algoritmaları
- İstatistik ve matematik problemleri

## 🔧 Teknik Detaylar

### Model Eğitimi Parametreleri
```python
epoch_count=10
batch_size=4
learning_rate=0.001
max_length=256
```

### Desteklenen Sorular
- "Data Science nedir?"
- "Python'da makine öğrenimi için hangi kütüphaneler kullanılıyor?"
- "Outlier nedir?"
- "R'da text mining nasıl yapılır?"

## 📈 Sonuçlar

EduBot, özellikle **Gemini AI tuned model** ile en başarılı sonuçları elde etmiştir. Türkçe veri bilimi sorularında %85+ doğruluk oranı sağlamaktadır.

## 🤝 Katkıda Bulunma

Bu proje açık kaynak kodludur. Katkılarınızı bekliyoruz:
1. Fork yapın
2. Feature branch oluşturun
3. Değişikliklerinizi commit edin
4. Pull request gönderin


## 👥 Geliştirici

**Murat Görkem Çoban** - Veri Bilimi ve Makine Öğrenmesi Uzmanı
**Begüm Erva Şahin** - Veri Bilimi ve Makine Öğrenmesi Uzmanı


## 📞 İletişim

Sorularınız için GitHub Issues kullanabilirsiniz.

---

⭐ **Projeyi beğendiyseniz star vermeyi unutmayın!**

🚀 **EduBot ile veri bilimi öğrenmeniz artık daha kolay!**
