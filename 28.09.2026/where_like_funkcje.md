SELECT nazwa_produktu, cena_sprzedazy from produkty WHERE cena_sprzedazy > 5000 
SELECT nazwa_produktu, min_stan_magazynowy FROM produkty WHERE min_stan_magazynowy >= 10
SELECT nazwa_produktu FROM produkty WHERE nazwa_produktu LIKE "%Samsung%"
SELECT imie,nazwisko,email FROM klienci WHERE email LIKE "%gmail.com"
SELECT nazwa_produktu,cena_sprzedazy ,opis FROM produkty WHERE nazwa_produktu like "%PRO%"
SELECT nazwa_produktu, cena_sprzedazy FROM produkty WHERE cena_sprzedazy BETWEEN 1000 and 3000
SELECT nazwa_produktu, waga ,jednostka_miary FROM produkty WHERE waga BETWEEN 0.1 AND 1
SELECT nazwa_produktu, id_producenta FROM produkty WHERE id_producenta = 1 OR 2 OR 11
SELECT imie,nazwisko,stanowisko from pracownicy where stanowisko = "Magazynier" OR "Kierownik magazynu" OR "Sprzedawca"
SELECT nazwa_produktu, cena_sprzedazy, dostepny FROM produkty WHERE dostepny = 1 and cena_sprzedazy < 2000
