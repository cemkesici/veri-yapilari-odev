# Insertion Sort 

---
### [22,27,16,2,18,6]
* InsertionSort Türüne göre aşamaları
    * Algoritma soldan sağa doğru her çalıştığında bir sonraki indexten başlayacak şekilde çalışır. Küçükten büyüğe sıralama yapılacaksa kendisinden önceki eleman ile karşılaştırma yapar ve kendisinden önce eleman kalmayana kadar kontrol etmeye devam eder, önceki eleman kendisinden küçükse hiçbir işlem yapılmaz sonraki indekse geçilir fakat kendisinden büyükse yer değiştirirler 
    ---
    1.  |1.|*22|27|16|2|18|6|  
        |-|- |- |- |-|- |-|
        
        |2.|22|*27|16|2|18|6|  
        |-|-|-|-|-|-|-|

         |3.|22|27|*16|2|18|6|  
        |-|-|-|-|-|-|-|
        |3.|22|*16|27|2|18|6| 

        fakat hala önünde bir index olduğu için algoritma devam eder ve 16 ile 22 karşılaştırılır, 16 küçük olduğu için 22 ile yer değiştirilir ve sıradaki indexe geçilir

        |3.|22|*16|27|2|18|6| 
        |-|-|-|-|-|- |-|
        |3.|*16|22|27|2|18|6|  
         ---
        |4.|16|22|27|*2|18|6|
        |-|-|-|-|-|- |-|
        |4.|16|22|*2|27|18|6| 
        ---
        |4.|16|22|*2|27|18|6|
        |-|-|-|-|-|- |-|
        |4.|16|*2|22|27|18|6|
         ---
        |4.|16|*2|22|27|18|6|   
        |-|-|-|-|-|- |-|
        |4.|*2|16|22|27|18|6|
         ---
        |5.|2|16|22|27|*18|6|
        |-|-|-|-|-|- |-|
        |5.|2|16|22|*18|27|6|
        |5.|2|16|*18|22|27|6|
         ---
        |6.|2|16|18|22|27|*6|
        |-|-|-|-|-|- |-|
        |6.|2|16|18|22|*6|27|
        |6.|2|16|18|*6|22|27|
        |6.|2|16|*6|18|22|27|
        |6.|2|*6|16|18|22|27|
        
* Big o gösterimi 
    O(n^2)

    ---
* Sıralamaya göre    
    * Worst case: İstediğimiz sıralamaya göre tam tersi halde sıralanmış olması,
Küçükten büyüğe bir sıralama yapmak istediğimiz zaman en kötü senaryo büyükten küçüğe sıralanmış halidir
=n^2

    * Average case: Küçükten ve büyükten sıralamaya yakın bir şekilde dağılmış hali
    =n^2

    * Best case: Dizinin istediğimiz halde sıralanmış olarak verilmesi. =n

---

* Dizi sıralandıktan sonra 18 sayısını aramak istememiz sayının ortaya yakın noktada bulunması sebebiyle Average case olarak adlandırılabilir
#### [7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.

 |1.|*7|3|5|8|2|9|4|15|6|      
 |------|-|-|-|-|-|-|-|- |-|
 
 |2.|*3|7|5|8|2|9|4|15|6|      
 |------|-|-|-|-|-|-|-|- |-|
 
 |3.|3|*5|7|8|2|9|4|15|6|      
 |------|-|-|-|-|-|-|-|- |-|
 
 |4.|3|5|7|*8|2|9|4|15|6|      
 |------|-|-|-|-|-|-|-|- |-|
