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
**Linia 1:** _#include <iostream>_ to nagłówek biblioteki, który pozwala nam korzystać z obiektów wejścia i wyjścia, takich jak _cout_. Pliki nagłówkowe dodają funkcjonalności do programów w C++.

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


### _[Powrót do strony głównej](./index.html)_