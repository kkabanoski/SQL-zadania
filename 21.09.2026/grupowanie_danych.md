SELECT MIN(placa_pod), MAX(placa_pod),MAX(placa_pod) - MIN(placa_pod) FROM pracownicy
SELECT etat, AVG(placa_pod) FROM pracownicy GROUP BY etat ORDER BY AVG(placa_pod) DESC;
SELECT COUNT(etat) FROM pracownicy WHERE etat = "PROFESOR"
SELECT id_zesp,SUM(placa_pod + placa_dod) FROM pracownicy GROUP BY id_zesp
SELECT id_zesp, COUNT(id_zesp) FROM pracownicy GROUP BY id_zesp HAVING COUNT(id_zesp) > 2 ORDER BY COUNT(id_zesp) DESC
SELECT zatrudniony,count(etat), etat, SUM(placa_pod + placa_dod) / 2 FROM pracownicy WHERE zatrudniony < "1990-01-01" GROUP by etat  
SELECT id_prac, COUNT(id_prac) FROM pracownicy GROUP BY id_prac HAVING COUNT(id_prac) > 1;
SELECT nazwa,SUM(placa_od + placa_do) / 2 FROM etaty GROUP by nazwa
SELECT etat,SUM(placa_pod + placa_dod) FROM pracownicy GROUP BY etat ORDER BY etat DESC
SELECT etat,COUNT(etat) FROM pracownicy GROUP BY etat 
SELECT etat,placa_pod + placa_dod FROM pracownicy WHERE placa_pod +placa_dod > 1400 GROUP BY etat 
SELECT etat, COUNT(etat) FROM pracownicy GROUP BY etat HAVING COUNT(etat) > 3
SELECT id_zesp, placa_pod+placa_dod / 2 FROM pracownicy GROUP BY id_zesp
SELECT etat, MAX(placa_pod+placa_dod) FROM pracownicy GROUP BY etat
SELECT zatrudniony,COUNT(id_prac) FROM pracownicy GROUP by year(zatrudniony) 
SELECT id_prac,imie,nazwisko,MIN(placa_pod + placa_dod) FROM pracownicy GROUP by placa_pod + placa_dod
SELECT id_prac, imie, nazwisko FROM pracownicy WHERE nazwisko LIKE "K%" 
SELECT id_prac, nazwisko, imie, placa_pod + placa_dod FROM pracownicy WHERE placa_pod + placa_dod > 3000
SELECT id_prac, nazwisko, imie, year(zatrudniony) FROM pracownicy WHERE year(zatrudniony) > 2022
SELECT id_prac, nazwisko, imie FROM pracownicy WHERE nazwisko LIKE "%a%"
SELECT id_prac, nazwisko, imie FROM pracownicy WHERE nazwisko LIKE "K%" AND nazwisko LIKE "%i"
SELECT id_zesp, COUNT(id_zesp) FROM pracownicy GROUP BY id_zesp HAVING COUNT(id_zesp) > 3;
