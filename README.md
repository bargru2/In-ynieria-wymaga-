# Opracowanie specyfikacji wymagań wybranego systemu 

---

# 1. Charakterystyka oprogramowania
# a. Nazwa skrócona
EasySales Mobile

#  b. Nazwa pełna
 System mobilnej sprzedaży przedstawiciela handlowego 

# c. Krótki opis ze wskazaniem celów <img height=20 src="documentation/media/windows_logo.png"/>
EasySales Mobile to nowoczesna aplikacja zaprojektowana dla firm dążących do usprawnienia i zautomatyzowania procesów sprzedaży, logistyki oraz obsługi klienta. Dedykowany jest dla przedstawicieli handlowych, pracowników terenowych, którzy większość czasu pracują poza biurem. Za pomocą zaawansowanych funkcji, integracji z systemem ERP oraz przyjaznemu interfejsowi jakość obsługi klienta znacząco się poprawia. Efektywnie wpływa na realizacje zamierzonych celów sprzedażowych poprzez korzystanie z systemu w dowolnym miejscu i czasie, koncentrując się na najszybszym dotarciu do klienta.  Dzięki temu EasySales Mobile skraca czas realizacji wykonywanych czynności.

# 2. Prawa autorskie.

# a. Autor
Bartosz Grudzień
---
Jakub Kreft
---
Stanisław Prystupa
---

# b. Warunki licencyjne do oprogramowania wytworzonego przez grupę

MIT License

Copyright (c) [2024] [BJS]

Niniejszym udziela się bezpłatnego pozwolenia każdej osobie uzyskującej kopię tego oprogramowania i powiązanej dokumentacji (dalej "Oprogramowanie"), do bezpłatnego użytkowania Oprogramowania bez ograniczeń, w tym bez ograniczeń do prawa do użytkowania, kopiowania, modyfikowania, łączenia, publikowania, dystrybucji, sublicencjonowania i/lub sprzedaży kopii Oprogramowania, oraz do zezwalania osobom, którym Oprogramowanie jest dostarczane, na takie same działania, z zastrzeżeniem następujących warunków:

Powyższa informacja o prawach autorskich oraz niniejsza informacja o pozwoleniu musi być zawarta we wszystkich kopiach lub istotnych częściach Oprogramowania.

OPROGRAMOWANIE JEST DOSTARCZANE "TAK JAK JEST", BEZ JAKIEJKOLWIEK GWARANCJI, WYRAŹNEJ LUB DOMNIEMANEJ, W TYM BEZ GWARANCJI PRZYDATNOŚCI HANDLOWEJ, PRZYDATNOŚCI DO OKREŚLONEGO CELU I NIENARUSZALNOŚCI PRAW. W ŻADNYM WYPADKU AUTORZY LUB POSIADACZE PRAW AUTORSKICH NIE BĘDĄ PONOSIĆ ODPOWIEDZIALNOŚCI ZA JAKIEKOLWIEK ROSZCZENIA, SZKODY LUB INNE ZOBOWIĄZANIA, CZY TO W WYNIKU DZIAŁANIA UMOWY, DELIKTU LUB INNEJ SYTUACJI POWSTAŁEJ W ZWIĄZKU Z OPROGRAMOWANIEM LUB KORZYSTANIEM Z NIEGO LUB INNYMI DZIAŁANIAMI W OPROGRAMOWANIU.

# 3. Specyfikacja wymagań
# a. Wymagania systemu EasySales Mobile

| Identyfikator | Nazwa                        | Opis                                                                                                  | Priorytet | Kategoria         |
|---------------|------------------------------|-------------------------------------------------------------------------------------------------------|-----------|-------------------|
| REQ-001       | Logowanie                    | System powinien umożliwiać użytkownikom logowanie przy użyciu unikalnego identyfikatora i hasła.      | 1         | Funkcjonalne      |
| REQ-002       | Przeglądanie produktów       | System powinien pozwalać użytkownikom na przeglądanie dostępnych produktów z ich opisami i cenami.     | 1         | Funkcjonalne      |
| REQ-003       | Dodawanie produktów do koszyka| System powinien umożliwiać dodawanie wybranych produktów do koszyka zakupowego.                       | 1         | Funkcjonalne      |
| REQ-004       | Składanie zamówienia         | System powinien umożliwiać składanie zamówienia i wybór metody płatności oraz dostawy.                | 1         | Funkcjonalne      |
| REQ-005       | Historia zamówień            | System powinien przechowywać historię zamówień użytkownika i umożliwiać ich przeglądanie.             | 2         | Funkcjonalne      |
| REQ-006       | Powiadomienia push           | System powinien wysyłać powiadomienia push o nowych ofertach i statusie zamówień.                     | 3         | Funkcjonalne      |
| REQ-007       | Wyszukiwanie produktów       | System powinien umożliwiać wyszukiwanie produktów po nazwie, kategorii lub innych parametrach.        | 1         | Funkcjonalne      |
| REQ-008       | Analiza sprzedaży            | System powinien oferować narzędzia do analizy wyników sprzedaży dla przedstawicieli handlowych.       | 2         | Funkcjonalne      |
| REQ-009       | Bezpieczeństwo danych        | System powinien zapewniać bezpieczne przechowywanie i transmisję danych użytkowników.                 | 1         | Pozafunkcjonalne  |
| REQ-010       | Obsługa wielu języków        | System powinien obsługiwać wiele języków, aby umożliwić korzystanie z aplikacji przez użytkowników z różnych krajów. | 3         | Pozafunkcjonalne  |
| REQ-011       | Responsywność interfejsu     | Interfejs użytkownika powinien być responsywny i dostosowany do różnych rozdzielczości ekranów.       | 2         | Pozafunkcjonalne  |
| REQ-012       | Integracja z systemami CRM   | System powinien być zintegrowany z istniejącymi systemami CRM używanymi przez firmę.                  | 2         | Funkcjonalne      |
| REQ-013       | Automatyczne aktualizacje    | System powinien wspierać automatyczne aktualizacje aplikacji bez potrzeby interwencji użytkownika.    | 3         | Pozafunkcjonalne  |
| REQ-014       | Obsługa offline              | System powinien umożliwiać dostęp do kluczowych funkcji w trybie offline.                             | 1         | Funkcjonalne      |
| REQ-015       | Raportowanie błędów          | System powinien automatycznie raportować błędy i awarie do zespołu wsparcia technicznego.             | 2         | Pozafunkcjonalne  |

# Scenariusze testów

## Scenariusz testowy 1: Logowanie użytkownika

- **Identyfikator**: TC-001
- **Nazwa**: Test logowania użytkownika
- **Opis**: Test sprawdzający możliwość logowania się użytkownika do systemu.
- **Warunki wstępne**: System jest uruchomiony, użytkownik ma założone konto.
- **Kroki**:
  1. Otwórz aplikację EasySales Mobile.
  2. Wprowadź poprawny identyfikator użytkownika.
  3. Wprowadź poprawne hasło użytkownika.
  4. Kliknij przycisk "Zaloguj się".
- **Oczekiwany wynik**: Użytkownik zostaje poprawnie zalogowany i przekierowany do ekranu głównego aplikacji.

## Scenariusz testowy 2: Przeglądanie produktów

- **Identyfikator**: TC-002
- **Nazwa**: Test przeglądania produktów
- **Opis**: Test sprawdzający możliwość przeglądania dostępnych produktów wraz z ich opisami i cenami.
- **Warunki wstępne**: Użytkownik jest zalogowany do systemu.
- **Kroki**:
  1. Otwórz zakładkę "Produkty".
  2. Przeglądaj listę dostępnych produktów.
  3. Kliknij na wybrany produkt, aby zobaczyć jego szczegóły.
- **Oczekiwany wynik**: Użytkownik może przeglądać listę produktów oraz wyświetlać szczegółowe informacje o każdym z nich.

## Scenariusz testowy 3: Dodawanie produktów do koszyka

- **Identyfikator**: TC-003
- **Nazwa**: Test dodawania produktów do koszyka
- **Opis**: Test sprawdzający możliwość dodawania produktów do koszyka zakupowego.
- **Warunki wstępne**: Użytkownik jest zalogowany do systemu.
- **Kroki**:
  1. Otwórz zakładkę "Produkty".
  2. Wybierz produkt do dodania do koszyka.
  3. Kliknij przycisk "Dodaj do koszyka".
  4. Otwórz koszyk zakupowy.
- **Oczekiwany wynik**: Wybrany produkt jest widoczny w koszyku zakupowym.

## Scenariusz testowy 4: Składanie zamówienia

- **Identyfikator**: TC-004
- **Nazwa**: Test składania zamówienia
- **Opis**: Test sprawdzający możliwość składania zamówienia i wyboru metody płatności oraz dostawy.
- **Warunki wstępne**: Użytkownik jest zalogowany do systemu, koszyk zakupowy zawiera co najmniej jeden produkt.
- **Kroki**:
  1. Otwórz koszyk zakupowy.
  2. Kliknij przycisk "Złóż zamówienie".
  3. Wybierz metodę płatności.
  4. Wybierz metodę dostawy.
  5. Potwierdź zamówienie.
- **Oczekiwany wynik**: Zamówienie zostaje poprawnie złożone, a użytkownik otrzymuje potwierdzenie.

---

# Sprawozdanie z wykonania scenariuszy testów

## Scenariusz testowy 1: Logowanie użytkownika

- **Identyfikator**: TC-001
- **Wynik**: 
  - **Status**: Zakończono pomyślnie
  - **Uwagi**: Użytkownik został poprawnie zalogowany i przekierowany do ekranu głównego aplikacji.

## Scenariusz testowy 2: Przeglądanie produktów

- **Identyfikator**: TC-002
- **Wynik**: 
  - **Status**: Zakończono pomyślnie
  - **Uwagi**: Użytkownik mógł przeglądać listę produktów oraz wyświetlać szczegółowe informacje o każdym z nich.

## Scenariusz testowy 3: Dodawanie produktów do koszyka

- **Identyfikator**: TC-003
- **Wynik**: 
  - **Status**: Zakończono pomyślnie
  - **Uwagi**: Wybrany produkt był widoczny w koszyku zakupowym.

## Scenariusz testowy 4: Składanie zamówienia

- **Identyfikator**: TC-004
- **Wynik**: 
  - **Status**: Zakończono pomyślnie
  - **Uwagi**: Zamówienie zostało poprawnie złożone, a użytkownik otrzymał potwierdzenie.

































4. Testy
a. Scenariusze testów
b. Sprawozdanie z wykonania scenariuszy testów
