# Rejestracja użytkownika

Testy rejestracji nowego użytkownika z poprawnymi i błędnymi danymi

---

## Rejestracja z poprawnymi danymi

**Opis:**  
Rejestracja nowego użytkownika za pomocą poprawnych danych

**Warunki wstępne:**

1. Zainstalowana aplikacja Tikrow na urządzeniu mobilnym
2. Dostęp do internetu na urządzeniu
3. Widoczny jest odnośnik do formularza rejestracyjnego _Załóż konto_
4. Aplikacja jest dostępna

### Kroki testowe

1. **Akcja:** Uzytkownik otwiera aplikację mobilną Tikrow  
   **Oczekiwany rezultat:** Aplikacja zostaje otwarta, widoczny jest ekran logowania

2. **Akcja:** Uzytkownik scrolluje na sam dół do sekcji **Nie masz konta? Zarejestruj się**  
   **Oczekiwany rezultat:** Widoczna sekcja **Nie masz konta? Zarejestruj się** oraz przycisk do formularza rejestracyjnego _Załóż konto_

3. **Akcja:** Użytkownik naciska przycisk _Załóż konto_  
   **Oczekiwany rezultat:** Aplikacja przechodzi do okna **Rejestracja dla Pracowników**

4. **Akcja:** Użytkownik wypełnia następujące pola prawidłowymi danymi:

   - Numer telefonu - poprawny, 6 cyfr, bez liter i znaków specjalnych
   - Kod pocztowy - poprawny, 2 cyfry, myślnik, 3 cyfry  
     **Oczekiwany rezultat:** Wszystkie pola formularza są wypełnione

5. **Akcja:** Użytkownik zaznacza checkbox _Zapoznałe/am się i akceptuję Regulamin Tikrow_  
   **Oczekiwany rezultat:** Checkbox zostaje zaznaczony

6. **Akcja:** Użytkownik naciska przycisk **Załóż konto**  
   **Oczekiwany rezultat:**
   - Formularz zostaje przesłany, następuje przejście do okna logowania i wyświetlona zostaje informacja o poprawnej rejestracji.
   - Na podany numer telefonu wysłana zostaje wiadomość zawierająca hasło do pierwszego logowania

---

## Rejestracja z niepoprawnymi danymi - za krótki numer telefonu

**Opis:**  
Rejestracja nowego użytkownika za pomocą niepoprawnych danych - za krótki numer telefonu

**Warunki wstępne:**

1. Zainstalowana aplikacja Tikrow na urządzeniu mobilnym
2. Dostęp do internetu na urządzeniu
3. Widoczny jest odnośnik do formularza rejestracyjnego _Załóż konto_
4. Aplikacja jest dostępna

### Kroki testowe

1. **Akcja:** Uzytkownik otwiera aplikację mobilną Tikrow  
   **Oczekiwany rezultat:** Aplikacja zostaje otwarta, widoczny jest ekran logowania

2. **Akcja:** Uzytkownik scrolluje na sam dół do sekcji **Nie masz konta? Zarejestruj się**  
   **Oczekiwany rezultat:** Widoczna sekcja **Nie masz konta? Zarejestruj się** oraz przycisk do formularza rejestracyjnego _Załóż konto_

3. **Akcja:** Użytkownik naciska przycisk _Załóż konto_  
   **Oczekiwany rezultat:** Aplikacja przechodzi do okna **Rejestracja dla Pracowników**

4. **Akcja:** Użytkownik wypełnia pole "Numer telefonu" numerem po mniejszej liczbie cyfr niż 9, np. 123456  
   Użytkownik wypełnia pole "Kod pocztowy" poprawnymi danymi  
   **Oczekiwany rezultat:** Wszystkie pola formularza są wypełnione

5. **Akcja:** Użytkownik zaznacza checkbox _Zapoznałe/am się i akceptuję Regulamin Tikrow_  
   **Oczekiwany rezultat:** Checkbox zostaje zaznaczony

6. **Akcja:** Użytkownik naciska przycisk **Załóż konto**  
   **Oczekiwany rezultat:**
   - Pod polem "Numer telefonu" wyświetlony zostaje komunikat walidacyjny w kolorze czerwonym o treści **Nieprawidłowy numer telefonu**
   - Formularz nie zostaje przesłany.

---

## Rejestracja z niepoprawnymi danymi - numer telefonu zawierający niedozwolone znaki

**Opis:**  
Rejestracja nowego użytkownika za pomocą niepoprawnych danych - numer telefonu zawierający litery oraz znaki specjalne

**Warunki wstępne:**

1. Zainstalowana aplikacja Tikrow na urządzeniu mobilnym
2. Dostęp do internetu na urządzeniu
3. Widoczny jest odnośnik do formularza rejestracyjnego _Załóż konto_
4. Aplikacja jest dostępna

### Kroki testowe

1. **Akcja:** Uzytkownik otwiera aplikację mobilną Tikrow  
   **Oczekiwany rezultat:** Aplikacja zostaje otwarta, widoczny jest ekran logowania

2. **Akcja:** Uzytkownik scrolluje na sam dół do sekcji **Nie masz konta? Zarejestruj się**  
   **Oczekiwany rezultat:** Widoczna sekcja **Nie masz konta? Zarejestruj się** oraz przycisk do formularza rejestracyjnego _Załóż konto_

3. **Akcja:** Użytkownik naciska przycisk _Załóż konto_  
   **Oczekiwany rezultat:** Aplikacja przechodzi do okna **Rejestracja dla Pracowników**

4. **Akcja:** Użytkownik wypełnia pole "Numer telefonu" danymi innymi niż numeryczne  
   **Oczekiwany rezultat:**
   - Po naciśnięciu na pole formularza o nazwie "Numer telefonu" wyświetla się jedynie klawiatura numeryczna uniemożliwiając wpisanie innych znaków niż cyfry

---

## Rejestracja z niepoprawnymi danymi - za długi numer telefonu

**Opis:**  
Rejestracja nowego użytkownika za pomocą niepoprawnych danych - numer telefonu ma więcej niż 9 cyfr

**Warunki wstępne:**

1. Zainstalowana aplikacja Tikrow na urządzeniu mobilnym
2. Dostęp do internetu na urządzeniu
3. Widoczny jest odnośnik do formularza rejestracyjnego _Załóż konto_
4. Aplikacja jest dostępna

### Kroki testowe

1. **Akcja:** Uzytkownik otwiera aplikację mobilną Tikrow  
   **Oczekiwany rezultat:** Aplikacja zostaje otwarta, widoczny jest ekran logowania

2. **Akcja:** Uzytkownik scrolluje na sam dół do sekcji **Nie masz konta? Zarejestruj się**  
   **Oczekiwany rezultat:** Widoczna sekcja **Nie masz konta? Zarejestruj się** oraz przycisk do formularza rejestracyjnego _Załóż konto_

3. **Akcja:** Użytkownik naciska przycisk _Załóż konto_  
   **Oczekiwany rezultat:** Aplikacja przechodzi do okna **Rejestracja dla Pracowników**

4. **Akcja:** Użytkownik wypełnia pole "Numer telefonu" np. 10 cyframi  
   **Oczekiwany rezultat:** Wpisanie więcej niż 9 cyfr skutkuje usunięciem nadmiarowych cyfr
