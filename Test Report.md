# Test Report – SauceDemo

## Informacje ogólne

| Pole | Wartość |
|------|----------|
| Projekt | SauceDemo |
| Tester | Kacper Dyrcz |
| Typ testów | Testy manualne |
| Środowisko | Google Chrome / Windows 11 |
| Data rozpoczęcia | 17.07.2026 |
| Data zakończenia | 17.07.2026 |

---

# Cel testów

Celem testów było sprawdzenie poprawności działania kluczowych funkcjonalności aplikacji SauceDemo, takich jak logowanie, zarządzanie koszykiem, sortowanie produktów oraz proces składania zamówienia.

---

# Zakres testów

Przetestowane funkcjonalności:

- Logowanie użytkownika
- Zarządzanie koszykiem
- Sortowanie produktów
- Proces Checkout

Nieobjęte testami:

- Testy wydajnościowe
- Testy bezpieczeństwa
- Testy kompatybilności między przeglądarkami

---

# Wyniki testów

W ramach projektu wykonano testy manualne zgodnie z przygotowanymi przypadkami testowymi oraz przeprowadzono dodatkowe testy eksploracyjne.

Podczas testów eksploracyjnych wykryto następujące problemy:

- brak możliwości zmiany sposobu sortowania produktów,
- brak możliwości usunięcia produktu z koszyka z poziomu strony Inventory,
- brak możliwości wpisania wartości w polu *Last Name* podczas procesu Checkout,
- niepoprawne wyświetlanie zdjęć produktów (zastąpienie ich zdjęciem psa).

---

# Wykryte problemy

| ID | Opis | Status |
|----|------|--------|
| BUG-001 | Brak możliwości zmiany sposobu sortowania produktów po zalogowaniu jako problem_user. | Open |
| BUG-002 | Po dodaniu produktu do koszyka przyciskiem *Add to cart* nie ma możliwości usunięcia produktu z poziomu strony głównej (Inventory). | Open |
| BUG-003 | Podczas procesu Checkout nie można wpisać nazwiska w polu *Last Name*, co uniemożliwia poprawne ukończenie zamówienia. | Open |
| BUG-004 | Zamiast zdjęć produktów wyświetlane jest zdjęcie psa, co powoduje nieprawidłową prezentację oferty. | Open |

---

# Podsumowanie

Podczas wykonywania testów większość podstawowych funkcjonalności aplikacji działała zgodnie z oczekiwaniami. W trakcie testów wykryto jednak kilka problemów występujących dla konta problem_user, które wpływają na komfort korzystania z aplikacji.

Zidentyfikowane błędy obejmują:
- brak możliwości zmiany sposobu sortowania produktów,
- brak możliwości usunięcia produktu z koszyka z poziomu strony głównej,
- brak możliwości wpisania nazwiska podczas procesu Checkout,
- niepoprawne wyświetlanie zdjęć produktów (zastąpienie ich zdjęciem psa).

Wykryte problemy zostały zgłoszone do dalszej analizy i wymagają weryfikacji przez zespół deweloperski.

---

# Rekomendacje

- Zweryfikować działanie sortowania dla kont testowych.
- Po wprowadzeniu poprawek wykonać testy regresji dotyczące modułu Inventory.
- Kontynuować testy pozostałych kont testowych (error_user, visual_user, performance_glitch_user).
