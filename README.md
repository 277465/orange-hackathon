# orange-hackathon
---

### **Etap 1: Przygotowanie środowiska i repozytorium (Dzień 1)**

#### 1.1. **Załóż repozytorium Git**
- Utwórz repozytorium na GitHubie (lub GitLabie).
- Stwórz odpowiednią strukturę folderów:
  - `frontend/` – dla aplikacji frontendowej.
  - `backend/` – dla aplikacji backendowej.
  - `docs/` – dla dokumentacji.
  - `tests/` – dla testów.

#### 1.2. **Zainstalowanie narzędzi**
- **Frontend**:
  - Jeśli robisz aplikację webową, zainstaluj React lub Vue.js.
  - Jeśli aplikacja mobilna, zainstaluj Flutter lub React Native.
- **Backend**:
  - Zainstaluj Node.js z Express, Python z Flask/Django (w zależności od preferencji).
- **Baza danych**:
  - Jeśli chcesz używać MySQL, PostgreSQL lub Firebase, skonfiguruj odpowiednią bazę danych.
- **API**:
  - Zainstaluj paczki do komunikacji z Camara API i Nokia NaC (np. `axios` w Node.js lub `requests` w Pythonie).

#### 1.3. **Podział zadań**
- **Osoba 1**: Backend, integracja API.
- **Osoba 2**: Frontend, UI/UX.
- **Osoba 3**: Testowanie, dokumentacja, debugowanie.

---

### **Etap 2: Projektowanie aplikacji (Dzień 2)**

#### 2.1. **Określenie funkcji aplikacji**
- **SIM Swap API**: Detekcja zmiany SIM.
- **Quality on Demand (QoD)**: Optymalizacja jakości połączenia (zwiększanie przepustowości, zmniejszanie opóźnień).
- **Location API**: Wykrywanie lokalizacji urządzenia.

#### 2.2. **Tworzenie UI/UX**
- **Osoba 2**: Zaczyna szkicowanie UI.
  - Ekran logowania.
  - Ekran główny z informacjami o SIM swap, jakości połączenia, lokalizacji.
  - Panel ustawień (powiadomienia, ustawienia lokalizacji, itd.).

#### 2.3. **Wybór technologii**
- **Frontend**: React, Vue.js (web) lub React Native, Flutter (mobile).
- **Backend**: Node.js z Express, Python z Flask.
- **Baza danych**: MySQL lub Firebase.

---

### **Etap 3: Integracja API (Dzień 3-7)**

#### 3.1. **Osoba 1 (Backend – API Integracja)**
- **SIM Swap API**:
  - Zintegruj Camara lub Nokia NaC API do wykrywania zmiany SIM.
  - Wykonaj zapytanie do API, aby wykryć, czy SIM zostało zmienione.
  - Użyj odpowiednich endpointów, np. `SimSwap API` z Camara.
- **QoD API**:
  - Zintegruj API do optymalizacji jakości połączenia.
  - Użyj endpointu `Quality on Demand` z Camara lub Nokia.
- **Location API**:
  - Zintegruj API do uzyskiwania lokalizacji urządzenia.
  - Użyj endpointu `Location API` z Camara lub Nokia.

#### 3.2. **Osoba 2 (Frontend – UI/UX)**
- Zbuduj UI do wyświetlania wyników:
  - Ekran główny: Informacje o SIM swap, QoD i lokalizacji.
  - Ekran szczegółów: Możliwość monitorowania jakości połączenia, historii SIM swap, lokalizacji.
  
#### 3.3. **Osoba 3 (Testowanie – Weryfikacja API)**
- Testuj integracje API (SIM swap, QoD, Location).
- Sprawdź, czy aplikacja poprawnie komunikuje się z API, czy dane są zwracane poprawnie.

---

### **Etap 4: Backend i logika aplikacji (Dzień 8-12)**

#### 4.1. **Osoba 1 (Backend – Rozwój logiki)**
- **Backend**: Tworzenie systemu backendowego do przetwarzania danych, np. przechowywanie historii SIM swap, historii lokalizacji.
  - Stwórz odpowiednie modele danych w bazie danych.
  - Implementuj endpointy API do zapisywania i pobierania danych o SIM swap, jakości połączenia i lokalizacji.
- **Uwierzytelnianie**: Zaimplementuj mechanizm logowania i rejestracji użytkownika (np. JWT – JSON Web Tokens).

#### 4.2. **Osoba 2 (Frontend – Integracja z Backendem)**
- Połącz frontend z backendem.
  - Zaimplementuj logikę frontendową do obsługi danych zwróconych przez backend (SIM swap, QoD, Location).
  - Twórz interaktywne komponenty do wyświetlania wyników w czasie rzeczywistym.
- Dostosuj frontend, aby wyświetlał aktualne dane (np. wykrywanie zmiany SIM, monitorowanie jakości połączenia).

#### 4.3. **Osoba 3 (Testowanie – Testy API)**
- Testuj backend i integrację z frontendem.
  - Upewnij się, że dane są poprawnie przekazywane między frontendem a backendem.
  - Testuj różne scenariusze (np. zmiana SIM, różne warunki jakości połączenia, błędna lokalizacja).

---

### **Etap 5: Testowanie i debugowanie (Dzień 13-15)**

#### 5.1. **Osoba 3 (Testowanie Aplikacji)**
- Testowanie aplikacji na różnych urządzeniach (desktop, mobile).
- Sprawdzanie, czy API działa poprawnie w różnych scenariuszach:
  - Zmiana SIM: Czy aplikacja wykrywa zmianę SIM.
  - QoD: Czy aplikacja optymalizuje połączenie w zależności od warunków.
  - Location: Czy aplikacja prawidłowo identyfikuje lokalizację urządzenia.
- Testowanie bezpieczeństwa i wydajności aplikacji.

#### 5.2. **Osoba 1 i Osoba 2 (Debugowanie i Poprawki)**
- Usuwanie znalezionych błędów i problemów.
- Optymalizacja kodu (np. przyspieszenie zapytań do API, poprawa wydajności frontendowej).

---

### **Etap 6: Finalizacja i Prezentacja (Dzień 16-17)**

#### 6.1. **Osoba 1 (Dokumentacja techniczna)**
- Przygotowanie dokumentacji API:
  - Jak działa SIM swap, QoD, Location API.
  - Jak działa backend i jakie dane są przechowywane w bazie danych.
  - Jak działa mechanizm logowania i uwierzytelniania użytkownika.

#### 6.2. **Osoba 2 (Prezentacja aplikacji)**
- Przygotowanie prezentacji aplikacji na hackathon:
  - Omówienie kluczowych funkcji aplikacji.
  - Demonstracja działania aplikacji (SIM swap, QoD, lokalizacja).

#### 6.3. **Osoba 3 (Testowanie przed prezentacją)**
- Ostateczne testy aplikacji, upewnienie się, że wszystkie funkcje działają płynnie.
- Przygotowanie prezentacji demo aplikacji.

---
