# 🧠 Brain Tumor Detection and Segmentation with YOLOv2 and Medical SAM
Bu proje, beyin tümörü bulunan MRI görüntülerinde tümör bölgelerini tespit etmek ve bu bölgeleri segment etmek amacıyla gerçekleştirilmiştir. Derin öğrenme tabanlı bu sistemde, tümörler öncelikle YOLOv2 nesne tespiti algoritması ile belirlenmiş, ardından tespit edilen bölgeler Medical SAM (Segment Anything Model) kullanılarak detaylı bir şekilde boyanmıştır.

📁 Proje Yapısı

📂Models
📂Kaynakça
📄yolovGUI.mlapp
📄DerinÖğrenmeRapor

###👥 Ekip
Bu proje, Derin Öğrenme dersi kapsamında 5 kişilik bir ekip tarafından geliştirilmiştir. Her ekip üyesi farklı bir ağ modeli eğitip nesne tespiti gerçekleştirmiştir.

Modeller:

- Squeezenet
- ResNet50
- ResNet18
- VGG16
- MobileNetV2

## 🔍 Kullanılan Yöntemler
✅ YOLOv2 (You Only Look Once v2)
- Eğitim MATLAB ortamında gerçekleştirilmiştir.

- Eğitim verileri, beyin tümörleri içeren MRI görüntülerinden oluşmaktadır.

- Model, tümör içeren alanları bounding box ile işaretlemektedir.
  
✅ Medical SAM (Segment Anything Model for Medical Images)
- Bounding box ile tespit edilen tümör bölgeleri, Medical SAM ile segment edilmiştir.

- Segmentasyon işlemi MATLAB ortamında gerçekleştirilmiştir.

- Her bounding box’ın içindeki piksel düzeyinde segmentasyon yapılmıştır.

## 🗂️ Veri Seti
Kaynak: Kaggle - Brain MRI Images for Brain Tumor Detection

- Veri Türü: Gri ölçekli MRI görüntüleri

Sınıflar:

- Tümör Var

## 🔧 Veri Ön İşleme
- Görüntü formatları .jpg formatına dönüştürüldü.

- Boyutlar 416x416 piksel (YOLOv2 için) olarak yeniden boyutlandırıldı.

- Segmentasyon işlemleri öncesi, bounding box'lar normalize edildi.

## 📊 Değerlendirme Metrikleri
YOLOv2 için:

- Precision, Recall, mAP

Segmentasyon için:

- IoU (Intersection over Union)

- Dice Coefficient

## 📌 Sonuçlar
YOLOv2, MRI görüntülerindeki tümörleri başarılı şekilde tespit etti.

Medical SAM ile birlikte, tespit edilen tümörlerin segmentasyonu daha hassas hale getirildi.

Modelin çıktıları, görsel analizlerle başarıyla doğrulandı.

Bu çalışma, tıbbi görüntü işleme alanında çok aşamalı bir derin öğrenme yaklaşımının etkinliğini göstermektedir.

## 🖼️ Ekran Görüntüleri
Aşağıda, uygulamaya ve eğitim sonuçlarına ait bazı ekran görüntüleri yer almaktadır. Bu görseller, grafiksel kullanıcı arayüzünü, model tahminlerini ve proje süresince elde edilen performans metriklerini göstermektedir.

## Uygulama Ana Ekranı
![Uygulama Ana Ekranı](https://github.com/user-attachments/assets/27945626-b572-4377-a614-b072f720a8a1)

## Model Seçimi
![Model Seçimi ](https://github.com/user-attachments/assets/099002ac-7626-4acf-b365-02faabe14499)

## Model Yükleme
![Model Yükleme](https://github.com/user-attachments/assets/0e53794a-76a9-4998-ac89-08fdf6dd6d5a)

## Görsel Seçimi
![Görsel Seçimi](https://github.com/user-attachments/assets/b1b47698-1903-468b-bbc7-6bc3fc263476)

## Görsel Yükleme
![resim yükleme](https://github.com/user-attachments/assets/0d9d726e-bc8e-4a15-860f-b227f075f132)

## Tespit
![tespit](https://github.com/user-attachments/assets/f411d957-da5b-4bbb-adca-304a74a8e28b)

## Medical SAM ile Boyama
![boyama](https://github.com/user-attachments/assets/aaaf9a50-5e7c-46c3-8638-4124ed1b6884)
