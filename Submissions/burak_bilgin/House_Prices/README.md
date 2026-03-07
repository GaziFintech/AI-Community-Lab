# 🏡 Proje: House Prices Regresyon ve EDA Analizi

## 📌 Amaç
Bu proje, AI Community Lab "Veri Bilimi Başlangıç" (Bölüm 5) müfredatı kapsamında hazırlanmıştır. Kaggle'ın 'House Prices' veri seti kullanılarak 81 farklı sütuna sahip karmaşık emlak verileri üzerinde Keşifsel Veri Analizi (EDA) süreçleri işletilmiştir. Projenin ana hedefi, sürekli sayı tahmini yapılan Regresyon problemlerinin mantığını kavramak, veri setindeki eksiklikleri otomatik döngülerle gidermek ve Random Forest Regressor modeli ile ev fiyatlarını tahmin etmektir.

## 🛠️ Kullanılan Teknolojiler
* **Programlama Dili:** Python
* **Veri Manipülasyonu:** Pandas, Numpy
* **Görselleştirme:** Matplotlib, Seaborn
* **Makine Öğrenimi:** Scikit-learn (RandomForestRegressor, MAE, R2 Score)

## 🚀 Nasıl Çalıştırılır?
Proje, `.ipynb` formatında tek bir Jupyter Notebook dosyasından oluşmaktadır. Çalıştırmak için Kaggle üzerinden `train.csv` dosyasının indirilip not defterinin bulunduğu çalışma dizinine eklenmesi gerekmektedir. Gerekli kütüphaneler yüklendikten sonra hücreler sırayla çalıştırılabilir.

## 📊 Sonuçlar ve Çıktılar
* **EDA Çıktıları:** Evlerin satış fiyatı dağılımları, yaşam alanı büyüklüğü (GrLivArea) ve genel kalite (OverallQual) gibi kritik özelliklerin fiyat üzerindeki güçlü pozitif etkileri görselleştirilmiştir.
* **Veri Ön İşleme:** 81 sütunluk veri setindeki sayısal ve kategorik boşluklar otomatik döngülerle (`median` ve `mode` kullanılarak) doldurulmuş, kategorik veriler `get_dummies` ile sayısallaştırılmıştır.
* **Model Performansı:** Kurulan regresyon modeli ile test verisi üzerinde başarılı bir **R2 Skoru** elde edilmiş ve "Gerçek Fiyatlar vs Modelin Tahminleri" dağılım grafiği (scatter plot) ile modelin başarılı trend takibi kanıtlanmıştır.