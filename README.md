# SQL-zadania
CREATE DATABASE pracownicy.sql
SELECT * FROM `pracownicy`
SELECT imie,nazwisko,stanowisko FROM `pracownicy`
SELECT * FROM `pracownicy` WHERE nazwisko = "Kowalski"
SELECT * FROM `pracownicy` WHERE placa < 1600
SELECT * FROM `pracownicy` WHERE placa BETWEEN 1400 and 1600
SELECT * FROM `pracownicy` WHERE id = 3 OR id = 5 OR id = 7
SELECT * FROM `pracownicy` WHERE imie LIKE 'Ka%'
SELECT id,imie,nazwisko FROM `pracownicy` WHERE PESEL is NULL
SELECT nazwisko FROM `pracownicy` 
SELECT * FROM pracownicy WHERE placa > 1400 AND stanowisko !="kierownik" AND pesel is not null

CREATE DATABASE zapytania_filmoteka
SELECT tytul from `film` WHERE dlugosc > 115
SELECT tytul FROM `film` WHERE rok < 2000
SELECT tytul from `film` WHERE tytul LIKE 'G%'

SELECT * FROM `film` ORDER BY tytul ASC
SELECT * FROM `film` ORDER BY LENGTH(tytul) ASC
SELECT imie,nazwisko FROM `rezyser` WHERE miejsce_urodzenia = 'Polska' OR miejsce_urodzenia = 'USA'
select id from ranking WHERE oscar > 0
