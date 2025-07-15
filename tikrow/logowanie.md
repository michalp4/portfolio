# Logowanie do Tikrow

**Opis:**  
Testy funkcjonalne logowania do aplikacji mobilnej Tikrow z poprawnymi i błędnymi danymi.

---

## Logowanie z poprawnymi danymi

**Opis:**  
Logowanie istniejącego użytkownika z poprawnym numerem telefonu i hasłem.

**Preconditions:**

1. Zainstalowana aplikacja Tikrow na urządzeniu mobilnym
2. Dostęp do internetu na urządzeniu
3. Użytkownik ma założone konto i zna hasło
4. Aplikacja jest dostępna

### Kroki testowe

1. Użytkownik otwiera aplikację Tikrow  
   **Oczekiwany rezultat:**  
   Aplikacja zostaje uruchomiona, wyświetla ekran logowania

2. Użytkownik w polu "Numer telefonu" wpisuje poprawny, 9-cyfrowy numer telefonu  
   **Oczekiwany rezultat:**  
   Pole jest wypełnione poprawnym numerem

3. Użytkownik w polu "Hasło" wpisuje poprawne hasło  
   **Oczekiwany rezultat:**  
   Pole jest wypełnione hasłem

4. Użytkownik naciska przycisk **Zaloguj się**  
   **Oczekiwany rezultat:**  
   Użytkownik zostaje zalogowany do aplikacji i widzi ekran główny

---

## Logowanie z niepoprawnym numerem telefonu - za krótki numer

**Opis:**  
Logowanie użytkownika z numerem telefonu krótszym niż 9 cyfr.

**Preconditions:**

1. Zainstalowana aplikacja Tikrow na urządzeniu mobilnym
2. Dostęp do internetu na urządzeniu
3. Aplikacja jest dostępna

### Kroki testowe

1. Użytkownik otwiera aplikację Tikrow  
   **Oczekiwany rezultat:**  
   Aplikacja zostaje uruchomiona, wyświetla ekran logowania

2. Użytkownik w polu "Numer telefonu" wpisuje numer krótszy niż 9 cyfr, np. 12345  
   **Oczekiwany rezultat:**  
   Pole jest wypełnione podanym numerem

3. Użytkownik w polu "Hasło" wpisuje dowolne hasło  
   **Oczekiwany rezultat:**  
   Pole jest wypełnione hasłem

4. Użytkownik naciska przycisk **Zaloguj się**  
   **Oczekiwany rezultat:**  
   Pojawia się komunikat błędu: **Nieprawidłowy numer telefonu**

---

## Logowanie z niepoprawnym hasłem - puste pole

**Opis:**  
Logowanie użytkownika bez podania hasła.

**Preconditions:**

1. Zainstalowana aplikacja Tikrow na urządzeniu mobilnym
2. Dostęp do internetu na urządzeniu
3. Aplikacja jest dostępna

### Kroki testowe

1. Użytkownik otwiera aplikację Tikrow  
   **Oczekiwany rezultat:**  
   Aplikacja zostaje uruchomiona, wyświetla ekran logowania

2. Użytkownik w polu "Numer telefonu" wpisuje poprawny, 9-cyfrowy numer telefonu  
   **Oczekiwany rezultat:**  
   Pole jest wypełnione podanym numerem

3. Użytkownik nie wpisuje hasła (pole pozostaje puste)  
   **Oczekiwany rezultat:**  
   Pole jest puste

4. Użytkownik naciska przycisk **Zaloguj się**  
   **Oczekiwany rezultat:**  
   Pojawia się komunikat błędu: **Pole hasła nie może być puste**

---

## Logowanie z niepoprawnym hasłem - błędne hasło

**Opis:**  
Logowanie użytkownika z błędnym hasłem.

**Preconditions:**

1. Zainstalowana aplikacja Tikrow na urządzeniu mobilnym
2. Dostęp do internetu na urządzeniu
3. Aplikacja jest dostępna

### Kroki testowe

1. Użytkownik otwiera aplikację Tikrow  
   **Oczekiwany rezultat:**  
   Aplikacja zostaje uruchomiona, wyświetla ekran logowania

2. Użytkownik w polu "Numer telefonu" wpisuje poprawny, 9-cyfrowy numer telefonu  
   **Oczekiwany rezultat:**  
   Pole jest wypełnione podanym numerem

3. Użytkownik w polu "Hasło" wpisuje błędne hasło  
   **Oczekiwany rezultat:**  
   Pole jest wypełnione hasłem

4. Użytkownik naciska przycisk **Zaloguj się**  
   **Oczekiwany rezultat:**  
   Pojawia się komunikat błędu: **Nieprawidłowe hasło**
