# Small Registration App

## Technical Recruitment

### Person :

* id            (Integer, not null, Unique, AutoIncrease)
* name          (String or text (varchar))
* surname       (String or text (varchar))
* father name   (String or text (varchar))
* age           (Byte or number type in db)
* gender        (Enum in java)

### User :

* person id (Reference Person class or table)
* username  (String or varchar , Unique)
* password  (String or varchar)

## Explanation

Yuxarıda qeyd edilən 2, Person və User adlı Java class"larımız və SQL cədvəllərimiz mövcuddur.

* Sizdən Tələb olunan tapşırıq aşağıdakı kimidir:
    * Bir java proqramı hazırlanır, hansı ki əmrlər komandalar şəklində verilir. Məsələn: proqram işə duşdukdən sonra
      sizdən bir komanda daxil etməyinizi gözləyir.
    * Komandalar aşağıdakılardır:
        * sp (Save Person). Bu komanda vasitəsilə istifadəçi Person bölməsində olan məlumatları ardıcıl olaraq doldurur
          və enter duyməsini basır. Bu zaman istifadəçinin daxil etdiyi məlumatlar bazada uyğun cədvələ əlavə olunur.
        * ru (Register User) User hissəsində verilən məlumatlar doldurulur yəni, Person id, username və parol.
          Doldurulduqdan sonra uyğun cədvələ əlavə edilir. Bu zaman bazada daxil edilən username olub olmadığı
          yoxlanılır. Əgər varsa istifadəçiyə məlumat verilir və username dəyişdirilməsi tələb olunur.
        * shp (Show People) Bu komanda vasitəsilə bazada olan Person cədvəlinin butun məlumatları list şəklində
          göstərilir.
        * exit - Bu komanda verildiyi zaman proqram söndurulur.

* Proqramın məqsədi Java class"larından və SQL cədvəllərindən istifadə edərək JDBC əlaqələrini yaratmaq və duzgun şəkildə
  sorğuları yazmaqdır. Bu tapşırığı etdiyiniz zaman OOP prinsiplərindən, Collectionlardan , Exceptions və Exception
  handling bölməsindən, SQL dən , JDBC dən və digər keçdiyimiz mövzulardan düzgun şəkildə istifadə etməyiniz tələb olunur.