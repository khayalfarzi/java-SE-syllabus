# Tapşırıq

Data transfer tapşırığı.
## Java OOP part
* OOP prinsiplərindən istifadə edərək bir insan class"ı yaradılır. Bu class daxilində OOP nin əsas 4 prinsipi də istifadə
* olunmalıdır.
* Class dəyərləri bunlardır: name,surname,age,father,mother

## Java Stream and Functional programming part
* Yuxarıda  qeyd olunan şərtlər əsasında yaradılan insan classından List formasında 15 dəyərdən ibarət bir massiv yaradılır (Collection istifadə edərək yaradılır)
*
* Java Stream funksiyalarından və funksional proqramlaşdırma dan istifadə edərək:
*
* Yaradılan List ada, soyada və yaşa (hər birini fərqli fərqli etmək lazımdır. butun filterləri eyni zamanda vermək zərurəti yoxdur)
* görə artma və azalma ardıcıllığında sortlanır.
*
* Sadəcə Stream funksiyalarından istifadə edərək bu 15 insanın orta yaş həddi tapılır. eyni zamanda yaşca ən böyuk və ən kiçik insan da tapılır

## Java File input/output stream part
* Yuxarıda qeyd edilən List formasında olan 15 insan siyahısı yaşa görə ardıcıl şəkildə duzuldukdən sonra uyğun bir fayla yazılır.
*
* Fayla yazıldıqdan sonra fayl bağlanır və bu barədə bildiriş yazısı görunur. Bundan sonra isə faylda olan məlumatlar yenidən
* console a çap olunur.
*
* Fayla yazılmış insan classının məlumatları ordan oxunduqdan sonra Yenidən insan classına çevrilir.

## Java sql part
* Yuxarıda yaradılmış insan classına uyğun sql cədvəli yaradılır.
* Bu cədvələ yuxarıda qeyd olunmuş 15 insan Listi əlavə olunur.
* Cədvələ əlavə olunmuş məlumatlar ordan oxunur.
* yaşın artma ardıcıllığı ilə sıralanmış formada cədvəldən məlumatlar oxunur.
* Cədvəlin yaşı 45 dən böyuk və 50 dən kiçik olan sətirlıri silinir.
* Yaşı 50 dən yuxarı olan insanların adları sonuna " 50"(məsələn ad : Xəyal. dəyişilmiş ad "Xəyal 50") əlavə edilir