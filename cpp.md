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
Linia 1: #include <iostream> to nagłówek biblioteki, który pozwala nam korzystać z obiektów wejścia i wyjścia, takich jak cout (używany w linii 5). Pliki nagłówkowe dodają funkcjonalności do programów w C++.

Linia 2: using namespace std oznacza, że możemy używać nazw obiektów i zmiennych z biblioteki standardowej bez konieczności poprzedzania ich prefiksem std::.

Nie martw się, jeśli nie rozumiesz jeszcze, jak działa #include <iostream> i using namespace std. Po prostu traktuj to jako coś, co (prawie) zawsze pojawia się w twoim programie.

Linia 3: Pusta linia. C++ ignoruje białe znaki, ale używamy ich, aby kod był bardziej czytelny.

Linia 4: Kolejną rzeczą, która zawsze pojawia się w programie C++, jest int main(). Jest to funkcja. Każdy kod wewnątrz jej nawiasów klamrowych {} zostanie wykonany.

Linia 5: cout (wymawiane "see-out") to obiekt używany razem z operatorem wstawiania (<<) do wyjścia/drukowania tekstu. W naszym przykładzie wypisze "Hello World!".

Uwaga: Każde polecenie w C++ kończy się średnikiem ;.
### _[Powrót do strony głównej](./index.html)_