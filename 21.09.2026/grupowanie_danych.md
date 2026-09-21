SELECT MIN(placa_pod), MAX(placa_pod),MAX(placa_pod) - MIN(placa_pod) FROM pracownicy
SELECT etat, AVG(placa_pod) FROM pracownicy GROUP BY etat ORDER BY AVG(placa_pod) DESC;
SELECT COUNT(etat) FROM pracownicy WHERE etat = "PROFESOR"
