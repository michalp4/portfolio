# Logowanie do Tikrow

Testy pozytywne oraz negatywne logowania do aplikacji

## Logowanie z poprawnymi danymi

**Opis:**  
Weryfikacja poprawnego logowania użytkownika z prawidłowymi danymi.

**Preconditions:**
1. Zainstalowana aplikacja Tikrow na urządzeniu mobilnym  
2. Dostęp do internetu na urządzeniu  
3. Założone konto w aplikacji  
4. Formularz logowania jest widoczny  
5. Aplikacja jest dostępna  

### Kroki testowe

1. Uzytkownik otwiera aplikację mobilną Tikrow  
   **Oczekiwany rezultat:**  
   Aplikacja zostaje otwarta, widoczny jest ekran logowania

2. Użytkownik wypełnia następujące pola prawidłowymi danymi:  
   - Numer telefonu - poprawny, zarejestrowany w systemie  
   - Hasło - poprawne, zgodne z wymaganiami  
   **Oczekiwany rezultat:**  
   Pola formularza są wypełnione

3. Użytkownik naciska przycisk Zaloguj się  
   **Oczekiwany rezultat:**  
   - Formularz zostaje przesłany  
   - Następuje przekierowanie do ekranu głównego  
   - Pojawia się panel użytkownika z widocznymi ofertami pracy  

---

## Logowanie z pustym polem "Numer telefonu"

**Opis:**  
Próba zalogowania do aplikacji bez wpisywania danych w polu "Numer telefonu".

**Preconditions:**
1. Zainstalowana aplikacja Tikrow na urządzeniu mobilnym  
2. Dostęp do internetu na urządzeniu  
3. Założone konto w aplikacji  
4. Formularz logowania jest widoczny  
5. Aplikacja jest dostępna  

### Kroki testowe

1. Użytkownik otwiera aplikację mobilną Tikrow  
   **Oczekiwany rezultat:**  
   Aplikacja zostaje otwarta, widoczny jest ekran logowania

2. Użytkownik wypełnia następujące pola prawidłowymi danymi:  
   - Hasło - poprawne, zgodne z wymaganiami  
   Pole "Numer telefonu" pozostaje puste  
   **Oczekiwany rezultat:**  
   Wypełnione jest pole "Hasło", pole "Numer telefonu" pozostaje puste

3. Użytkownik naciska przycisk zaloguj się  
   **Oczekiwany rezultat:**  
   Pod polem "Numer telefonu" pojawia się komunikat walidacyjny w kolorze czerwonym o treści **Wymagane.** Aplikacja nie przeładowuje się

---

## Logowanie z pustym polem "Hasło"

**Opis:**  
Próba zalogowania do aplikacji bez wpisywania danych w polu "Hasło".

**Preconditions:**
1. Zainstalowana aplikacja Tikrow na urządzeniu mobilnym  
2. Dostęp do internetu na urządzeniu  
3. Założone konto w aplikacji  
4. Formularz logowania jest widoczny  
5. Aplikacja jest dostępna  

### Kroki testowe

1. Użytkownik otwiera aplikację mobilną Tikrow  
   **Oczekiwany rezultat:**  
   Aplikacja zostaje otwarta, widoczny jest ekran logowania

2. Użytkownik wypełnia następujące pola prawidłowymi danymi:  
   - Numer telefonu - poprawny, zarejestrowany w systemie  
   Pole "Hasło" pozostaje puste  
   **Oczekiwany rezultat:**  
   Wypełnione jest pole "Numer telefonu", pole "Hasło" pozostaje puste

3. Użytkownik naciska przycisk zaloguj się  
   **Oczekiwany rezultat:**  
   Pod polem "Hasło" pojawia się komunikat walidacyjny w kolorze czerwonym o treści **Wymagane.** Aplikacja nie przeładowuje się

---

## Logowanie z wpisanym za krótkim numerem w polu "Numer telefonu"

**Opis:**  
Próba zalogowania do aplikacji za pomocą za krótkiego numeru telefonu.

**Preconditions:**
1. Zainstalowana aplikacja Tikrow na urządzeniu mobilnym  
2. Dostęp do internetu na urządzeniu  
3. Założone konto w aplikacji  
4. Formularz logowania jest widoczny  
5. Aplikacja jest dostępna  

### Kroki testowe

1. Użytkownik otwiera aplikację mobilną Tikrow  
   **Oczekiwany rezultat:**  
   Aplikacja zostaje otwarta, widoczny jest ekran logowania

2. Użytkownik wpisuje za krótki numer telefonu, np. 1234567  
   Użytkownik pole "Hasło" prawidłowymi, zgodnymi z wymaganiami danymi  
   **Oczekiwany rezultat:**  
   Wypełnione są wszystkie pola formularza

3. Użytkownik naciska przycisk zaloguj się  
   **Oczekiwany rezultat:**  
   Pod formularzem pojawia się komunikat walidacyjny w kolorze czerwonym o treści **Wprowadzono niepoprawny login lub hasło.** Aplikacja nie przeładowuje się

---

## Logowanie z wpisanym numerem zawierającym znaki specjalne oraz litery w polu "Numer telefonu"

**Opis:**  
Próba zalogowania do aplikacji za pomocą błędnego numeru telefonu zawierającego litery oraz znaki specjalne.

**Preconditions:**
1. Zainstalowana aplikacja Tikrow na urządzeniu mobilnym  
2. Dostęp do internetu na urządzeniu  
3. Założone konto w aplikacji  
4. Formularz logowania jest widoczny  
5. Aplikacja jest dostępna  

### Kroki testowe

1. Użytkownik otwiera aplikację mobilną Tikrow  
   **Oczekiwany rezultat:**  
   Aplikacja zostaje otwarta, widoczny jest ekran logowania

2. Użytkownik wpisuje za krótki numer telefonu, np. 123456az!  
   Użytkownik wypełnia pole "Hasło" prawidłowymi, zgodnymi z wymaganiami danymi  
   **Oczekiwany rezultat:**  
   Wypełnione są wszystkie pola formularza

3. Użytkownik naciska przycisk zaloguj się  
   **Oczekiwany rezultat:**  
   Pod formularzem pojawia się komunikat walidacyjny w kolorze czerwonym o treści **Wprowadzono niepoprawny login lub hasło.** Aplikacja nie przeładowuje się

---

## Logowanie z wpisanym błędnym hasłem

**Opis:**  
Próba zalogowania do aplikacji za pomocą błędnego hasła.

**Preconditions:**
1. Zainstalowana aplikacja Tikrow na urządzeniu mobilnym  
2. Dostęp do internetu na urządzeniu  
3. Założone konto w aplikacji  
4. Formularz logowania jest widoczny  
5. Aplikacja jest dostępna  

### Kroki testowe

1. Użytkownik otwiera aplikację mobilną Tikrow  
   **Oczekiwany rezultat:**  
   Aplikacja zostaje otwarta, widoczny jest ekran logowania

2. Użytkownik wypełnia pole "Numer telefonu" poprawnym, zarejestrowanym w bazie numerem  
   Użytkownik uzupełnia pole "Hasło" nieprawidłowymi danymi  
   **Oczekiwany rezultat:**  
   Wypełnione są wszystkie pola formularza

3. Użytkownik naciska przycisk zaloguj się  
   **Oczekiwany rezultat:**  
   Pod formularzem pojawia się komunikat walidacyjny w kolorze czerwonym o treści **Wprowadzono niepoprawny login lub hasło.** Aplikacja nie przeładowuje się
