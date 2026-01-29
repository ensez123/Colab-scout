[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ensez123/Colab-scout/blob/main/Untitled0.ipynb)

# Colab-scout: Veri Odaklı Futbol Scouting Sistemi

Bu proje, Google Colab ortamında geliştirilmiş, veri madenciliği ve makine öğrenmesi tekniklerini kullanan kapsamlı bir futbolcu izleme (scouting) ve analiz sistemidir.

## Projenin Amacı
Sentetik veya gerçek oyuncu verilerini kullanarak; performans metriklerini standartlaştırmak, makine öğrenmesi modelleriyle piyasa değeri tahmini yapmak ve interaktif dashboardlar aracılığıyla "gizli yetenekleri" (underrated players) keşfetmektir.

## Temel Özellikler
- **Sentetik Veri Üretimi:** Sözleşme detayları ve lig kalitesi gibi faktörleri içeren detaylı oyuncu veri seti oluşturma.
- **Veri Önişleme:** Per-90 metrikleri, Min-Max normalizasyon ve IQR ile aykırı değer temizliği.
- **XGBoost Regresyon:** Oyuncu performansına dayalı piyasa değeri tahmini ve hiperparametre optimizasyonu.
- **Opportunity Index:** Model tahmini ile gerçek piyasa değeri arasındaki farka dayalı fırsat analizi.
- **Benzer Oyuncu Bulucu:** Cosine Similarity kullanarak benzer profildeki oyuncuları tespit etme.
- **İnteraktif Dashboard:** Plotly Radar Chart ve ipywidgets ile dinamik oyuncu analizi.

## Proje Değerlendirmesi (Analiz Raporu)

### 1. Kod Kalitesi
*   **Modüler Yapı:** Dashboard ve analiz fonksiyonları modüler bir yapıda tasarlanmış. Hata yönetimi (`try-except`) başarıyla uygulanmış.
*   **Gelişim Alanı:** Kod tekrarlarını azaltmak için veri üretim ve modelleme adımları merkezi fonksiyonlarda toplanabilir.

### 2. Model Performansı
*   **Başarı:** XGBoost algoritması ve çapraz doğrulama (cross-validation) teknikleri modelin doğruluğunu artırmak için doğru kullanılmış.
*   **Gelişim Alanı:** Gerçek dünya verileriyle modelin genelleme yeteneği daha fazla test edilebilir.

### 3. Veri Analizi Yöntemleri
*   **Analitik Yaklaşım:** Per-90 standardizasyonu ve "Opportunity Index" gibi metrikler, scouting dünyasındaki güncel analitik yaklaşımlarla örtüşüyor.
*   **Normalizasyon:** Verilerin ölçeklendirilmesi, çok boyutlu analizleri (Radar Chart gibi) daha anlamlı kılıyor.

### 4. Görselleştirme
*   **Kullanıcı Deneyimi:** Plotly grafikleri interaktiflik sunarken, ipywidgets arayüzü projenin bir uygulama gibi çalışmasını sağlıyor.

---
