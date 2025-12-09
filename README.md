# Forest Fires — Lojistik Regresyon Analizi

Bu proje, Portekiz'in Montesinho bölgesinde 2000–2003 yılları arasında kaydedilmiş orman yangını verileri kullanılarak yangın oluşup oluşmayacağının lojistik regresyon modeli ile tahmin edilmesini amaçlamaktadır.

## Projenin Amacı
Çevresel, meteorolojik ve yangın riski ile ilişkili değişkenler kullanılarak, bir yangının meydana gelip gelmeyeceğini tahmin eden ikili (binary) sınıflandırma modeli kurulmuştur. 
Model, veri ön işleme, modelleme, doğrulama ve değerlendirme adımlarından oluşmaktadır.

## Kullanılan Veri Seti
Forest Fires veri seti aşağıdaki değişkenleri içermektedir:

### Konumsal Değişkenler
- X, Y: Coğrafi koordinatlar

### Yangın Risk İndeksleri
- FFMC: İnce yanıcı maddelerin kuruluk derecesi  
- DMC: Orta vadeli kuraklık indeksi  
- DC: Uzun vadeli kuraklık indeksi  
- ISI: Yangının başlangıç yayılma hızı  

### Meteorolojik Değişkenler
- temp: Sıcaklık (°C)  
- RH: Bağıl nem (%)  
- wind: Rüzgar hızı (km/h)  
- rain: Yağış miktarı (mm)  

### Hedef Değişken
- fire:  
  - 1 → Yangın var  
  - 0 → Yangın yok  

## Yapılan İşlemler
- Eksik veri analizi  
- Kategorik değişkenlerin one-hot encoding ile dönüştürülmesi  
- Yeni hedef değişkeninin (fire) oluşturulması  
- Eğitim–test ayrımı (stratified split)  
- Lojistik regresyon modeli kurulumu  
- Model performans metrikleri: Accuracy, Precision, Recall, F1-score  
- Confusion Matrix görselleştirilmesi  
- Korelasyon analizi ve ısı haritası  

## Model Performansı
Model genel olarak anlamlı bir doğruluk oranı elde etmiş ve yangın var/yok durumunu başarılı şekilde sınıflandırmıştır.

## Sonuç
Lojistik regresyon modeli, çevresel değişkenler kullanılarak yangın çıkma olasılığını öngörmede etkili sonuçlar vermiştir. 
Model, veri analizi ve makine öğrenimi süreçlerinin bir örneğini temsil etmektedir.

## Geliştirici
Berkay Akçay  
2025 - Büyük Veri Analitiği (BDA) Vize Projesi
