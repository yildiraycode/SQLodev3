# SQLodev3
## sql sorguları patika odev 1 ##
**Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.**<br/>
1.country tablosunda bulunan country sütunundaki ülke isimlerinden 'A' karakteri ile başlayıp 'a' karakteri ile sonlananları sıralayınız.<br/><br/>
SELECT * FROM country<br/>
WHERE country LIKE 'A%a';<br/><br/><br/>
2.country tablosunda bulunan country sütunundaki ülke isimlerinden en az 6 karakterden oluşan ve sonu 'n' karakteri ile sonlananları sıralayınız.<br/><br/>
SELECT country<br/>
FROM country<br/>
WHERE LENGTH(country) >= 6 AND country LIKE '%n';<br/><br/><br/>
3.film tablosunda bulunan title sütunundaki film isimlerinden en az 4 adet büyük ya da küçük harf farketmesizin 'T' karakteri içeren film isimlerini sıralayınız.<br/><br/>
SELECT title<br/>
FROM film<br/>
WHERE title ILIKE '%T%T%T%T%';<br/><br/><br/>
4.film tablosunda bulunan tüm sütunlardaki verilerden title 'C' karakteri ile başlayan ve uzunluğu (length) 90 dan büyük olan ve rental_rate 2.99 olan verileri sıralayınız.<br/>
SELECT *<br/>
FROM film<br/>
WHERE length>90 and title LIKE 'C%' and rental_rate=2.99; <br/><br/><br/>
