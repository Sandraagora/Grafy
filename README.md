# Grafy

Ustalenie Najkrótszego Algorytmu:


Algorytm Dijstry:

•	Algorytm Dijkstry służy do wyznaczania najmniejszej odległości od ustalonego wierzchołka  do wszystkich pozostałych w skierowanym grafie, w odróżnieniu jednak od Algorytmu Forda-Bellmana, graf wejściowy nie może zawierać krawędzi o ujemnych wagach.
•	Działanie Algorytm Dijkstry znajduje w grafie wszystkie najkrótsze ścieżki pomiędzy wybranym wierzchołkiem a wszystkimi pozostałymi, przy okazji wyliczając również koszt przejścia każdej z tych ścieżek. Algorytm Dijkstry jest przykładem algorytmu zachłannego.
•	Z algorytmu Dijkstry można skorzystać przy obliczaniu najkrótszej drogi do danej miejscowości. Wystarczy przyjąć, że każdy z punktów skrzyżowań dróg to jeden z wierzchołków grafu, a odległości między punktami to wagi krawędzi.

Algorytm Bellmana-Forda:

•	Algorytm Bellmana-Forda rozwiązuje problem najkrótszej ścieżki, tj. pozwala znaleźć ścieżkę o najmniejszej wadze pomiędzy dwoma wierzchołkami w grafie ważonym. W odróżnieniu od algorytmu Dijkstry, poprawność algorytmu Bellmana-Forda nie opiera się na założeniu, że wagi w grafie są nieujemne (nie może jednak występować cykl o łącznej ujemnej wadze osiągalny ze źródła). Za tę ogólność płaci się jednak wyższą złożonością czasową.



Opis:
•	Dla każdego wierzchołka przypisywane są dwie wartości: koszt dojścia  oraz poprzednik. Początkowo każdy wierzchołek ma koszt dojścia nieskończony, a poprzednik jest nieznany. Wyjątkiem jest wierzchołek początkowy dla którego koszt dojścia wynosi 0.
•	Dalszy etap polega na utworzeniu kolejki wszystkich wierzchołków. Nastpnie dopóki kolejka nie jest pusta należy usunąć wierzchołek o najmniejszym kluczu dystansie i zbadać dla niego wszystkie połączone wierzchołki. Jeśli połączenie z wybranego wierzchołka do sąsiada ma łącznie mniejszą wartość niż docelowy wierzchołek to należy zaktualizować koszt dojścia oraz sąsiada.
