# Przypadki testowe – MrBuggy 7

---

## Przypadek: BUGGY-9  
**Opis:** Nie pojawia się komunikat walidacyjny przy polu Confirm password  
**Priorytet:** Low  
**Status:** Do zrobienia  

**Kroki do reprodukcji:**  
1. Otwórz aplikację  
2. Wypełnij formularz rejestracji, zostawiając pole Confirm password puste  
3. Kliknij Save  

**Oczekiwany rezultat:**  
Powinien pojawić się komunikat "This field is required" przy polu Confirm password  

---

## Przypadek: BUGGY-10  
**Opis:** Przy tworzeniu konta administratora brakuje wymaganych pól  
**Priorytet:** Medium  
**Status:** Do zrobienia  

**Kroki do reprodukcji:**  
1. Uruchom aplikację  
2. Przejdź do formularza tworzenia konta  
3. Sprawdź, czy są pola: First name, Last name, Email, Phone number  

**Oczekiwany rezultat:**  
Formularz powinien zawierać wszystkie wymagane pola  

---

## Przypadek: BUGGY-11  
**Opis:** Wyszukiwarka w zakładce Providers nie uwzględnia spacji  
**Priorytet:** Medium  
**Status:** Do zrobienia  

**Kroki do reprodukcji:**  
1. Przejdź do zakładki Providers  
2. Dodaj wpisy z nazwami "TEST" i "TEST 2"  
3. Wyszukaj frazę "TEST "  

**Oczekiwany rezultat:**  
Na liście powinny się pojawić tylko wyniki z dokładnie dopasowaną spacją  

---

## Przypadek: BUGGY-12  
**Opis:** Wyszukiwarka nie uwzględnia polskich znaków  
**Priorytet:** Medium  
**Status:** Do zrobienia  

**Kroki do reprodukcji:**  
1. Przejdź do zakładki Providers  
2. Dodaj wpis z polskimi znakami, np. Żołądź  
3. Wyszukaj wpis z polskimi znakami  

**Oczekiwany rezultat:**  
Wyszukiwarka powinna uwzględniać polskie znaki i pokazywać poprawne wyniki  

---

## Przypadek: BUGGY-13  
**Opis:** Po kliknięciu w ikonę X lista wyników Providers nie jest odświeżana  
**Priorytet:** Medium  
**Status:** Do zrobienia  

**Kroki do reprodukcji:**  
1. Przejdź do zakładki Providers  
2. Dodaj nowego providera  
3. Wpisz frazę w polu wyszukiwania  
4. Kliknij ikonę X  

**Oczekiwany rezultat:**  
Lista wyników powinna się odświeżyć i pokazać wszystkich providerów  

---

## Przypadek: BUGGY-14  
**Opis:** Przycisk w zakładce Units nie jest responsywny na większych proporcjach/powiększonym ekranie aplikacji  
**Priorytet:** Lowest  
**Status:** Do zrobienia  

**Kroki do reprodukcji:**  
1. Otwórz aplikację i zaloguj się na konto administratora  
2. Przejdź do zakładki Units  
3. Użyj kombinacji CTRL + scroll up, aby powiększyć obszar aplikacji kilka razy  

**Oczekiwany rezultat:**  
Przycisk *Clear* powinien dopasowywać się do szerokości kontenera i zachować responsywność na dużym powiększeniu  

---

## Przypadek: BUGGY-15  
**Opis:** Po wywołaniu kombinacji klawiszy CTRL + O, użytkownik ma możliwość otwarcia witryny w programie  
**Priorytet:** Medium  
**Status:** Do zrobienia  

**Kroki do reprodukcji:**  
1. Otwórz program MrBuggy 7  
2. Zaloguj się na konto administratora  
3. Naciśnij kombinację klawiszy CTRL + O lub CTRL + L  
4. Wpisz adres strony, np. https://google.com  
5. Kliknij OK  

**Oczekiwany rezultat:**  
Program nie daje możliwości otwierania w aplikacji żadnych zewnętrznych elementów jak foldery, pliki, witryny www  

---
