---
layout: default
---

# Programowanie w C++
Nauczysz się tutaj kodowania w C++, podstawowej składni oraz wielu innych elementów kodu 
## Podstawowa składnia języka C++

```cpp
#include <iostream>
using namespace std;

int main() {
  cout << "Witaj świecie!";
  return 0;
}
```
**Linia 1:** _#include <iostream.>_ to nagłówek biblioteki, który pozwala nam korzystać z obiektów wejścia i wyjścia, takich jak _cout_ . Pliki nagłówkowe dodają funkcjonalności do programów w C++.

**Linia 2:** _using namespace std_ oznacza, że możemy używać nazw obiektów i zmiennych z biblioteki standardowej bez konieczności poprzedzania ich prefiksem _std::_.

**Linia 3:** Pusta linia. C++ ignoruje białe znaki, ale używamy ich, aby kod był bardziej czytelny.

**Linia 4:** Kolejną rzeczą, która zawsze pojawia się w programie C++, jest _int main()_. Jest to funkcja. Każdy kod wewnątrz jej nawiasów klamrowych {} zostanie wykonany.

**Linia 5:** _cout_ to obiekt używany razem z operatorem wstawiania (<<) do wyjścia/drukowania tekstu. W naszym przykładzie wypisze "Witaj świecie!".

**Uwaga:** Każde polecenie w C++ kończy się średnikiem ;.

**Linia 6:** _return 0_ kończy funkcję _main_.

**Linia 7:** Nie zapomnij dodać zamykającego nawiasu klamrowego }, aby faktycznie zakończyć funkcję _main_.

#### Dodatkowe uwagi
- **Komentarze:** Warto dodać komentarze do kodu, aby inni programiści (lub Ty sam w przyszłości) mogli łatwiej zrozumieć, co dany fragment kodu robi. Komentarze w C++ zaczynają się od // dla komentarzy jednoliniowych i /* ... */ dla komentarzy wieloliniowych.

- **Konwencje nazewnictwa:** Używanie przejrzystych i opisowych nazw zmiennych, funkcji i klas sprawia, że kod jest łatwiejszy do zrozumienia i utrzymania.

## Zmienne w C++
Zmienne to kontenery do przechowywania wartości danych. W C++ istnieją różne typy zmiennych, które są definiowane za pomocą różnych słów kluczowych. Oto niektóre z nich:
1. **int** - przechowuje liczby całkowite (bez miejsc dziesiętnych), takie jak 123 lub -123
2. **double** - przechowuje liczby zmiennoprzecinkowe (z miejscami dziesiętnymi), takie jak 19.99 lub -19.99
3. **char** - przechowuje pojedyncze znaki, takie jak 'a' lub 'B'. Wartości typu char są otoczone pojedynczymi cudzysłowami
4. **string** - przechowuje tekst, taki jak "Hello World". Wartości typu string są otoczone podwójnymi cudzysłowami
5. **bool** - przechowuje wartości mające dwa stany: true (prawda) lub false (fałsz)

#### Przykład zastosowania zmiennych

```cpp
#include <iostream>
#include <string> // Potrzebne do użycia typu string

using namespace std;

int main() {
    int liczbaCalkowita = 123; // Zmienna typu int
    double liczbaZmiennoprzecinkowa = 19.99; // Zmienna typu double
    char pojedynczyZnak = 'A'; // Zmienna typu char
    string tekst = "Witaj świecie"; // Zmienna typu string
    bool prawdaCzyFalsz = true; // Zmienna typu bool

    // Wyświetlanie wartości zmiennych
    cout << "Liczba całkowita: " << liczbaCalkowita << endl;
    cout << "Liczba zmiennoprzecinkowa: " << liczbaZmiennoprzecinkowa << endl;
    cout << "Pojedynczy znak: " << pojedynczyZnak << endl;
    cout << "Tekst: " << tekst << endl;
    cout << "Prawda czy fałsz: " << prawdaCzyFalsz << endl;

    return 0;
}
```
## Operatory Arytmetyczne w C++
Operatory arytmetyczne są używane do wykonywania podstawowych operacji matematycznych. Oto lista operatorów arytmetycznych dostępnych w C++ wraz z ich opisem i przykładami:

| Operator | Nazwa         | Opis                              | Przykład    |
|----------|---------------|-----------------------------------|-------------|
| +        | Dodawanie     | Dodaje dwie wartości              | x + y       |
| -        | Odejmowanie   | Odejmuje jedną wartość od drugiej | x - y       |
| *        | Mnożenie      | Mnoży dwie wartości               | x * y       |
| /        | Dzielenie     | Dzieli jedną wartość przez drugą  | x / y       |
| %        | Modulo        | Zwraca resztę z dzielenia         | x % y       |
| ++       | Inkrementacja | Zwieksza wartość zmiennej o 1     | ++x lub x++ |
| --       | Dekrementacja | Zmniejsza wartość zmiennej o 1    | --x lub x-- |

## Operatory Przypisania w C++
Operatory przypisania są używane do przypisywania wartości zmiennym. Poniżej znajduje się lista operatorów przypisania dostępnych w C++ wraz z ich opisem i przykładami:


| Operator | Przykład  | 	To samo co |
|---------|-----------|-------------|
| =	      | x = 5	    | x = 5       |
| +=	     | x += 3	   | x = x + 3   |
| -=	     | x -= 3	   | x = x - 3   |
| *=	     | x *= 3	   | x = x * 3   |
| /=	     | x /= 3	   | x = x / 3   |
| %=	     | x %= 3	   | x = x % 3   |
| &=	     | x &= 3	   | x = x & 3   |
| ^=	     | x ^= 3	   | x = x ^ 3   |
| **>>**=     | 	x >>= 3  | 	x = x >> 3 |
| <<=     | 	x <<= 3	 | x = x << 3  |

## Operatory Porównania
Operatory porównania są używane do porównywania dwóch wartości (lub zmiennych). Jest to ważne w programowaniu, ponieważ pozwala nam znajdować odpowiedzi i podejmować decyzje.

Wartość zwracana przez operator porównania to albo 1, albo 0, co oznacza odpowiednio true (prawda) lub false (fałsz). Te wartości są znane jako wartości logiczne (Boolean).

Operatory porównania są używane do porównywania dwóch wartości (lub zmiennych). Jest to ważne w programowaniu, ponieważ pozwala nam znajdować odpowiedzi i podejmować decyzje.

| Operator | 	Nazwa	             | Przykład |
|----------|---------------------|----------|
| ==       | 	Równe	             | x == y   |
| !=	      | Różne	              | x != y   |
| **>**	       | Większe niż	        | x > y    |
| <	       | Mniejsze niż	       | x < y    |
| **>**=	      | Większe lub równe	  | x >= y   |
| <=	      | Mniejsze lub równe	 | x <= y   |


### _[Powrót do strony głównej](./index.html)_