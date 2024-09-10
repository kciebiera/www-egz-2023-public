Informacje ogólne
======

Jest jedno zadanie programistyczne składające się z kilku punktów. Egzamin trwa od 14:10 do 17:00.

Cel zadania:
=====

Stworzenie serwisu umożliwiającego zapisywanie i odczytywanie wartości kursów akcji. 
Kurs to wartość przypisana do konkretnej etykiety. Etykiety i nazwy firm są znane i ustalone:

| Nazwa firmy |	Etykieta akcji| 
| - | - |
| Stellar Dynamics | STDY |
| Indigo Innovations | INDI |
| Zenith Horizons	| ZNHR |
| Crimson Technologies | CRMT |
| Azure Aeronautics	| AZAE |
| Emerald Enterprises	| EMEN |
| Obsidian Solutions | OBSO |
| Veridian Ventures | VRVN |
| Sapphire Systems | SAPH |
| Garnet Global	| GARG|

Serwer FastAPI
=====

Zaimplementuj serwer FastAPI, który udostępnia następujące metody (każda z nich powinna posiadać dokumentację):

1. Odczyt listy wszystkich nazw firm i odpowiadających im etykiet.
2. Odczyt najnowszej wartości kursu akcji dla podanej etykiety.
3. Odczyt n najnowszych wartości kursu wraz z czasami zmian dla podanej etykiety.
4. Odczyt najnowszych kursów wszystkich akcji (zwraca tylko etykietę i wartość, bez nazwy firmy).
5. Zapis aktualnej wartości kursu akcji dla autoryzowanego użytkownika (proponowana metoda autoryzacji: API KEY).

Możesz przechowywać dane w pamięci, pliku, bazie danych albo innym dogodnym dla siebie formacie.

Przechowywanie danych
====

Możesz wybrać dowolną metodę przechowywania danych: w pamięci, w pliku, w bazie danych lub inną, która Ci odpowiada.

Uwagi
====

1. **Modele Pydantic:** Dla metod 2-3 przygotuj modele Pydantic do walidacji danych wejściowych i wyjściowych.
2. **Dokumentacja:** Każdy endpoint powinien posiadać krótką dokumentację (1-2 zdania), dostępną w automatycznie generowanej dokumentacji FastAPI (pod adresem /docs).
3. **Przykładowe testy:** Zaimplementuj przykładowe testy.


Klient w TypeScript
======

Stwórz klienta w TypeScript, który umożliwia korzystanie z wszystkich metod serwera FastAPI.

- Dla metody 3 (n najnowszych wartości) klient powinien wyświetlić dane w tabeli z kolumnami: data zmiany i wartość.
- Dla metody 4 (wartości kursów) klient powinien wyświetlić dane w tabeli z kolumnami: nazwa firmy, etykieta, wartość. W tym przypadku konieczne będą dwa wywołania do FastAPI.

Uwagi ogólne
======

1. Zarówno klient, jak i serwer będą oceniane maksymalnie na 10 punktów.
2. Możesz oddać tylko klienta (za mniejszą liczbę punktów), implementując makiety (mockupy) serwera.
