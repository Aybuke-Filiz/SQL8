# SQL8
1.test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.
CREATE TABLE  employee(
	id SERIAL ,
	name VARCHAR(50),
	birthday DATE,
	email VARCHAR(100)
);

2.Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.

3.Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.
-UPDATE employee
SET name = 'Updated Name'
WHERE id = 5;
-UPDATE employee
SET email = 'newemail@example.com'
WHERE name = 'Fleurette Balmforth';
-UPDATE employee
SET name = 'Updated Jane'
WHERE birthday = '2024-08-08';
-UPDATE employee
SET birthday = '1980-01-01'
WHERE email = 'jbrandenberg1d@barnesandnoble.com';
-UPDATE employee
SET name = 'Updated Name 2', email = 'updatedemail2@example.com'
WHERE id = 2;

4.Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.
-DELETE FROM employee
WHERE id = 3;
-DELETE FROM employee
WHERE name = 'Dalli Simison';
-DELETE FROM employee
WHERE birthday = '2025-01-02';
-DELETE FROM employee
WHERE email = 'mkingcoteb@intel.com';
-DELETE FROM employee
WHERE id = 4 AND email = 'fbalmforth3@163.com';
