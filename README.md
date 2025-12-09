📊 MentalHealthPredict – Depresyon ve Ruhsal Hastalık Geçmişinin Tahmini

Bu proje, bireylerin **depresyon ve ruhsal hastalık geçmişini** (History of Mental Illness – 0/1) tahmin etmek amacıyla veri madenciliği ve makine öğrenmesi yöntemlerinin karşılaştırıldığı bir sınıflandırma çalışmasıdır.
Veri seti 413.768 gözlem ve 15 özellikten oluşmaktadır.

Proje kapsamında:

* Veri ön işleme
* Özellik seçimi (Chi², MI, VarianceThreshold, SelectKBest)
* Boyut indirgeme (PCA)
* Farklı sınıflandırma modelleri
* Model performans karşılaştırmaları

gerçekleştirilmiştir.

---

📁 Proje Yapısı

Proje üç ekip üyesi tarafından yürütülmüştür ve her üye kendi Jupyter Notebook dosyasında aşağıdaki modelleri geliştirmiştir:

| Üye         | Görevler ve Modeller                                     |
| ----------- | -------------------------------------------------------- |
| **Wisam**   | Feature Selection, PCA, Logistic Regression              |
| **Mustafa** | KNN, GaussianNB, SelectKBest, PCA                        |
| **Cüneyd**  | Logistic Regression & Decision Tree + Mutual Information |

Tüm üyeler veri ön işleme, model oluşturma ve görselleştirme adımlarını kendi defterlerinde gerçekleştirmiştir.

---

🎯 Projenin Amacı

* Ruhsal hastalık geçmişi olan bireyleri sınıflandırmak
* Özellik seçimi yöntemlerinin model performansına etkisini değerlendirmek
* PCA’nin boyut indirgeme sonrası doğruluk üzerindeki etkisini incelemek
* En iyi sonuç veren model ve özellik setini belirlemek

---

🛠 Kullanılan Yöntemler

🔹 Veri İşleme

* Label Encoding
* Hedef dağılım analizi
* Outlier incelemesi
* Eksik değer kontrolü

🔹 Özellik Seçimi

* Chi-Square
* Mutual Information
* VarianceThreshold
* SelectKBest (k=10, 30)

🔹 Boyut İndirgeme

* PCA (n_components değişimi ile performans analizi)

🔹 Kullanılan Modeller

* Logistic Regression
* Decision Tree Classifier
* K-Nearest Neighbors
* Gaussian Naive Bayes
* FS + PCA + Model kombinasyonları

---

📈 Sonuçların Özeti

Genel olarak:

* **AUC** değerleri en yüksek LR + MI ve GaussianNB modellerinde görülmüştür.
* **F1 skorları** sınıf dengesizliği nedeniyle düşüktür.
* PCA bazı modellerde performansı artırmazken bazı modellerde küçük iyileşme sağlamıştır.
* Özellik seçimi bazı durumlarda overfitting’i azaltmıştır.

---

📉 Confusion Matrix Görselleri

Her notebook dosyasında tüm modeller için Confusion Matrix grafikleri oluşturulmuştur.

---

🧠 Ekip

* **Wisam**
* **Mustafa**
* **Cüneyd**

Grup Adı: **DigitalNomads**

---

🧰 Kullanılan Teknolojiler

* Python 3.x
* Pandas, NumPy
* Scikit-learn
* Matplotlib, Seaborn
* Jupyter Notebook

---

🔧 Nasıl Çalıştırılır?

```bash
git clone <repo-link>
cd MentalHealthPredict
jupyter notebook
```

Notebook dosyalarından herhangi birini açarak modeli çalıştırabilirsiniz.


📄 Lisans

Bu proje yalnızca **akademik amaçlıdır**; ticari kullanım yasaktır.


