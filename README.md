# AKBANK-DERIN-OGRENME-BOOTCAMP

# Derin Öğrenme Projesi: Balık Sınıflandırma

Bu proje, Kaggle'daki büyük ölçekli balık veri seti kullanarak derin öğrenme ile balık sınıflandırması yapmayı amaçlamaktadır. Proje, derin öğrenme alanında başlangıç düzeyinde pratik deneyim kazanmayı hedefler.

## Proje İçeriği

- Veri seti: [A Large Scale Fish Dataset](https://www.kaggle.com/datasets/crowww/a-large-scale-fish-dataset/data)
- Kütüphaneler: `TensorFlow`, `Keras`, `Pandas`, `Matplotlib`
- Kullanılan model: Yapay Sinir Ağı (ANN)
- Eğitim: Veri artırma kullanılarak eğitim gerçekleştirilecektir.
- **Kaggle Notebook Linki**: https://www.kaggle.com/code/erenefeorhan/deeplearning

## Geliştirme Ortamı

Proje, Kaggle ortamında geliştirilmektedir. Kaggle üzerinde oluşturduğunuz bir notebook üzerinde çalışmanız beklenmektedir.

### Gereksinimler

Projenin çalışabilmesi için aşağıdaki kütüphanelerin yüklü olması gerekmektedir:

```bash
pip install tensorflow pandas matplotlib
```
Veri Ön İşleme
Veri seti, klasörler içinde yer alan .png formatındaki fotoğraflardan oluşmaktadır. Bu aşamada aşağıdaki işlemler gerçekleştirilmiştir:
Görsellerin yolları ve etiketleri toplandı.
Bir Pandas DataFrame oluşturuldu.
Veri artırma teknikleri uygulandı.

Model Eğitimi
Model, aşağıdaki mimari ile oluşturulmuştur:
Giriş Katmanı: 150x150 piksel
Düzleştirme Katmanı
Gizli Katman: 128 düğüm, ReLU aktivasyon fonksiyonu
Dropout Katmanı: %50 dropout oranı
Çıkış Katmanı: Sınıf sayısına göre softmax aktivasyonu

Modeli Derleme
Model, aşağıdaki metriklerle derlenmiştir:
Optimizer: Adam
Kayıp Fonksiyonu: Categorical Crossentropy
Metrikler: Doğruluk (Accuracy)

Sonuçlar
Model, eğitim sürecinde doğruluk ve kayıp fonksiyonu gibi metriklerle değerlendirilecektir. Eğitim süreci sonunda modelin performansı incelenecektir.

