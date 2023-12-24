# Metrik Pengujian
### Silhouette Score<br>
Silhouette score adalah metrik evaluasi yang mengukur seberapa baik setiap data poin ditempatkan dalam klusternya sendiri dibandingkan dengan kluster sekitarnya. Silhouette score berkisar antara -1 hingga 1, di mana nilai yang tinggi menunjukkan bahwa objek berada dalam kluster yang sesuai, dan nilai yang rendah menunjukkan adanya tumpang tindih antar kluster. Berikut adalah formula untuk silhouette score:
<br>
<br>Silhouette Score = b-a/(max(a,b))<br>
<br>
Keterangan:
- a adalah rata-rata jarak antara suatu poin dengan semua poin dalam kluster yang sama.
- b adalah rata-rata jarak terdekat antara suatu poin dengan semua poin dalam kluster yang berbeda (kluster terdekat).<br>
<br>Secara umum, silhouette score dapat digunakan untuk memilih jumlah kluster yang optimal dalam metode K-means, di mana nilai tertinggi menunjukkan bahwa jumlah kluster yang dipilih memberikan pemisahan yang baik antar kluster.

# Hasil Evaluasi pada Coding
Dengan menggunakan nilai silhouette score, kita dapat memahami sejauh mana suatu poin berada dalam kluster yang sesuai dan sejauh mana kluster berbeda saling terpisah. Berikut adalah interpretasi nilai silhouette score:<br>
<br>1  : Poin berada dalam kluster yang sesuai.
<br>0  : Poin berada tepat di antara dua kluster.
<br>−1 : Poin lebih dekat dengan kluster sekitarnya daripada kluster tempat poin tersebut berada.<br>
<br>Pembahasan dengan topik "Analisis Segmetasi Pengunjung suatu Mall dengan Metode K-means Clustering menggunakan Elbow Method" mendapatkan hasil k=3 untuk jumlah cluster optimal berdasarkan _Elbow Method_. Kemudian dilakukan pengujian dengan _Silhouete Score_ dan mendapatkan hasil score tertinggi yaitu S=0.6508577554020604, engan jumlah cluster k=2<br>
<br>Maka berdasarkan hasil scorenya dibuatkan visualisasi persebaran titik-titik cluster sesuai dengan hasil perhitungannya. 
