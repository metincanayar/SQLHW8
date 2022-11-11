# SQLHW8

#### 1- test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.
```SQL
CREATE TABLE employee(
	employee_id SERIAL PRIMARY KEY,
	name VARCHAR(50) NOT NULL,
	birthday DATE,
	email VARCHAR(100)
);
```


#### 2- Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.

```SQL
insert into employee (name, birthday, email) values ('Cecelia', '1956-01-16', 'cpiddington0@google.fr');
insert into employee (name, birthday, email) values ('Claudina', '1957-02-27', 'cmatuszyk1@telegraph.co.uk');
insert into employee (name, birthday, email) values ('Pauletta', '1970-12-23', 'pcatlette2@gizmodo.com');
insert into employee (name, birthday, email) values ('Crissy', '1981-07-02', 'cwicher3@cbslocal.com');
insert into employee (name, birthday, email) values ('Boniface', '1962-05-23', 'ballaway4@cmu.edu');
insert into employee (name, birthday, email) values ('Roosevelt', '1973-01-16', 'rblenkiron5@admin.ch');
insert into employee (name, birthday, email) values ('Lisabeth', '1960-09-03', 'lfolca6@hp.com');
insert into employee (name, birthday, email) values ('Alexina', '1960-11-16', 'adack7@phpbb.com');
insert into employee (name, birthday, email) values ('Phillida', '1993-12-26', 'pmusso8@abc.net.au');
insert into employee (name, birthday, email) values ('Layne', '1974-04-29', 'lvine9@webeden.co.uk');
insert into employee (name, birthday, email) values ('Cal', '1956-03-06', 'ccornillia@state.gov');
insert into employee (name, birthday, email) values ('Sianna', '1969-03-19', 'sbrotherhedb@weibo.com');
insert into employee (name, birthday, email) values ('Jay', null, null);
insert into employee (name, birthday, email) values ('Franciskus', '1958-03-08', 'fknathd@nps.gov');
insert into employee (name, birthday, email) values ('Barbabas', '1982-07-13', 'bdyersone@wufoo.com');
insert into employee (name, birthday, email) values ('Milly', '1987-08-25', 'mhambribef@mozilla.org');
insert into employee (name, birthday, email) values ('Lind', '1991-12-02', 'lnewittg@unc.edu');
insert into employee (name, birthday, email) values ('Issiah', '1995-01-07', 'ijoseh@reverbnation.com');
insert into employee (name, birthday, email) values ('Alberto', '1993-08-09', 'aantonioi@delicious.com');
insert into employee (name, birthday, email) values ('Benedikt', '1962-11-19', 'brawlinsonj@princeton.edu');
insert into employee (name, birthday, email) values ('Jens', '1983-01-21', 'jbeaumentk@elegantthemes.com');
insert into employee (name, birthday, email) values ('Tabina', '1977-07-17', 'tfairl@wiley.com');
insert into employee (name, birthday, email) values ('Alida', '1991-07-01', 'agiorgiettom@oakley.com');
insert into employee (name, birthday, email) values ('Hartwell', '1993-09-23', 'hhobbenn@slideshare.net');
insert into employee (name, birthday, email) values ('Allen', '1976-04-22', 'amonksfieldo@ovh.net');
insert into employee (name, birthday, email) values ('Creigh', '1976-05-28', 'cduckfieldp@dailymotion.com');
insert into employee (name, birthday, email) values ('Gideon', '1969-01-15', 'gmaddyq@163.com');
insert into employee (name, birthday, email) values ('Jakie', '1970-01-20', 'jremmerr@shinystat.com');
insert into employee (name, birthday, email) values ('Eunice', '1992-05-21', 'eswyers@arizona.edu');
insert into employee (name, birthday, email) values ('Josh', '1962-09-04', 'jleest@sakura.ne.jp');
insert into employee (name, birthday, email) values ('Paige', '1974-06-26', 'psilcoxu@patch.com');
insert into employee (name, birthday, email) values ('Issy', '1983-08-31', 'ijagielskiv@merriam-webster.com');
insert into employee (name, birthday, email) values ('Waylen', '1952-02-14', 'wtrusew@simplemachines.org');
insert into employee (name, birthday, email) values ('Jory', null, null);
insert into employee (name, birthday, email) values ('Joannes', '1979-01-09', 'jpowtery@nsw.gov.au');
insert into employee (name, birthday, email) values ('Allyce', '1990-02-12', 'aknevitz@altervista.org');
insert into employee (name, birthday, email) values ('Horton', '1990-11-02', 'hoaten10@facebook.com');
insert into employee (name, birthday, email) values ('Delila', '1961-11-21', 'dclewarth11@devhub.com');
insert into employee (name, birthday, email) values ('Bobine', '1995-08-30', 'bvonderempten12@europa.eu');
insert into employee (name, birthday, email) values ('Theodoric', '1966-01-24', 'tgammel13@newsvine.com');
insert into employee (name, birthday, email) values ('Rhys', '1977-03-31', 'rromney14@1und1.de');
insert into employee (name, birthday, email) values ('Boyce', '1989-03-13', 'bvater15@slate.com');
insert into employee (name, birthday, email) values ('Lorette', '1984-05-23', 'lcoxon16@vimeo.com');
insert into employee (name, birthday, email) values ('Bonny', '1960-07-27', 'bbasire17@feedburner.com');
insert into employee (name, birthday, email) values ('Hersh', '1980-02-03', 'hstafford18@sciencedirect.com');
insert into employee (name, birthday, email) values ('Ashlie', '1952-03-30', 'agoldhawk19@yellowpages.com');
insert into employee (name, birthday, email) values ('Chris', '1981-02-22', 'ccampaigne1a@google.co.uk');
insert into employee (name, birthday, email) values ('Bary', '1955-12-23', 'bcaplan1b@china.com.cn');
insert into employee (name, birthday, email) values ('Mandy', '1969-08-21', 'mknutton1c@springer.com');
insert into employee (name, birthday, email) values ('Ezri', '1958-06-04', 'etrue1d@sakura.ne.jp');
```
#### 3- Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.

```SQL
UPDATE employee
SET name = 'M___'
WHERE name LIKE 'M%'
RETURNING *;

UPDATE employee
SET email = null
WHERE name = 'M___'
RETURNING *;

UPDATE employee
SET birthday = '1983-01-21'
WHERE name = 'M___'
RETURNING *;

UPDATE employee
SET name = 'Metin'
WHERE name = 'M___'
RETURNING *;

UPDATE employee
SET birthday = '1960-07-27'
WHERE name = 'Bary'
RETURNING *;
```
#### 4- Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.

```SQL
DELETE FROM employee
WHERE email LIKE 'm%'
RETURNING *;

DELETE FROM employee
WHERE employee_id >39
RETURNING *;

DELETE FROM employee
WHERE name = 'Metin';

DELETE FROM employee
WHERE name LIKE '%D'
RETURNING *;

DELETE FROM employee
WHERE email ILIKE '%a%a'
RETURNING *;

```
