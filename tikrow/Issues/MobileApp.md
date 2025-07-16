# Issues – Tikrow Mobile App

## 1. Formularz rejestracji – brak reakcji na szybkie wpisywanie znaków

### Opis:
W formularzu rejestracyjnym dla pracowników, podczas szybkiego wprowadzania znaków (np. numeru telefonu), część z nich nie zostaje zarejestrowana przez aplikację. Problem dotyczy opóźnionej reakcji pola tekstowego, co prowadzi do **gubienia znaków** przy szybszym pisaniu.

---

### Kroki do reprodukcji:
1. Uruchom aplikację mobilną Tikrow.
2. Przejdź do zakładki **„Załóż konto”** w sekcji **„Nie masz konta? Zarejestruj się”**.
3. Kliknij pole **„Numer telefonu komórkowego”**.
4. Szybko wprowadź ciąg cyfr (np. z klawiatury systemowej).

---

### Aktualne zachowanie:
- Część znaków nie pojawia się w polu formularza – pole nie nadąża za tempem wpisywania, co może prowadzić do błędnych danych.

---

### Oczekiwane zachowanie:
- Wszystkie znaki powinny być rejestrowane i wyświetlane natychmiast, niezależnie od tempa ich wprowadzania.

---

### Środowisko:
- **Wersja:** Produkcyjna
- **System:** Android 13
- **Urządzenie:** Samsung Galaxy S20 Ultra

---

### Priorytet:
Niski
