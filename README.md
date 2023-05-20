# SQL_ODV3
# SQL Ödev 3 | LIKE ve ILIKE

Merhabalar,

Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.

1-) country tablosunda bulunan country sütunundaki ülke isimlerinden 'A' karakteri ile başlayıp 'a' karakteri ile sonlananları sıralayınız.
SELECT country FROM country
WHERE country LIKE 'A%a';

![image](https://github.com/CYazar12/SQL_ODV3/assets/109551508/9377c0e1-f7fd-4a27-a924-41e5d31624e4)


2-) country tablosunda bulunan country sütunundaki ülke isimlerinden en az 6 karakterden oluşan ve sonu 'n' karakteri ile sonlananları sıralayınız.
SELECT country FROM country
WHERE country LIKE '_____%n';

![image](https://github.com/CYazar12/SQL_ODV3/assets/109551508/210ff6eb-7a33-46d7-8288-daf1fa0ddf0a)


3- ) film tablosunda bulunan title sütunundaki film isimlerinden en az 4 adet büyük ya da küçük harf farketmesizin 'T' karakteri içeren film isimlerini sıralayınız.
SELECT title FROM film
WHERE title ILIKE '%T%T%T%T%';

![image](https://github.com/CYazar12/SQL_ODV3/assets/109551508/84043be1-8861-47de-803e-0882e2ba2ee0)


4- ) film tablosunda bulunan tüm sütunlardaki verilerden title 'C' karakteri ile başlayan ve uzunluğu (length) 90 dan büyük olan ve rental_rate 2.99 olan verileri sıralayınız.

SELECT * FROM film
WHERE title LIKE 'C%'
AND length >90 
AND rental_rate = 2.99;

![image](https://github.com/CYazar12/SQL_ODV3/assets/109551508/5296a039-b52f-4b17-8ed7-d75b78794403)

