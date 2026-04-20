# Veri Yapıları ve Algoritmalar Ödevi - Semina Kılınç

Bu repository içerisinde, veri yapıları dersinde işlediğimiz temel arama ve sıralama algoritmalarının Python uygulamaları yer almaktadır. Kodları yazarken her algoritmanın çalışma performansını (hızını) ölçebilecek bir yapı kurguladım.

## Proje İçeriği

Bu çalışmada hem klasik sıralama yöntemlerini hem de verimli arama tekniklerini fonksiyonel bir yapıda hazırladım. Kodun içinde bulunan `performans_izleyici` sayesinde, hangi algoritmanın veri setini ne kadar sürede işlediğini net bir şekilde raporlayabiliyoruz.

### Kullanılan Algoritmalar

# Algoritma Rehberi

## 1. Sıralama Algoritmaları (Sorting Algorithms)
Sıralama algoritmaları, veriyi belirli bir düzene (küçükten büyüğe veya tam tersi) sokmak için kullanılır.

---

### **Kabarcık Sıralama (Bubble Sort)**
* **Mantık:** Dizinin başından başlar, yan yana duran iki elemanı karşılaştırır. Eğer soldaki sağdakinden büyükse yerlerini değiştirir. Bu işlem, en büyük eleman dizinin sonuna "baloncuk gibi" çıkana kadar tekrarlanır.
* **Karmaşıklık:** $O(n^2)$ (En kötü ve ortalama durum).
* **Kullanım:** Çok küçük veri setlerinde veya sadece eğitim amaçlı kullanılır; gerçek dünyada verimsizdir.

---

### **Seçmeli Sıralama (Selection Sort)**
* **Mantık:** Dizideki en küçük elemanı bulur ve onu birinci sıradaki elemanla takas eder. Sonra kalanlar içinden en küçüğü bulup ikinci sıraya koyar.
* **Karmaşıklık:** $O(n^2)$.
* **Kullanım:** Bellek kullanımı (takas sayısı) kısıtlı olduğunda tercih edilebilir, ancak genelde yavaştır.

---

### **Araya Ekleme (Insertion Sort)**
* **Mantık:** Elinizdeki iskambil kağıtlarını sıralamaya benzer. Dizinin her elemanını alıp kendisinden önceki sıralı kısımda uygun olan "boşluğa" yerleştirir.
* **Karmaşıklık:** $O(n^2)$ (En iyi durumda, yani dizi zaten sıralıysa $O(n)$).
* **Kullanım:** Neredeyse sıralanmış veri setlerinde veya çok küçük dizilerde inanılmaz hızlıdır.

---

### **Hızlı Sıralama (Quick Sort)**
* **Mantık:** Bir "Pivot" eleman seçilir. Pivot'tan küçük olanlar sola, büyük olanlar sağa toplanır. Ardından her iki taraf için aynı işlem tekrarlanır (Rekürsif).
* **Karmaşıklık:** Ortalama $O(n \log n)$, en kötü $O(n^2)$.
* **Kullanım:** Günümüzde sistem kütüphanelerinde (örneğin C++ `std::sort`) en çok kullanılan algoritmalardan biridir.

---

## 2. Arama Algoritmaları (Searching Algorithms)
Arama algoritmaları, bir veri kümesi içinde belirli bir değeri bulmak için tasarlanmıştır.

---

### **Doğrusal Arama (Linear Search)**
* **Mantık:** Bir kütüphanede kitabı raftaki en baştan başlayıp tek tek bakarak aramaya benzer. Listeyi 0. indisten son indise kadar tarar.
* **Karmaşıklık:** $O(n)$.
* **Kullanım:** Veriler sıralanmamışsa veya liste çok kısaysa kullanılır.
* **Dezavantaj:** Veri büyüdükçe (milyonlarca kayıt varsa) çok yavaşlar.

---

### **İkili Arama (Binary Search)**
* **Mantık:** **Şart:** Liste sıralı olmalıdır. Listenin tam ortasına bakar. Aranan sayı ortadaki sayıdan büyükse sağ tarafa, küçükse sol tarafa odaklanır. Her adımda arama alanını yarıya indirir.
* **Karmaşıklık:** $O(\log n)$.
* **Örnek:** 1 milyon kayıtlık bir listede Doğrusal Arama en kötü durumda 1.000.000 işlem yaparken, İkili Arama sadece yaklaşık 20 işlemde sonucu bulur.

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
