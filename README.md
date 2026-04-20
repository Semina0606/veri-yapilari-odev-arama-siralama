# Veri Yapıları ve Algoritmalar Ödevi - Semina Kılınç

Bu repository içerisinde, veri yapıları dersinde işlediğimiz temel arama ve sıralama algoritmalarının Python uygulamaları yer almaktadır. Kodları yazarken her algoritmanın çalışma performansını (hızını) ölçebilecek bir yapı kurguladım.

## Proje İçeriği

Bu çalışmada hem klasik sıralama yöntemlerini hem de verimli arama tekniklerini fonksiyonel bir yapıda hazırladım. Kodun içinde bulunan `performans_izleyici` sayesinde, hangi algoritmanın veri setini ne kadar sürede işlediğini net bir şekilde raporlayabiliyoruz.

### Kullanılan Algoritmalar

**1. Sıralama Algoritmaları:**
* **Kabarcık Sıralama (Bubble Sort):** Elemanları tek tek karşılaştırarak yer değiştiren temel yöntem.
* **Seçmeli Sıralama (Selection Sort):** Listenin en küçük elemanını bulup başa taşıyarak ilerler.
* **Araya Ekleme (Insertion Sort):** Sayıları sıralı bir diziye ekliyormuş gibi uygun yerine yerleştirir.
* **Hızlı Sıralama (Quick Sort):** Parçala ve yönet mantığıyla çalışan, en hızlı sonuç veren algoritmalardan biridir.

**2. Arama Algoritmaları:**
* **Doğrusal Arama (Linear Search):** Hedef veriyi bulana kadar listeyi baştan sona tarar.
* **İkili Arama (Binary Search):** Sıralı listeyi sürekli ikiye bölerek hedefe çok hızlı ulaşır.

## Performans Raporu (Zaman Karmaşıklığı)

Algoritmaların teorik çalışma hızları aşağıdaki gibidir:

| Algoritma | Karmaşıklık (En Kötü) |
| :--- | :--- |
| Quick Sort | O(n log n) |
| Bubble Sort | O(n^2) |
| Binary Search | O(log n) |
| Linear Search | O(n) |

## Nasıl Kullanılır?
Terminal üzerinden `python main.py` komutuyla programı çalıştırabilirsiniz. Program çıktı olarak orijinal diziyi, sıralanmış hali ve algoritmaların ms cinsinden çalışma sürelerini ekrana basacaktır.

---
**Öğrenci:** Semina Kılınç  
**Bölüm:** Yapay Zeka Operatörlüğü  
**Ders:** Veri Yapıları
