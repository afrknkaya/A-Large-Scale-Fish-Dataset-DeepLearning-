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
Veri setindeki görüntü dosyalarının yol bilgileri ve etiketler (balık türleri) ile bir DataFrame oluşturulmuştur.

## 4. Eğitim ve Test Kümelerine Ayırma
Veri seti eğitim ve test kümelerine %80 eğitim, %20 test olacak şekilde ayrılmıştır. Stratified sampling yöntemi ile her sınıfın dengeli olmasına dikkat edilmiştir

## 5. Görüntü İşleme ve Veri Artırma
Görüntüler, 150x150 piksel boyutuna küçültülmüştür. Ayrıca, eğitim sürecinde görüntüleri normalleştirmek için ImageDataGenerator kullanılmıştır

## 6. Model Oluşturma
Proje kapsamında bir Yapay Sinir Ağı (ANN) modeli oluşturulmuştur. Modelin mimarisi şu şekildedir:

Flatten: Görüntülerin çok boyutlu yapısını düzleştirme.
Dense (128 ve 64 nöronlu katmanlar): Gizli katmanlar, her bir katmandan sonra %50 Dropout eklenmiştir.
Dense (Çıkış katmanı): Balık sınıflarını tahmin etmek için softmax aktivasyon fonksiyonu kullanılmıştır.

## 7. Model Eğitimi
Model 10 epoch boyunca eğitim ve test verisi üzerinde eğitilmiştir. Eğitim esnasında doğrulama doğruluğu ve kaybı takip edilmiştir:


## 8. Model Performansı
Modelin doğruluğu ve kaybı görselleştirilmiştir. Eğitim ve doğrulama verileri üzerinde elde edilen doğruluk oranları şu şekildedir:


## 9. Test Sonuçları
Test veri setinde modelin doğruluğu %5,5 civarında ölçülmüştür:


## 10. Hiperparametre Optimizasyonu
En iyi öğrenme oranını bulmak için GridSearch ile hiperparametre optimizasyonu yapılmıştır:


## Sonuçlar
Bu proje kapsamında balık sınıflarını tanımak için bir yapay sinir ağı oluşturulmuş, model eğitilmiş ve doğrulama seti ile test edilmiştir. Doğruluğu arttırmak için hiperparametre optimizasyonu ve farklı model mimarileri denenebilir.
