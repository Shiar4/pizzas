# Pizzas

## Praca na zajęciach z debugowania (moduł Narzędzia programisty)

Znajdź i popraw błędy w programie przy użyciu debuggera gdb/lldb. Po poprawkach wszystkie testy powinny przechodzić.

* +10 XP za poprawienie błędów w programie

## Praca na zajęciach z testowania (moduł Testowanie)

### Część 1

* Napisz własne klasy PizzaDummy i PizzaStub. Porównaj je z implementacjami w pliku test/mocks/PizzaMock.hpp
* Popraw interfejs Pizza, aby nie posiadał on swojego konstruktora. Napisz odpowiednie konstruktory w klasach dziedziczących (jeśli są potrzebne). Popraw też atrapy testowe.

### Część 2

* Popraw klasę PizzaMock, aby była napisana z użyciem nowszej wersji GMocka.
* Usuń zależność od czasu w testach za pomocą dummy lub stuba.

## Praca domowa

1. (10 XP) Napisz klasę TimeMock, którą zastąpisz dummy/stuba napisanego podczas zajęć. Używaj go poprzez StrictMock. Dodaj właściwe `EXPECT_CALL` w kodzie testów.
2. (15 XP) Dopisz nowy przypadek testowy, w którym powielasz działanie funkcji main.cpp, ale zamawiasz 3 pizze: `StubPizza` oraz 2 różne `MockPizza` (różne nazwy, ceny i czas pieczenia; jedna jako StrictMock, druga jako NiceMock). Ustaw właściwe `EXPECT_CALL`.
3. (5 XP) Utwórz własny plik .github/workflows/module3.yml, który spowoduje, że GitHub automatycznie uruchomi testy. Zobacz, jak to jest zrealizowane w innych repozytoriach [Coders School na GH](https://github.com/coders-school)

Możecie pracować w parach 🙂
