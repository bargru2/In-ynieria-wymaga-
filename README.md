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

**Identyfikator przypadków testowych:** TC-001  
**Nazwa:** Test logowania użytkownika  
**Opis:** Test sprawdzający możliwość logowania się użytkownika do systemu.  
**Warunki wstępne:** System jest uruchomiony, użytkownik ma założone konto.  

**Kroki:**
1. Otwórz aplikację EasySales Mobile.
2. Wprowadź poprawny identyfikator użytkownika.
3. Wprowadź poprawne hasło użytkownika.
4. Kliknij przycisk "Zaloguj się".

**Oczekiwany wynik:** Użytkownik zostaje poprawnie zalogowany i przekierowany do ekranu głównego aplikacji.

---

## Scenariusz testowy 2: Przeglądanie produktów

**Identyfikator przypadków testowych:** TC-002  
**Nazwa:** Test przeglądania dostępnych produktów  
**Opis:** Test sprawdzający możliwość przeglądania produktów z opisami i cenami.  
**Warunki wstępne:** System jest uruchomiony, użytkownik jest zalogowany.  

**Kroki:**
1. Otwórz aplikację EasySales Mobile.
2. Przejdź do sekcji produktów.
3. Przeglądaj listę dostępnych produktów.
4. Kliknij na wybrany produkt, aby zobaczyć szczegóły.

**Oczekiwany wynik:** Użytkownik widzi listę produktów z opisami i cenami oraz może przeglądać szczegóły wybranego produktu.

---

## Scenariusz testowy 3: Dodawanie produktów do koszyka

**Identyfikator przypadków testowych:** TC-003  
**Nazwa:** Test dodawania produktu do koszyka  
**Opis:** Test sprawdzający możliwość dodawania produktów do koszyka zakupowego.  
**Warunki wstępne:** System jest uruchomiony, użytkownik jest zalogowany.  

**Kroki:**
1. Otwórz aplikację EasySales Mobile.
2. Przejdź do sekcji produktów.
3. Wybierz produkt do dodania do koszyka.
4. Kliknij przycisk "Dodaj do koszyka".

**Oczekiwany wynik:** Produkt zostaje dodany do koszyka zakupowego.

---

## Scenariusz testowy 4: Składanie zamówienia

**Identyfikator przypadków testowych:** TC-004  
**Nazwa:** Test składania zamówienia  
**Opis:** Test sprawdzający możliwość składania zamówienia z wyborem metody płatności oraz dostawy.  
**Warunki wstępne:** System jest uruchomiony, użytkownik ma produkty w koszyku.  

**Kroki:**
1. Otwórz aplikację EasySales Mobile.
2. Przejdź do koszyka zakupowego.
3. Kliknij przycisk "Złóż zamówienie".
4. Wybierz metodę płatności oraz dostawy.
5. Potwierdź zamówienie.

**Oczekiwany wynik:** Zamówienie jest składane, a użytkownik otrzymuje potwierdzenie.

---

## Scenariusz testowy 5: Przeglądanie historii zamówień

**Identyfikator przypadków testowych:** TC-005  
**Nazwa:** Test przeglądania historii zamówień  
**Opis:** Test sprawdzający możliwość przeglądania historii zamówień użytkownika.  
**Warunki wstępne:** System jest uruchomiony, użytkownik jest zalogowany.  

**Kroki:**
1. Otwórz aplikację EasySales Mobile.
2. Przejdź do sekcji "Historia zamówień".
3. Przeglądaj listę zamówień.
4. Kliknij na wybrane zamówienie, aby zobaczyć szczegóły.

**Oczekiwany wynik:** Użytkownik widzi historię swoich zamówień z możliwością przeglądania szczegółów.

---

## Scenariusz testowy 6: Powiadomienia push

**Identyfikator przypadków testowych:** TC-006  
**Nazwa:** Test powiadomień push  
**Opis:** Test sprawdzający wysyłanie powiadomień push o nowych ofertach i statusie zamówień.  
**Warunki wstępne:** System jest uruchomiony, użytkownik jest zalogowany.  

**Kroki:**
1. Upewnij się, że użytkownik ma włączone powiadomienia push.
2. Sprawdź, czy użytkownik otrzymuje powiadomienie o nowej ofercie.
3. Sprawdź, czy użytkownik otrzymuje powiadomienie o statusie zamówienia.

**Oczekiwany wynik:** Użytkownik otrzymuje powiadomienia push o nowych ofertach i statusie zamówienia.

---

## Scenariusz testowy 7: Wyszukiwanie produktów

**Identyfikator przypadków testowych:** TC-007  
**Nazwa:** Test wyszukiwania produktów  
**Opis:** Test sprawdzający możliwość wyszukiwania produktów po nazwie, kategorii lub innych parametrach.  
**Warunki wstępne:** System jest uruchomiony, użytkownik jest zalogowany.  

**Kroki:**
1. Otwórz aplikację EasySales Mobile.
2. Przejdź do sekcji wyszukiwania.
3. Wprowadź nazwę produktu, kategorię lub inne parametry.
4. Kliknij przycisk "Szukaj".

**Oczekiwany wynik:** System zwraca listę produktów spełniających kryteria wyszukiwania.

---

## Scenariusz testowy 8: Analiza sprzedaży

**Identyfikator przypadków testowych:** TC-008  
**Nazwa:** Test analizy wyników sprzedaży  
**Opis:** Test sprawdzający dostęp do narzędzi analizy sprzedaży dla przedstawicieli handlowych.  
**Warunki wstępne:** System jest uruchomiony, użytkownik jest przedstawicielem handlowym.  

**Kroki:**
1. Otwórz aplikację EasySales Mobile.
2. Przejdź do sekcji analizy sprzedaży.
3. Wybierz okres i inne parametry analizy.
4. Kliknij przycisk "Analizuj".

**Oczekiwany wynik:** System generuje i wyświetla wyniki analizy sprzedaży zgodnie z wybranymi parametrami.

---

## Scenariusz testowy 9: Bezpieczeństwo danych

**Identyfikator przypadków testowych:** TC-009  
**Nazwa:** Test bezpieczeństwa danych  
**Opis:** Test sprawdzający bezpieczne przechowywanie i transmisję danych użytkowników.  
**Warunki wstępne:** System jest uruchomiony.  

**Kroki:**
1. Otwórz aplikację EasySales Mobile.
2. Przejdź do sekcji logowania.
3. Sprawdź, czy dane logowania są przesyłane z użyciem protokołu HTTPS.
4. Zaloguj się i sprawdź, czy dane użytkownika są przechowywane w bezpieczny sposób.

**Oczekiwany wynik:** Dane użytkownika są bezpiecznie przesyłane i przechowywane.

---

## Scenariusz testowy 10: Obsługa wielu języków

**Identyfikator przypadków testowych:** TC-010  
**Nazwa:** Test obsługi wielu języków  
**Opis:** Test sprawdzający możliwość korzystania z aplikacji w różnych językach.  
**Warunki wstępne:** System jest uruchomiony, użytkownik jest zalogowany.  

**Kroki:**
1. Otwórz aplikację EasySales Mobile.
2. Przejdź do ustawień języka.
3. Wybierz inny język.
4. Sprawdź, czy interfejs użytkownika zmienia się na wybrany język.

**Oczekiwany wynik:** System obsługuje wybrany język i zmienia interfejs użytkownika zgodnie z ustawieniami.

---

## Scenariusz testowy 11: Responsywność interfejsu

**Identyfikator przypadków testowych:** TC-011  
**Nazwa:** Test responsywności interfejsu  
**Opis:** Test sprawdzający, czy interfejs użytkownika jest responsywny i dostosowany do różnych rozdzielczości ekranów.  
**Warunki wstępne:** System jest uruchomiony, użytkownik jest zalogowany.  

**Kroki:**
1. Otwórz aplikację EasySales Mobile na różnych urządzeniach (smartfon, tablet, komputer).
2. Sprawdź, czy interfejs użytkownika jest dostosowany do rozdzielczości ekranu każdego urządzenia.

**Oczekiwany wynik:** Interfejs użytkownika jest responsywny i dostosowany do różnych rozdzielczości ekranów.

---

## Scenariusz testowy 12: Integracja z systemami CRM

**Identyfikator przypadków testowych:** TC-012  
**Nazwa:** Test integracji z systemami CRM  
**Opis:** Test sprawdzający integrację aplikacji z istniejącymi systemami CRM.  
**Warunki wstępne:** System jest uruchomiony, użytkownik jest zalogowany.  

**Kroki:**
1. Otwórz aplikację EasySales Mobile.
2. Przejdź do sekcji integracji z CRM.
3. Sprawdź, czy dane z CRM są synchronizowane z aplikacją.

**Oczekiwany wynik:** System poprawnie synchronizuje dane z istniejącymi systemami CRM.

---

## Scenariusz testowy 13: Automatyczne aktualizacje

**Identyfikator przypadków testowych:** TC-013  
**Nazwa:** Test automatycznych aktualizacji  
**Opis:** Test sprawdzający wsparcie dla automatycznych aktualizacji aplikacji.  
**Warunki wstępne:** System jest uruchomiony, użytkownik jest zalogowany.  

**Kroki:**
1. Otwórz aplikację EasySales Mobile.
2. Sprawdź, czy aplikacja automatycznie aktualizuje się do najnowszej wersji bez interwencji użytkownika.

**Oczekiwany wynik:** System wspiera automatyczne aktualizacje aplikacji.

---

## Scenariusz testowy 14: Obsługa offline

**Identyfikator przypadków testowych:** TC-014  
**Nazwa:** Test obsługi offline  
**Opis:** Test sprawdzający dostęp do kluczowych funkcji w trybie offline.  
**Warunki wstępne:** System jest uruchomiony, użytkownik jest zalogowany.  

**Kroki:**
1. Otwórz aplikację EasySales Mobile.
2. Wyłącz połączenie internetowe.
3. Sprawdź, czy użytkownik może korzystać z kluczowych funkcji aplikacji w trybie offline.

**Oczekiwany wynik:** System umożliwia dostęp do kluczowych funkcji w trybie offline.

---

## Scenariusz testowy 15: Raportowanie błędów

**Identyfikator przypadków testowych:** TC-015  
**Nazwa:** Test raportowania błędów  
**Opis:** Test sprawdzający automatyczne raportowanie błędów i awarii do zespołu wsparcia technicznego.  
**Warunki wstępne:** System jest uruchomiony, użytkownik jest zalogowany.  

**Kroki:**
1. Otwórz aplikację EasySales Mobile.
2. Wymuś wystąpienie błędu lub awarii.
3. Sprawdź, czy system automatycznie raportuje błąd do zespołu wsparcia technicznego.

**Oczekiwany wynik:** System automatycznie raportuje błędy i awarie do zespołu wsparcia technicznego.

---

# Sprawozdanie z wykonania scenariuszy testów

## Scenariusz testowy 1: Logowanie użytkownika

**Identyfikator:** TC-001  
**Wynik:**
- Status: Zakończono pomyślnie
- Uwagi: Użytkownik został poprawnie zalogowany i przekierowany do ekranu głównego aplikacji.

---

## Scenariusz testowy 2: Przeglądanie produktów

**Identyfikator:** TC-002  
**Wynik:**
- Status: Zakończono pomyślnie
- Uwagi: Lista produktów wyświetlona zgodnie z oczekiwaniami, możliwość przeglądania szczegółów produktów działa poprawnie.

---

## Scenariusz testowy 3: Dodawanie produktów do koszyka

**Identyfikator:** TC-003  
**Wynik:**
- Status: Zakończono pomyślnie
- Uwagi: Dodawanie produktów do koszyka działa sprawnie, produkt został dodany zgodnie z oczekiwaniami.

---

## Scenariusz testowy 4: Składanie zamówienia

**Identyfikator:** TC-004  
**Wynik:**
- Status: Zakończono pomyślnie
- Uwagi: Składanie zamówienia przebiegło bez problemów, wybór metody płatności oraz dostawy możliwy i funkcjonalny.

---

## Scenariusz testowy 5: Przeglądanie historii zamówień

**Identyfikator:** TC-005  
**Wynik:**
- Status: Zakończono pomyślnie
- Uwagi: Historia zamówień jest wyświetlana poprawnie, użytkownik może przeglądać szczegóły zamówień bez problemów.

---

## Scenariusz testowy 6: Powiadomienia push

**Identyfikator:** TC-006  
**Wynik:**
- Status: Zakończono pomyślnie
- Uwagi: Powiadomienia push o nowych ofertach oraz statusie zamówienia są wysyłane i odbierane prawidłowo przez użytkownika.

---

## Scenariusz testowy 7: Wyszukiwanie produktów

**Identyfikator:** TC-007  
**Wynik:**
- Status: Zakończono pomyślnie
- Uwagi: Wyszukiwanie produktów po nazwie, kategorii oraz innych parametrach działa sprawnie, lista produktów jest filtrowana zgodnie z wprowadzonymi kryteriami.

---

## Scenariusz testowy 8: Analiza sprzedaży

**Identyfikator:** TC-008  
**Wynik:**
- Status: Zakończono pomyślnie
- Uwagi: Narzędzia analizy sprzedaży są dostępne i generują wyniki zgodnie z wybranymi parametrami, funkcjonalność jest zgodna z oczekiwaniami.

---

## Scenariusz testowy 9: Bezpieczeństwo danych

**Identyfikator:** TC-009  
**Wynik:**
- Status: Zakończono pomyślnie
- Uwagi: Dane logowania są przesyłane z użyciem protokołu HTTPS, dane użytkowników przechowywane są w bezpieczny sposób.

---

## Scenariusz testowy 10: Obsługa wielu języków

**Identyfikator:** TC-010  
**Wynik:**
- Status: Zakończono pomyślnie
- Uwagi: Aplikacja obsługuje zmianę języka interfejsu użytkownika zgodnie z ustawieniami użytkownika.

---

## Scenariusz testowy 11: Responsywność interfejsu

**Identyfikator:** TC-011  
**Wynik:**
- Status: Zakończono pomyślnie
- Uwagi: Interfejs użytkownika jest responsywny i dostosowany do różnych rozdzielczości ekranów (smartfon, tablet, komputer).

---

## Scenariusz testowy 12: Integracja z systemami CRM

**Identyfikator:** TC-012  
**Wynik:**
- Status: Zakończono pomyślnie
- Uwagi: Dane z CRM są synchronizowane z aplikacją EasySales Mobile zgodnie z oczekiwaniami.

---

## Scenariusz testowy 13: Automatyczne aktualizacje

**Identyfikator:** TC-013  
**Wynik:**
- Status: Zakończono pomyślnie
- Uwagi: Aplikacja wspiera automatyczne aktualizacje do najnowszych wersji bez interwencji użytkownika.

---

## Scenariusz testowy 14: Obsługa offline

**Identyfikator:** TC-014  
**Wynik:**
- Status: Zakończono pomyślnie
- Uwagi: Kluczowe funkcje aplikacji są dostępne i działają poprawnie w trybie offline.

---

## Scenariusz testowy 15: Raportowanie błędów

**Identyfikator:** TC-015  
**Wynik:**
- Status: Zakończono pomyślnie
- Uwagi: System automatycznie raportuje błędy i awarie do zespołu wsparcia technicznego.

























