# Selection-Sort-Projesi

Derslerde Selection Sort ve Insertion Sort aynıymış gibi anlatılmış fakat ödevi yaparken aynı olmadıklarını gördüm. Ben Selection Sort'a göre ödevimi yapacağım.

[22,27,16,2,18,6] -> Selection Sort

## Selection Sort
Selection Sort'a göre aşamalar
* [22,27,16,2,18,6]
* [2,27,16,22,18,6]--> En küçük sayıyı buluyoruz ve en başa yazıp diğer elemanla yer değiştiriyoruz. (n tane eleman)
* [2,6,16,22,18,27]--> (n-1) eleman içinden tekrar en küçük sayıyı bulup ikinci sıraya yazıyoruz.
* [2,6,16,18,22,27]--> küçükten büyüğe doğru sıralanmış oldu.

## Big-O gösterimi

lk adımda (n) eleman, ikinci adımda (n-1) eleman, üçüncü adımda (n-2) eleman ile işlem yaparak 1 eleman kalana kadar devam ediyoruz.

Formül--> n+(n-1)+(n-2)+...+1= n(n+1) /2

n^2+n /2 elde ettik. n^2 yi alıyoruz.
Sonuç--> O(n^2)

## Time Complexity

Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer?

[2,6,16,18,22,27]

Dizi sıralandıktan sonra 18 sayısı ortada olduğu için avarage case kapsamına girer.

## [7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımı

* [2,3,5,8,7,9,4,15,6]--> En küçük sayı ve en baştakini yer değiştir.
* [2,3,5,8,7,9,4,15,6]--> 3 doğru yerde.Dokunma.
* [2,3,4,8,7,9,5,15,6]--> 4 ve 5 yer değiştirir.
* [2,3,4,5,7,9,8,15,6]--> 5 ve 8 yer değiştirir.
* [2,3,4,5,6,9,8,15,7]--> 6 ve 7 yer değiştirir.
* [2,3,4,5,6,7,8,15,9]--> 7 ve 9 yer değiştirir.
* [2,3,4,5,6,7,8,15,9]--> 8 olması gerektiği yerde.
* [2,3,4,5,6,7,8,9,15]--> 9 ve 15 yer değiştirir.
