# Testy funkcjonalne - Logowanie do Tikrow

Testy pozytywne oraz negatywne logowania do aplikacji.

---

## Test Case 1: Logowanie z poprawnymi danymi

**Preconditions:**

1. Zainstalowana aplikacja Tikrow na urządzeniu mobilnym
2. Dostęp do internetu na urządzeniu
3. Założone konto w aplikacji
4. Formularz logowania jest widoczny
5. Aplikacja jest dostępna

**Steps:**

1. Uzytkownik otwiera aplikację mobilną Tikrow  
   **Expected result:**  
   Aplikacja zostaje otwarta, widoczny jest ekran logowania

2. Użytkownik wypełnia następujące pola prawidłowymi danymi:

   - Numer telefonu - poprawny, zarejestrowany w systemie
   - Hasło - poprawne, zgodne z wymaganiami  
     **Expected result:**  
     Pola formularza są wypełnione

3. Użytkownik naciska przycisk Zaloguj się  
   **Expected result:**
   - Formularz zostaje przesłany
   - Następuje przekierowanie do ekranu głównego
   - Pojawia się panel użytkownika z widocznymi ofertami pracy

---

## Test Case 2: Logowanie z pustym polem "Numer telefonu"

**Preconditions:**

1. Zainstalowana aplikacja Tikrow na urządzeniu mobilnym
2. Dostęp do internetu na urządzeniu
3. Założone konto w aplikacji
4. Formularz logowania jest widoczny
5. Aplikacja jest dostępna

**Steps:**

1. Użytkownik otwiera aplikację mobilną Tikrow  
   **Expected result:**  
   Aplikacja zostaje otwarta, widoczny jest ekran logowania

2. Użytkownik wypełnia następujące pola prawidłowymi danymi:

   - Hasło - poprawne, zgodne z wymaganiami  
     Pole "Numer telefonu" pozostaje puste  
     **Expected result:**  
     Wypełnione jest pole "Hasło", pole "Numer telefonu" pozostaje puste

3. Użytkownik naciska przycisk zaloguj się  
   **Expected result:**  
   Pod polem "Numer telefonu" pojawia się komunikat walidacyjny w kolorze czerwonym o treści **Wymagane.**  
   Aplikacja nie przeładowuje się

---

## Test Case 3: Logowanie z pustym polem "Hasło"

**Preconditions:**

1. Zainstalowana aplikacja Tikrow na urządzeniu mobilnym
2. Dostęp do internetu na urządzeniu
3. Założone konto w aplikacji
4. Formularz logowania jest widoczny
5. Aplikacja jest dostępna

**Steps:**

1. Użytkownik otwiera aplikację mobilną Tikrow  
   **Expected result:**  
   Aplikacja zostaje otwarta, widoczny jest ekran logowania

2. Użytkownik wypełnia następujące pola prawidłowymi danymi:

   - Numer telefonu - poprawny, zarejestrowany w systemie  
     Pole "Hasło" pozostaje puste  
     **Expected result:**  
     Wypełnione jest pole "Numer telefonu", pole "Hasło" pozostaje puste

3. Użytkownik naciska przycisk zaloguj się  
   **Expected result:**  
   Pod polem "Hasło" pojawia się komunikat walidacyjny w kolorze czerwonym o treści **Wymagane.**  
   Aplikacja nie przeładowuje się

---

## Test Case 4: Logowanie z wpisanym za krótkim numerem w polu "Numer telefonu"

**Preconditions:**

1. Zainstalowana aplikacja Tikrow na urządzeniu mobilnym
2. Dostęp do internetu na urządzeniu
3. Założone konto w aplikacji
4. Formularz logowania jest widoczny
5. Aplikacja jest dostępna

**Steps:**

1. Użytkownik otwiera aplikację mobilną Tikrow  
   **Expected result:**  
   Aplikacja zostaje otwarta, widoczny jest ekran logowania

2. Użytkownik wpisuje za krótki numer telefonu, np. 1234567  
   Użytkownik pole "Hasło" prawidłowymi, zgodnymi z wymaganiami danymi  
   **Expected result:**  
   Wypełnione są wszystkie pola formularza

3. Użytkownik naciska przycisk zaloguj się  
   **Expected result:**  
   Pod formularzem pojawia się komunikat walidacyjny w kolorze czerwonym o treści **Wprowadzono niepoprawny login lub hasło.**  
   Aplikacja nie przeładowuje się

---

## Test Case 5: Logowanie z wpisanym numerem zawierającym znaki specjalne oraz litery w polu "Numer telefonu"

**Preconditions:**

1. Zainstalowana aplikacja Tikrow na urządzeniu mobilnym
2. Dostęp do internetu na urządzeniu
3. Założone konto w aplikacji
4. Formularz logowania jest widoczny
5. Aplikacja jest dostępna

**Steps:**

1. Użytkownik otwiera aplikację mobilną Tikrow  
   **Expected result:**  
   Aplikacja zostaje otwarta, widoczny jest ekran logowania

2. Użytkownik wpisuje za krótki numer telefonu, np. 123456az!  
   Użytkownik wypełnia pole "Hasło" prawidłowymi, zgodnymi z wymaganiami danymi  
   **Expected result:**  
   Wypełnione są wszystkie pola formularza

3. Użytkownik naciska przycisk zaloguj się  
   **Expected result:**  
   Pod formularzem pojawia się komunikat walidacyjny w kolorze czerwonym o treści **Wprowadzono niepoprawny login lub hasło.**  
   Aplikacja nie przeładowuje się

---

## Test Case 6: Logowanie z wpisanym błędnym hasłem

**Preconditions:**

1. Zainstalowana aplikacja Tikrow na urządzeniu mobilnym
2. Dostęp do internetu na urządzeniu
3. Założone konto w aplikacji
4. Formularz logowania jest widoczny
5. Aplikacja jest dostępna

**Steps:**

1. Użytkownik otwiera aplikację mobilną Tikrow  
   **Expected result:**  
   Aplikacja zostaje otwarta, widoczny jest ekran logowania

2. Użytkownik wypełnia pole "Numer telefonu" poprawnym, zarejestrowanym w bazie numerem  
   Użytkownik uzupełnia pole "Hasło" nieprawidłowymi danymi  
   **Expected result:**  
   Wypełnione są wszystkie pola formularza

3. Użytkownik naciska przycisk zaloguj się  
   **Expected result:**  
   Pod formularzem pojawia się komunikat walidacyjny w kolorze czerwonym o treści **Wprowadzono niepoprawny login lub hasło.**  
   Aplikacja nie przeładowuje się
