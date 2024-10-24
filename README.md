# A-Large-Scale-Fish-Dataset-DeepLearning-

## Kaggle Link
https://www.kaggle.com/code/ahmetfurkankaya/notebook5e414c7f4e

Bu proje, A Large-Scale Fish Dataset'i kullanarak balık türlerini sınıflandırmayı hedefleyen bir görüntü sınıflandırma uygulamasıdır. Projede Derin Öğrenme (Deep Learning) teknikleri ve Yapay Sinir Ağı (ANN) mimarisi kullanılmıştır. Eğitim ve test verileri üzerinde görüntü işleme, veri artırma, model oluşturma ve hiperparametre optimizasyonu gibi çeşitli adımlar gerçekleştirilmiştir.

#Proje Adımları
## 1. Geliştirme Ortamı ve Kütüphaneler
Proje Python programlama dili ile geliştirilmiş olup, TensorFlow ve Keras gibi kütüphaneler kullanılmıştır. Aşağıdaki kütüphaneler projede yer almıştır:

Numpy: Sayısal işlemler için.
Pandas: Veri çerçevesi oluşturma ve işleme.
Matplotlib: Görselleştirme için.
TensorFlow ve Keras: Derin öğrenme modelleri oluşturma ve eğitme.
scikit-learn: Veri bölme ve hiperparametre optimizasyonu için.
## 2. Veri Setinin Yüklenmesi
A Large-Scale Fish Dataset Kaggle platformundan alınarak proje ortamına yüklenmiştir. Veri setinde çeşitli balık türlerine ait görüntüler bulunmaktadır. Görüntüler, balık türlerine göre klasörlenmiştir.

## 3. DataFrame Oluşturma
Veri setindeki görüntü dosyalarının yol bilgileri ve etiketler (balık türleri) ile bir DataFrame oluşturulmuştur:
