# Makemore Projesi

Bu proje, Andrej Karpathy'nin "makemore" serisinden esinlenilerek oluşturulmuş bir karakter-seviyesi dil modelidir. Model, verilen örnek kelimelere benzer yeni kelimeler üretmeyi öğrenir.

## Proje Hakkında

Bu proje şunları içerir:
- Karakter tabanlı dil modeli implementasyonu
- PyTorch kullanarak sinir ağı uygulaması
- Kelime üretimi için bigram modeli
- Eğitim sürecinin görselleştirilmesi

## Kurulum

1. Gerekli paketleri yükleyin:
```bash
pip install torch numpy matplotlib jupyter
```

2. Projeyi klonlayın:
```bash
git clone https://github.com/[kullanıcı-adınız]/micrograd.git
cd micrograd
```

## Kullanım

1. Jupyter Notebook'u başlatın:
```bash
jupyter notebook
```

2. `makemore.ipynb` dosyasını açın
3. Notebook'taki hücreleri sırasıyla çalıştırın

## Veri Seti

Proje, `names.txt` dosyasındaki isimleri kullanarak eğitilir. Bu dosya her satırda bir isim içerir.

## Model Detayları

- Girdi: Karakter dizileri
- Çıktı: Sonraki karakterin olasılık dağılımı
- Eğitim: Cross-entropy loss kullanılarak gradient descent
- Aktivasyon: Tanh ve Softmax fonksiyonları

## Lisans

Bu proje MIT lisansı altında lisanslanmıştır. Detaylar için `LICENSE` dosyasına bakınız.

## Katkıda Bulunma

1. Bu depoyu fork edin
2. Yeni bir branch oluşturun (`git checkout -b yeni-ozellik`)
3. Değişikliklerinizi commit edin (`git commit -am 'Yeni özellik eklendi'`)
4. Branch'inizi push edin (`git push origin yeni-ozellik`)
5. Pull Request oluşturun
