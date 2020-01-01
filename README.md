# Kmeans

Benzer nesneleri birlikte gruplamayı zaten biliyorsunuz. Fikir çok basit olsa da, bu fikirden etkilenen kullanım durumlarının miktarı harikadır. Makine öğrenmesi literatüründe buna genellikle kümeleme denir — benzer nesneleri otomatik olarak aynı gruplara gruplandırır.

## Clustering
Kümeleme, verilerin yapısı hakkında bir sezgiyi elde etmek için kullanılan en yaygın keşifsel veri analizi tekniklerinden biridir. Farklı kümelerdeki veri noktaları çok farklıyken, aynı alt gruptaki (küme) veri noktalarının çok benzer olması nedeniyle verilerdeki alt grupların belirlenmesi görevi olarak tanımlanabilir. Bu yazıda, sadeliği nedeniyle en çok kullanılan kümeleme algoritmalarından biri olarak kabul edilen K-means algoritmasını ele alacağız.


### K-Means’ı Nerede Uygulayabiliriz?
Öncelikle bu algoritmayı nerelerde, hangi amaçlarda kullanabiliriz bunlara göz atalım. Bana göre bir algoritmayı incelemeye başlamadan önce onun neye hizmet ettiğini bilmek bizim çalışma verimimizi arttırır.
→Belge Sınıflandırması
Belgeleri etiketlere, konulara ve belgenin içeriğine göre birden fazla kategoride kümeleyin. Bu çok standart bir sınıflandırma problemidir ve k-means aracı bu amaç için oldukça uygun bir algoritmadır.
→Suç Yerlerinin Belirlenmesi
Bir şehirdeki belirli bölgelerde mevcut olan suçlarla ilgili veriler, suç kategorisi, suç alanı ve ikisi arasındaki ilişki, bir şehirdeki ya da bölgedeki suça eğilimli alanlara ilişkin kaliteli bilgiler verebilir.. gibi yerlerde kullanabiliriz.

### Denetimsiz Öğrenmenin(Unsupervised Learning) Anlamı:

K-Means algoritması bir unsupervised learning(gözetimsiz öğrenme) ve kümeleme algoritmasıdır.
Denetimsiz öğrenme, modeli denetlemeniz gerekmeyen bir makine öğrenme tekniğidir. Bunun yerine, modelin bilgi keşfetmek için kendi başına çalışmasına izin vermeniz gerekir. Temel olarak etiketlenmemiş verilerle ilgilenir.Denetimsiz öğrenme algoritmaları, denetimli öğrenmeye kıyasla daha karmaşık işlem görevlerini gerçekleştirmenizi sağlar.

#### Denetimsiz Öğrenimi kullanmanın başlıca nedenleri
- Denetimsiz makine öğrenmesi, verilerde her türlü bilinmeyen kalıpları bulur.
- Denetimsiz yöntemler, kategorizasyon için faydalı olabilecek özellikleri bulmanıza yardımcı olur.
- Gerçek zamanlı olarak gerçekleşir, bu nedenle tüm girdi verileri öğrenilenlerin varlığında analiz edilir ve etiketlenir.
- Etiketlenmemiş verileri bilgisayardan elde etmek, elle müdahale gerektiren etiketli verilerden daha kolaydır.

## Kümeleme Yöntemleri
Kümelerin verilerden oluşturulma şekline bağlı olarak, farklı kümeleme yöntemleri olabilir. Kurumlar tarafından yoğun olarak kullanılan en popüler kümelenme tekniklerine bir göz atalım. Bu türler:

 - ### Bölümleme yöntemleri(Partitioning methods):
Bölüm tabanlı kümeleme yöntemleri, verilen nesneleri, n boyutlu bir düzlemde rastgele veya belirli bazı nesnelerden uzaklıklarını ölçerek kümeler. Bu nedenle, bu yöntemler aynı zamanda mesafeye dayalı yöntemler olarak da bilinir.!
![bölümleme](https://miro.medium.com/max/530/1*Lt9OpyDIrhOpUZ6tPbMBzQ.png)

 - ### Hiyerarşik yöntemler(Hierarchical methods):
 Hiyerarşik kümeleme yöntemleri, bölümleme yöntemlerinden farklıdır. Veri noktalarını benzerliklerine göre seviyelere / hiyerarşilere ayırırlar. Bu seviyeler birlikte ağaç benzeri bir yapı oluşturur (dendrogram). Bu bölünme iki şekilde gerçekleşebilir — yukarıdan aşağıya ve aşağıdan yukarıya.
![hiyerarşik](https://miro.medium.com/max/450/1*I4aPYQpixu0cCTx39gPcBw.png)

- ### Yoğunluk bazlı yöntemler(Density-based methods)
 Veri noktalarının mesafesini göz önünde bulundurmak yerine, yoğunluğa dayalı kümeleme yöntemlerinde, bir mahalle kümeleri oluşturduğu düşünülmektedir. Komşuluk, verilen verilerden bir küme oluşturmak için ilgilenilen bir bölgede (tipik olarak başka bir veri noktası) bulunması gereken buradaki veri noktalarının sayısını ifade eder.
 ![yogunluk](https://miro.medium.com/max/609/1*M6sCAkRH9Q_LwbdlB0X27A.png)





