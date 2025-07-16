# Issues – Tikrow Web Page

## 1. Dropdown w sekcji FAQ nie zamyka się poprawnie, gdy wcześniej rozwinięto inne pytanie

### Opis:
Na podstronie FAQ, jeśli użytkownik rozwinie jedno pytanie, a następnie – bez jego zamykania – rozwinie kolejne, to próba zamknięcia pierwszego pytania prowadzi do niespójnego działania dropdownu i ikony strzałki:

- pierwsze kliknięcie **nie zamyka dropdownu**, ale **przywraca ikonę do pozycji domyślnej** (strzałka w dół),
- drugie kliknięcie **zamyka dropdown**, ale **ikona ponownie zmienia się na strzałkę w górę** – mimo że dropdown został zamknięty.

### Kroki do reprodukcji:
1. Wejdź na stronę: [https://tikrow.com/dla-pracownikow/faq/](https://tikrow.com/dla-pracownikow/faq/)
2. Kliknij pytanie: **"Jak mogę się zarejestrować w Tikrow?"**
3. Bez jego zamykania, kliknij kolejne pytanie: **"Kto może się zarejestrować w aplikacji?"**
4. Kliknij ponownie pierwsze pytanie.
5. Kliknij je jeszcze raz.

### Aktualne zachowanie:
- **1. kliknięcie:** Ikona przy pytaniu „Jak mogę się zarejestrować…” zmienia się z góry na dół, ale dropdown pozostaje otwarty.
- **2. kliknięcie:** Dropdown zamyka się, ale ikona ponownie zmienia się na strzałkę skierowaną w górę – mimo że dropdown jest już zamknięty.

### Oczekiwane zachowanie:
Kliknięcie w rozwinięte pytanie powinno:
- zamknąć jego dropdown,
- przywrócić ikonę do pozycji domyślnej (strzałka w dół),
- zachowywać się spójnie niezależnie od liczby wcześniej otwartych pytań.

### Środowisko:
- **Wersja:** Produkcyjna
- **System:** Windows 11 x64  
- **Przeglądarka:** OperaGX

### Priorytet:
Niski (problem wizualno-logiczny, bez wpływu na funkcjonalność strony)
