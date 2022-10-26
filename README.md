[Patika.dev](https://www.patika.dev/tr)

Proje 2
### [16, 21, 11, 8, 12, 22] -> Merge Sort

### Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
                 [16, 21, 11, 8, 12, 22]                  ( başlangıç)

          [16, 21, 11]            [8, 12, 22]             (dizi ikiye bölündü)

    [16, 21]      [11]            [8]     [12, 22]        ( sağ ve soldaki diziler tekrar ikiye bölündü)    
          
    [16]   [21]      [11]           [8]     [12]    [22]    (tek eleman kalana kadar dizi bir kez daha bölündü)
          
     [16, 21]      [11]           [8]     [12, 22]        (diziler birleştirilirken sıralandı)
     
        [11, 16, 21]                 [8, 12, 22]          (tekrar birleştirilirken sıralandı)
        
                 [8, 11, 12, 16, 21, 22]                  (son birleştirmede diziyi elde ediyoruz)
        

### Big-O gösterimini yazınız.
recursive bir fonksiyon olduğu için dizi tek eleman kalana kadar ikiye bölünmektedir. 2^x= n    logn= x
her bölünmüş dizinin merge işlemi için de dizinin uzunluğu kadar n işlemi yapılır.    O(n*(logn))  -->  O(6(log6)) 
