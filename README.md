# TestScope AI - Çevresel Test Risk Tahmin Sistemi

TestScope AI, MIL-STD-810 ve ISO 16750 gibi çevresel test standartlarını temel alarak test senaryolarını simüle eden ve yapay zekâ destekli risk analizi gerçekleştiren bir uygulamadır. Sıcaklık, nem, titreşim ve basınç gibi çevresel parametreleri analiz ederek risk seviyelerinin değerlendirilmesini ve görselleştirilmesini sağlar.

## Özellikler

### **Çoklu Standart Desteği**
- MIL-STD-810, ISO 16750 gibi test standartlarına göre hazır senaryolar

### **Hazır Test Senaryoları**
- Tek tıklama ile standartlara uygun sabit değerlerin otomatik yüklenmesi

### **Yapay Zeka Destekli Analiz**
- Makine öğrenmesi algoritmaları (Random Forest %91.2 doğruluk) ile risk tahmini

### **Görselleştirilmiş Sonuçlar**
- Gauge chart ve bar chart ile risk seviyelerinin görsel analizi
- **Yeni:** İyileştirilmiş kullanıcı arayüzü - yumuşak renk tonları ve tutarlı tasarım

### **Parametre Bazlı Risk Analizi**
- Sıcaklık, nem, titreşim ve basınç değerlerinin ayrı ayrı değerlendirilmesi

### **Gelişmiş Kullanıcı Deneyimi**
- **Renk Tutarlılığı:** Tüm yeşil tonlar aynı renk paletinde
- **Yumuşak Kontrast:** FAIL durumu için yumuşak kırmızı tonlar
- **İkon Hizalama:** Tüm ikonlar metinlerle mükemmel hizalanmış
- **Tipografi:** Büyük ve kalın yüzdeler, okunabilirlik artırıldı
- **Eşit Boşluklar:** Tüm kartlar arasında tutarlı margin
- **Açıklayıcı Metrikler:** Tooltip'ler ve daha anlaşılır isimler
- **Renk Kodlaması:** Tahmin Güveni (mavi), Risk Seviyesi (yeşil), PASS Olasılığı (yeşil)
- **Temiz Tasarım:** Sadece gerekli metrikler gösteriliyor

## Test Parametreleri

| Parametre | Aralık | Birim |
|-----------|--------|-------|
| Sıcaklık | -40°C ile +85°C | °C |
| Nem | %10 ile %95 | % |
| Titreşim | 0.1g ile 10g | g |
| Basınç | 800hPa ile 1200hPa | hPa |

## 🎮 Kullanım

### **1. Test Standardını Seçin**
MIL-STD-810, ISO 16750 gibi uygun standardı seçin.

### **2. Hazır Test Senaryosu Yükleyin**
Tek tıkla standart değerler otomatik yüklensin.

### **3. Parametreleri Düzenleyin**
Sıcaklık, nem, titreşim ve basınç değerlerini isteğe göre değiştirin.

### **4. Risk Analizi Yapın**
"Risk Analizi Yap" butonuna tıklayarak yapay zeka destekli analiz başlatın.

### **5. Sonuçları İnceleyin**
Risk yüzdesi, risk seviyesi ve parametre bazlı analizleri görüntüleyin.

## 🛠️ Teknolojiler

- **Python**: Ana programlama dili
- **Streamlit**: Web arayüzü
- **Plotly**: Görselleştirmeler
- **Scikit-learn**: Makine öğrenmesi
- **Pandas / NumPy**: Veri işleme

## Risk Değerlendirme

- **Düşük Risk (0-30%)**: ✅ Test başarılı
- **Orta Risk (30-70%)**: ⚠️ Dikkat gerekli  
- **Yüksek Risk (70-100%)**: ❌ Test başarısız

## 🛠️ Kurulum

```bash
# 1. Repository'yi klonlayın
git clone https://github.com/username/testscope-ai.git
cd testscope-ai

# 2. Sanal ortam oluşturun
python -m venv .venv
source .venv/bin/activate  # Linux/Mac
# veya
.venv\Scripts\activate     # Windows

# 3. Bağımlılıkları yükleyin
pip install -r requirements.txt

# 4. Uygulamayı başlatın
streamlit run app.py
```

## 📁 Proje Yapısı

```
TestScope AI/
├── app.py              # Ana Streamlit uygulaması
├── models/             # AI modelleri ve eğitim
├── utils/              # Veri işleme ve görselleştirme
├── data/               # Test verileri
└── notebooks/          # Analiz raporları
```

## AI Modelleri

- **Random Forest**: %91.2 doğruluk oranı
- **Logistic Regression**: %70 doğruluk oranı
- **Otomatik Model Seçimi**: En iyi performans gösteren model

## Görselleştirmeler

- **Risk Gauge**: Dairesel risk göstergesi
- **Radar Grafiği**: Parametre risk analizi
- **Bar Grafikleri**: Risk faktörleri karşılaştırması
- **Trend Analizi**: Geçmiş test sonuçları
