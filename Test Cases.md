#  Test Cases - SauceDemo

Projekt przedstawia przykładową specyfikację testów manualnych przygotowaną dla aplikacji **SauceDemo**.

## Spis treści
- Logowanie
- Koszyk
- Sortowanie produktów
- Checkout

##  Informacje

- **Projekt:** SauceDemo
- **Narzędzie:** TestLink
- **Rodzaj testów:** Manual Testing

---

#  Test Suite: Checkout

**Test Case:** TC-7 – Checkout

**Autor:** kapucyn

| Krok | Akcja | Oczekiwany rezultat |
|------|--------|---------------------|
| 1 | Płatność bez wpisania danych | Wyświetla się komunikat **"Error: First Name is required"** |
| 2 | Płatność bez wpisania imienia | Wyświetla się komunikat **"Error: First Name is required"** |
| 3 | Płatność bez wpisania nazwiska | Wyświetla się komunikat **"Error: Last Name is required"** |
| 4 | Płatność bez wpisania ZIP/Postal Code | Wyświetla się komunikat **"Error: Postal Code is required"** |
| 5 | Wpisanie wszystkich danych i kliknięcie **Continue** | Użytkownik zostaje przekierowany na stronę podsumowania zamówienia |
| 6 | Kliknięcie **Finish** | Wyświetla się komunikat potwierdzający poprawne złożenie zamówienia |

### Informacje

| Pole | Wartość |
|------|---------|
| Execution Type | Manual |
| Estimated Duration | 5 min |
| Importance | High |

---

#  Test Suite: Koszyk

**Test Case:** TC-5 – Koszyk

**Autor:** kapucyn

### Preconditions

- Użytkownik znajduje się na stronie **Inventory**

| Krok | Akcja | Oczekiwany rezultat |
|------|--------|---------------------|
| 1 | Wyświetlenie listy produktów | Lista produktów jest poprawnie wyświetlona |
| 2 | Dodanie produktu do koszyka | Liczba produktów w koszyku zwiększa się o 1 |
| 3 | Usunięcie produktu z koszyka | Produkt zostaje usunięty z koszyka |
| 4 | Przejście do koszyka | Wyświetla się lista produktów znajdujących się w koszyku |

### Informacje

| Pole | Wartość |
|------|---------|
| Execution Type | Manual |
| Estimated Duration | 3 min |
| Importance | High |

---

#  Test Suite: Logowanie

**Test Case:** TC-4 – Weryfikacja logiki logowania

**Autor:** kapucyn

### Preconditions

Dostępne konta testowe:

- `standard_user`
- `locked_out_user`

| Krok | Akcja | Oczekiwany rezultat |
|------|--------|---------------------|
| 1 | Logowanie bez wpisania danych | Wyświetla się komunikat o błędnych danych logowania |
| 2 | Logowanie bez wpisania hasła | Wyświetla się komunikat **"Password is required"** |
| 3 | Logowanie bez wpisania loginu | Wyświetla się komunikat **"Username is required"** |
| 4 | Logowanie poprawnymi danymi | Użytkownik zostaje przekierowany do listy produktów |
| 5 | Logowanie jako zablokowany użytkownik | Wyświetla się komunikat **"Sorry, this user has been locked out."** |

### Informacje

| Pole | Wartość |
|------|---------|
| Execution Type | Manual |
| Estimated Duration | 4 min |
| Importance | High |

---

#  Test Suite: Sortowanie produktów

**Test Case:** TC-6 – Sortowanie produktów

**Autor:** kapucyn

| Krok | Akcja | Oczekiwany rezultat |
|------|--------|---------------------|
| 1 | Ustawienie sortowania od A do Z | Produkty wyświetlane są w kolejności alfabetycznej A–Z |
| 2 | Ustawienie sortowania od Z do A | Produkty wyświetlane są w kolejności alfabetycznej Z–A |
| 3 | Ustawienie sortowania według rosnącej ceny | Produkty wyświetlane są od najtańszych do najdroższych |
| 4 | Ustawienie sortowania według malejącej ceny | Produkty wyświetlane są od najdroższych do najtańszych |

### Informacje

| Pole | Wartość |
|------|---------|
| Execution Type | Manual |
| Estimated Duration | 3 min |
| Importance | Medium |

---

#  Podsumowanie

Projekt obejmuje testy najważniejszych funkcjonalności aplikacji **SauceDemo**:

- ✅ Logowanie
- ✅ Zarządzanie koszykiem
- ✅ Sortowanie produktów
- ✅ Proces Checkout

Całość została przygotowana w narzędziu **TestLink** jako przykład dokumentacji testowej do portfolio Junior Manual Testera.
