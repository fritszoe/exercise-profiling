# Reflection - Module 5

'''
Nama: Fatih Raditya Pratama
Class: AdPro-B
'''

## 1.) JMeter vs Intellij's Profiler

1. JMeter
JMeter digunakan untuk simulasi behaviour dan load user untuk mengukur performa aplikasi. Jadi, JMeter tidak secara langsung point out dimana letak
kesalahan kita, dan hanya akan memberikan gambaran dimana bagian yang perlu di optimized.
2. Intellij's Profiler
Di profiler Intellij, kita bisa secara detail melihat langsung performa dari app yang kita buat sehingga kita bisa langsung tahu bagian apa saja yang
perlu dilakukan optimisasi, mana yang masih lambat, dan mana yang sudah cepat.

## 2.) How does profiling help?
Dengan profiling, saya bisa lihat bahwa ada fitur yang jalannya sangat lambat sekali yaitu saat kita ingin mengakses all-students, dan dari situ
saya bisa melakukan optimisasi dan melihat sejauh apa runtime nya berkurang

## 3.) Does Intellij Profiler Actually Help Me?
Yes, seperti pada poin sebelumnya saya berhasil menemukan ada yang jalannya lambat sekali dan berhasil membuat runtime nya berkurang dari 9000ms jadi 2000ms

## 4.) Challenges?
Mungkin mencari cara dalam optimisasi nya yang sulit, untuk yang pertama dan kedua (all-student, dan all-student-names) masih lumayan mudah, namun untuk yang
highest-gpa mulai sedikit bingung gimana cara optimize nya? 

## 5.) Why Intellij Profiler
Karena dengan Intellij profiler bisa lihat detail dari fitur yang kita ingin cek, dia sudah optimal atau belum, masih bisa di optimize atau sudah cukup, kita
bisa melihat via intellij profiler

## 6.) What if Profiler isn't consistent with JMeter data?
Well, kita bisa run ulang (cara paling simple) dan selain itu kita bisa lihat juga test scenario dan conditions

## 7.) What strategies do you implement in optimizing application code after analyzing results from performance testing and profiling? How do you ensure the changes you make do not affect the application's functionality?
Well untuk saya sendiri, saya akan mencoba memahami bagaimana code ini bekerja, dia mau ngapain, cara ngelakuin nya gimana, terus dari situ kita bisa lihat dan bisa ubah
dan optimize app nya, contohnya saat saya bingung gimana mau optimize yang highest-gpa, setelah lihat, ternyata si StudentRepository extends JPARepository dan setelah
baca docs, saya bisa buat jadi lebih optimized.

## Attachments
**JMeter GUI Test Results (Pre-Optimization)**
![all-student](/docs/img/tableresults_test_plan_1.png)
*/all-student*

![all-student-name](/docs/img/tableresults_test_plan_2.png)
*/all-student-name*

![highest-gpa](/docs/img/tableresults_test_plan_3.png)
*/highest-gpa*

**JMeter CLI Test Results (Pre-Optimization)**
![all-student-name](/docs/img/cmdresults_test_plan_2.png)
*/all-student-name*

![highest-gpa](/docs/img/cmdresults_test_plan_3.png)
*/highest-gpa*

**JMeter GUI Test Results (Post-Optimization)**

![all-student](/docs/img/tableresults_post_test_plan_1.png)
*/all-student*

![all-student-name](/docs/img/tableresults_post_test_plan_2.png)
*/all-student-name*

![highest-gpa](/docs/img/tableresults_post_test_plan_3.png)
*/highest-gpa*

**JMeter CLI Test Results (Post-Optimization)**
![all-student](/docs/img/cmdresults_post_test_plan_1.png)
*/all-student*

![all-student-name](/docs/img/cmdresults_post_test_plan_2.png)
*/all-student-name*

![highest-gpa](/docs/img/cmdresults_post_test_plan_3.png)
*/highest-gpa*