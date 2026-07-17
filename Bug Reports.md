
# Bug Report – SauceDemo

## Opis projektu

Dokument zawiera zgłoszenia błędów wykrytych podczas testów eksploracyjnych aplikacji *SauceDemo* z wykorzystaniem konta testowego problem_user.

---

# BUG-001 – Brak możliwości zmiany sposobu sortowania produktów

## Informacje

| Pole | Wartość |
|------|----------|
| ID | BUG-001 |
| Priorytet | Medium |
| Typ zgłoszenia | Bug |
| Status | Open |
| Moduł | Inventory |

### Kroki reprodukcji

1. Zaloguj się jako problem_user.
2. Przejdź do listy produktów.
3. Kliknij listę rozwijaną sortowania.
4. Wybierz opcję *Name (Z to A)*.

### Oczekiwany rezultat

Produkty zostają posortowane zgodnie z wybraną opcją.

### Rzeczywisty rezultat

Zmiana sposobu sortowania nie działa pomimo dostępnych opcji.

---

# BUG-002 – Brak możliwości usunięcia produktu z koszyka z poziomu strony Inventory

## Informacje

| Pole | Wartość |
|------|----------|
| ID | BUG-002 |
| Priorytet | High |
| Typ zgłoszenia | Bug |
| Status | Open |
| Moduł | Inventory |

### Kroki reprodukcji

1. Zaloguj się jako problem_user.
2. Dodaj dowolny produkt do koszyka.
3. Spróbuj usunąć produkt z poziomu strony głównej.

### Oczekiwany rezultat

Po dodaniu produktu do koszyka przycisk *Add to cart* zmienia się na *Remove*, umożliwiając usunięcie produktu.

### Rzeczywisty rezultat

Produkt pozostaje w koszyku i nie można go usunąć z poziomu strony Inventory.

---

# BUG-003 – Brak możliwości wpisania nazwiska podczas procesu Checkout

## Informacje

| Pole | Wartość |
|------|----------|
| ID | BUG-003 |
| Priorytet | High |
| Typ zgłoszenia | Bug |
| Status | Open |
| Moduł | Checkout |

### Kroki reprodukcji

1. Zaloguj się jako problem_user.
2. Dodaj produkt do koszyka.
3. Przejdź do procesu Checkout.
4. Wpisz imię.
5. Spróbuj wpisać nazwisko w polu *Last Name*.

### Oczekiwany rezultat

Pole *Last Name* umożliwia wprowadzenie nazwiska.

### Rzeczywisty rezultat

Pole *Last Name* nie pozwala na wpisanie żadnych znaków, co uniemożliwia przejście do kolejnego etapu zamówienia.

---

# BUG-004 – Niepoprawne wyświetlanie zdjęć produktów

## Informacje

| Pole | Wartość |
|------|----------|
| ID | BUG-004 |
| Priorytet | Medium |
| Typ zgłoszenia | Bug |
| Status | Open |
| Moduł | Inventory |

### Kroki reprodukcji

1. Zaloguj się jako problem_user.
2. Przejdź do strony z listą produktów.
3. Zweryfikuj zdjęcia produktów.

### Oczekiwany rezultat

Każdy produkt wyświetla przypisane do niego zdjęcie.

### Rzeczywisty rezultat

Zamiast zdjęć produktów wyświetlane jest zdjęcie psa dla wielu produktów.

---

# Podsumowanie

Podczas testów eksploracyjnych aplikacji SauceDemo z wykorzystaniem konta problem_user wykryto cztery błędy dotyczące działania aplikacji. Wszystkie zgłoszenia zostały udokumentowane zgodnie z dobrymi praktykami raportowania błędów i mogą zostać odtworzone zgodnie z opisanymi krokami reprodukcji.
