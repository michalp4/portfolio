# Przypadki testowe – MrBuggy 7 (poprawione)

## Rejestracja – brak komunikatu przy pustym polu Confirm password
**ID:** BUGGY-9

**Priorytet:** Low

**Kroki do reprodukcji:**
1. Otwórz aplikację
2. Wypełnij formularz rejestracji, zostawiając pole Confirm password puste
3. Kliknij Save

**Oczekiwany rezultat:**
Powinien pojawić się komunikat "This field is required" przy polu Confirm password

---

## Formularz tworzenia konta administratora – sprawdzenie wymaganych pól
**ID:** BUGGY-10

**Priorytet:** Medium

**Kroki do reprodukcji:**
1. Uruchom aplikację
2. Przejdź do formularza tworzenia konta
3. Sprawdź, czy są pola: First name, Last name, Email, Phone number

**Oczekiwany rezultat:**
Formularz powinien zawierać wszystkie wymagane pola

---

## Wyszukiwanie w zakładce Providers – frazy ze spacją
**ID:** BUGGY-11

**Priorytet:** Medium

**Kroki do reprodukcji:**
1. Przejdź do zakładki Providers
2. Dodaj wpisy z nazwami "TEST" i "TEST 2"
3. Wyszukaj frazę "TEST "

**Oczekiwany rezultat:**
Na liście powinny się pojawić tylko wyniki z dokładnie dopasowaną spacją

---

## Wyszukiwanie w zakładce Providers – obsługa polskich znaków
**ID:** BUGGY-12

**Priorytet:** Medium

**Kroki do reprodukcji:**
1. Przejdź do zakładki Providers
2. Dodaj wpis z polskimi znakami, np. Żołądź
3. Wyszukaj wpis z polskimi znakami

**Oczekiwany rezultat:**
Wyszukiwarka powinna uwzględniać polskie znaki i pokazywać poprawne wyniki

---

## Zakładka Providers – brak odświeżenia wyników po kliknięciu X
**ID:** BUGGY-13

**Priorytet:** Medium

**Kroki do reprodukcji:**
1. Przejdź do zakładki Providers
2. Dodaj nowego providera
3. Wpisz frazę w polu wyszukiwania
4. Kliknij ikonę X

**Oczekiwany rezultat:**
Lista wyników powinna się odświeżyć i pokazać wszystkich providerów

---

## Responsywność przycisku Clear w zakładce Units przy powiększeniu ekranu
**ID:** BUGGY-14

**Priorytet:** Lowest

**Kroki do reprodukcji:**
1. Otwórz aplikację i zaloguj się na konto administratora
2. Przejdź do zakładki Units
3. Użyj kombinacji CTRL + scroll up, aby powiększyć obszar aplikacji kilka razy

**Oczekiwany rezultat:**
Przycisk Clear powinien dopasowywać się do szerokości kontenera i zachować responsywność na dużym powiększeniu

---

## Działanie skrótów klawiszowych CTRL + O i CTRL + L  w aplikacji
**ID:** BUGGY-15

**Priorytet:** Medium

**Kroki do reprodukcji:**
1. Otwórz program MrBuggy 7
2. Zaloguj się na konto administratora
3. Naciśnij kombinację klawiszy CTRL + O lub CTRL + L
4. Wpisz adres strony, np. https://google.com
5. Kliknij OK

**Oczekiwany rezultat:**
Aplikacja nie umożliwia otwarcia zewnętrznej witryny przez skrót klawiszowy

---

