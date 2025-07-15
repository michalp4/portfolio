# Rejestracja użytkownika

Testy rejestracji nowego użytkownika z poprawnymi i błędnymi danymi

## Rejestracja z poprawnymi danymi

**Opis:**  
Rejestracja nowego użytkownika za pomocą poprawnych danych.

**Preconditions:**

1. Zainstalowana aplikacja Tikrow na urządzeniu mobilnym
2. Dostęp do internetu na urządzeniu
3. Widoczny jest odnośnik do formularza rejestracyjnego _Załóż konto_
4. Aplikacja jest dostępna

### Kroki testowe

1. Uzytkownik otwiera aplikację mobilną Tikrow  
   **Oczekiwany rezultat:**  
   Aplikacja zostaje otwarta, widoczny jest ekran logowania

2. Uzytkownik scrolluje na sam dół do sekcji **Nie masz konta? Zarejestruj się**  
   **Oczekiwany rezultat:**  
   Widoczna sekcja **Nie masz konta? Zarejestruj się** oraz przycisk do formularza rejestracyjnego _Załóż konto_

3. Użytkownik naciska przycisk _Załóż konto_  
   **Oczekiwany rezultat:**  
   Aplikacja przechodzi do okna **Rejestracja dla Pracowników**

4. Użytkownik wypełnia następujące pola prawidłowymi danymi:

   - Numer telefonu - poprawny, 6 cyfr, bez liter i znaków specjalnych
   - Kod pocztowy - poprawny, 2 cyfry, myślnik, 3 cyfry  
     **Oczekiwany rezultat:**  
     Wszystkie pola formularza są wypełnione

5. Użytkownik zaznacza checkbox _Zapoznałe/am się i akceptuję Regulamin Tikrow_  
   **Oczekiwany rezultat:**  
   Checkbox zostaje zaznaczony

6. Użytkownik naciska przycisk **Załóż konto**  
   **Oczekiwany rezultat:**  
   Formularz zostaje przesłany, nastepuje przejscie do okna logowania i wyświetlona zostaje informacja o poprawnej rejestracji.  
   Na podany numer telefonu wysłana zostaje wiadomość zawierająca hasło do pierwszego logowania

---

## Rejestracja z niepoprawnymi danymi - za krótki numer telefonu

**Opis:**  
Rejestracja nowego użytkownika za pomocą niepoprawnych danych - za krótki numer telefonu.

**Preconditions:**

1. Zainstalowana aplikacja Tikrow na urządzeniu mobilnym
2. Dostęp do internetu na urządzeniu
3. Widoczny jest odnośnik do formularza rejestracyjnego _Załóż konto_
4. Aplikacja jest dostępna

### Kroki testowe

1. Uzytkownik otwiera aplikację mobilną Tikrow  
   **Oczekiwany rezultat:**  
   Aplikacja zostaje otwarta, widoczny jest ekran logowania

2. Uzytkownik scrolluje na sam dół do sekcji **Nie masz konta? Zarejestruj się**  
   **Oczekiwany rezultat:**  
   Widoczna sekcja **Nie masz konta? Zarejestruj się** oraz przycisk do formularza rejestracyjnego _Załóż konto_

3. Użytkownik naciska przycisk _Załóż konto_  
   **Oczekiwany rezultat:**  
   Aplikacja przechodzi do okna **Rejestracja dla Pracowników**

4. Użytkownik wypełnia pole "Numer telefonu" numerem po mniejszej liczbie cyfr niż 9, np. 123456  
   Użytkownik wypełnia pole "Kod pocztowy" poprawnymi danym  
   **Oczekiwany rezultat:**  
   Wszystkie pola formularza są wypełnione

5. Użytkownik zaznacza checkbox _Zapoznałe/am się i akceptuję Regulamin Tikrow_  
   **Oczekiwany rezultat:**  
   Checkbox zostaje zaznaczony

6. Użytkownik naciska przycisk **Załóż konto**  
   **Oczekiwany rezultat:**  
   Pod polem "Numer telefonu" wyświetlony zostaje komunikat walidacyjny w kolorze czerwonym **Numer telefonu musi zawierać 9 cyfr.** Formularz nie jest przesyłany

---

## Rejestracja z niepoprawnymi danymi - błędny kod pocztowy

**Opis:**  
Rejestracja nowego użytkownika za pomocą błędnych danych - niepoprawny kod pocztowy.

**Preconditions:**

1. Zainstalowana aplikacja Tikrow na urządzeniu mobilnym
2. Dostęp do internetu na urządzeniu
3. Widoczny jest odnośnik do formularza rejestracyjnego _Załóż konto_
4. Aplikacja jest dostępna

### Kroki testowe

1. Uzytkownik otwiera aplikację mobilną Tikrow  
   **Oczekiwany rezultat:**  
   Aplikacja zostaje otwarta, widoczny jest ekran logowania

2. Uzytkownik scrolluje na sam dół do sekcji **Nie masz konta? Zarejestruj się**  
   **Oczekiwany rezultat:**  
   Widoczna sekcja **Nie masz konta? Zarejestruj się** oraz przycisk do formularza rejestracyjnego _Załóż konto_

3. Użytkownik naciska przycisk _Załóż konto_  
   **Oczekiwany rezultat:**  
   Aplikacja przechodzi do okna **Rejestracja dla Pracowników**

4. Użytkownik wypełnia pole "Numer telefonu" poprawnymi danymi  
   Użytkownik wypełnia pole "Kod pocztowy" niepoprawnym kodem, np. 12345  
   **Oczekiwany rezultat:**  
   Wszystkie pola formularza są wypełnione

5. Użytkownik zaznacza checkbox _Zapoznałe/am się i akceptuję Regulamin Tikrow_  
   **Oczekiwany rezultat:**  
   Checkbox zostaje zaznaczony

6. Użytkownik naciska przycisk **Załóż konto**  
   **Oczekiwany rezultat:**  
   Pod polem "Kod pocztowy" wyświetlony zostaje komunikat walidacyjny w kolorze czerwonym **Niepoprawny format kodu pocztowego.** Formularz nie jest przesyłany
