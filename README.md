Bu proje, hava kirliliği verilerini analiz ederek PM2.5 ve PM10 partiküllerinin dağılımını incelemeyi amaçlamaktadır. 
Proje kapsamında çeşitli istatistiksel analizler ve görselleştirmeler yapılmıştır.
Veriler, farklı zaman dilimlerine göre hava kalitesini değerlendirmek için kullanılabilir.

Veri Seti
Veri seti, hava kirliliği ile ilgili çeşitli parametreleri içermektedir.
Ana hedef, PM2.5 ve PM10 seviyelerinin nasıl dağıldığını ve bu seviyelerin hangi koşullarda yüksek olduğunu incelemektir.

Veri Seti Özellikleri:
PM2.5: 2.5 mikrometreden küçük partiküller.
PM10: 10 mikrometreden küçük partiküller.
Tarih/Zaman: Ölçüm tarihleri ve saatleri.
Hava Durumu Parametreleri: Sıcaklık, nem, rüzgar hızı vb.
Kullanılan Kütüphaneler
Bu proje Python ve bazı popüler veri analizi kütüphaneleri kullanılarak geliştirilmiştir:

Pandas: Veri manipülasyonu ve analiz için.
Matplotlib & Seaborn: Veri görselleştirmeleri için.
Scikit-learn: Makine öğrenmesi algoritmalarının uygulanması için.
Numpy: Sayısal hesaplamalar için.
Analiz ve Sonuçlar
Proje boyunca PM2.5 ve PM10 verileri üzerinde yapılan analizler şunları içermektedir:

Veri Temizleme ve Ön İşleme: Eksik veriler ve aykırı değerler temizlendi.
Dağılım Analizleri: PM2.5 ve PM10 partiküllerinin zaman içerisindeki dağılımı incelendi.
Korelasyon Analizi: PM2.5 ve PM10 ile diğer hava durumu parametreleri arasındaki ilişkiler incelendi.
Tahmin Modelleri: PM2.5 ve PM10 seviyelerinin gelecekteki değerlerini tahmin etmek için zaman serisi modelleme yapıldı.
Kullanım
Gereksinimler:
Proje için Python 3.6+ ve aşağıdaki kütüphaneler gereklidir:

bash
Kodu kopyala
pip install pandas numpy matplotlib seaborn scikit-learn
Çalıştırma:
Veri Seti: data.csv dosyasını indirin ve projenizin kök dizinine yerleştirin.
Analiz ve Modelleme: analysis.py dosyasını çalıştırarak verilerinizi analiz edebilirsiniz.
Örnek Kullanım:
python
Kodu kopyala
import pandas as pd

# Veri setini yükleyin
data = pd.read_csv('data.csv')

# PM2.5 ve PM10 dağılımını çizdirin
import matplotlib.pyplot as plt
import seaborn as sns

sns.kdeplot(data['PM2.5'], color='blue', label='PM2.5')
sns.kdeplot(data['PM10'], color='red', label='PM10')
plt.title('PM2.5 ve PM10 Dağılımı')
plt.xlabel('PM2.5 ve PM10 Değerleri')
plt.ylabel('Count')
plt.legend()
plt.show()
Sonuç ve Öneriler
Proje, hava kalitesini anlamak ve bu verileri çeşitli uygulamalarda kullanmak adına önemli bilgiler sunmaktadır.
Özellikle PM2.5 ve PM10 seviyelerinin dağılımları, hava kirliliği yönetim politikaları için kritik veriler sunabilir. 
Çevre kirliliği ile mücadelede bu tür analizlerin düzenli olarak yapılması tavsiye edilmektedir.
