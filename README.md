Fraud Detection in Credit Card Data using Unsupervised & Supervised Machine Learning
Proje Açıklaması

Bu proje, bir finansal işlem veri seti üzerinde hem gözetimli (supervised) hem de gözetimsiz (unsupervised) öğrenme algoritmalarını kullanarak 
dolandırıcılık tespiti ve veri kümesi içindeki yapıları keşfetmeye yönelik bir analiz gerçekleştirir. Veri seti, işlem detaylarını ve kullanıcı bilgilerini içermektedir.

Veri Seti

  Veri Seti Adı: fraudTrain.csv
  Açıklama: Bu veri seti, çeşitli finansal işlemleri içerir ve her bir işlem için dolandırıcılık (fraud) olup olmadığı bilgisi sağlar.
  Öznitelikler:
      'trans_date_trans_time': İşlem tarihi ve saati
      'cc_num': Kredi kartı numarası
      'merchant': Satıcı
      'category': Kategori
      'amt': İşlem miktarı
      'is_fraud': Dolandırıcılık (1: Evet, 0: Hayır)
      Diğer öznitelikler (örn. kullanıcı bilgileri, coğrafi bilgiler)

Veriyi İşleme

Veri Ön İşleme:
      Gereksiz sütunlar çıkarıldı: 'Unnamed: 0', 'first', 'last', 'state', 'city_pop', 'job', 'dob'
      Kategorik veriler one-hot encoding ile dönüştürüldü.
      Sayısal veriler standartlaştırıldı.

Modelleme:

  Gözetimli Öğrenme (Supervised Learning):
      Model: Lojistik Regresyon, Random Forest
      Performans Metrikleri: Doğruluk Skoru, Confusion Matrix, F1 Skoru
      Sonuç:                      
                            Doğruluk skoru
                  Algorithm	                Accuracy(Doğruluk)
            0	Logistic Regression	          0.993951
            1	Random Forest	                0.997396
                           Confusion Matrix
                  Algorithm	            Confusion Matrix
          0	Logistic Regression	    [[386650, 200], [2153, 0]]
          1	Random Forest	          [[386686, 164], [849, 1304]]
                              F1 Skoru
                Algorithm	               F1
          0	Logistic Regression	      0.000000
          1	Random Forest	            0.720243


  Gözetimsiz Öğrenme (Unsupervised Learning):
      Model: K-means Kümeleme
      Performans Metrikleri: Inertia, Silhouette Skoru
      Sonuç: 
  


Sonuç ve Öneriler

    Veri setinizin hem gözetimli hem de gözetimsiz öğrenme algoritmaları için ne kadar uygun olduğunu tartışın.
    Hangi öğrenme türünün belirli uygulamalar için daha uygun olduğunu ve olası gelecekteki analizler için önerilerde bulunun.
    [Gelecekte yapılabilecek iyileştirmeler veya ek analizler hakkında öneriler]
