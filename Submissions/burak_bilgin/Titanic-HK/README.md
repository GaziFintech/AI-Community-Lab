# 🚢 Proje: Titanic Sınıflandırma ve EDA Analizi

## 📌 Amaç
Bu proje, AI Community Lab "Veri Bilimi Başlangıç" (Bölüm 5) müfredatı kapsamında hazırlanmıştır. Kaggle'ın klasik Titanic veri seti kullanılarak uçtan uca bir veri bilimi süreci işletilmiştir. Projenin ana odak noktaları:
1. Keşifsel Veri Analizi (EDA) ile veri setindeki gizli örüntüleri (cinsiyet, bilet sınıfı ve yaşın hayatta kalmaya etkisi) görselleştirmek.
2. Eksik verileri doldurmak (Imputation) ve metinsel verileri makine öğrenimine uygun hale getirmek (Encoding).
3. Random Forest algoritması kullanarak bir sınıflandırma modeli kurmak, hiperparametre optimizasyonu ile skoru artırmak ve modelin tahmin yeteneğini detaylı olarak raporlamaktır.

## 🛠️ Kullanılan Teknolojiler
* **Programlama Dili:** Python
* **Veri Manipülasyonu:** Pandas
* **Görselleştirme:** Matplotlib, Seaborn
* **Makine Öğrenimi:** Scikit-learn (RandomForestClassifier, GridSearchCV, Confusion Matrix)

## 🚀 Nasıl Çalıştırılır?
Proje, tek bir Jupyter Notebook (`Titanic_Cozumu.ipynb`) dosyasından oluşmaktadır. 
Önceden herhangi bir CSV dosyası indirmenize gerek yoktur; kod, veriyi açık kaynaklı bir URL üzerinden `pandas` ile otomatik olarak çeker.
Aşağıdaki kütüphanelerin yüklü olduğundan emin olduktan sonra Google Colab veya yerel Jupyter ortamında hücreleri sırasıyla çalıştırabilirsiniz:
`pip install pandas scikit-learn matplotlib seaborn`

## 📊 Sonuçlar ve Çıktılar
* **EDA Çıktıları:** Yolcuların cinsiyet, bilet sınıfı ve yaş dağılımları görselleştirilmiş; hayatta kalma oranlarında 1. Sınıf yolcuların ve kadınların belirgin bir avantaja sahip olduğu saptanmıştır.
* **Model Performansı:** Kurulan temel (base) Random Forest modeli ile başlangıçta **%79.89** doğruluk (accuracy) elde edilmiştir.
* **Optimizasyon:** `GridSearchCV` kullanılarak hiperparametre optimizasyonu (ağaç sayısı, derinlik vb.) yapılmış ve modelin test seti üzerindeki doğruluk oranı **%81+** seviyesine çıkarılmıştır.
* **Değerlendirme:** Modelin tahmin gücü, Karmaşıklık Matrisi (Confusion Matrix) ısı haritası ile jüri sunumuna uygun formatta görselleştirilmiş ve test verisinden alınan rastgele örneklerle modelin başarılı/başarısız tahminleri yan yana listelenmiştir.