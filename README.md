# orange-hackathon
Oto szczegółowy plan krok po kroku, jak stworzyć aplikację **SmartSecure**, używając Camara API i Nokia Network as Code (NaC), wraz z podziałem na zadania dla trzech osób w zespole:

### **Krok 1: Przygotowanie projektu i środowiska (Dzień 1)**
1. **Założenie repozytorium Git**:
   - Utwórz repozytorium na GitHubie lub innym systemie kontroli wersji (np. GitLab).
   - Ustal strukturę folderów (frontend, backend, dokumentacja, testy).

2. **Zainstalowanie narzędzi i bibliotek**:
   - **Frontend**: Wybierz framework (np. React, Angular, Vue.js) do aplikacji webowej lub Flutter/React Native do aplikacji mobilnej.
   - **Backend**: Wybierz język programowania i framework (np. Node.js, Python + Flask/Django).
   - **Baza danych**: Zainstaluj bazę danych (np. MySQL, PostgreSQL lub Firebase).
   - **API**: Zainstaluj pakiety do komunikacji z Camara API i Nokia NaC (np. axios, fetch w JavaScript).

3. **Podział ról**:
   - **Osoba 1**: Backend i integracja z API.
   - **Osoba 2**: Frontend i UI/UX.
   - **Osoba 3**: Testowanie API, dokumentacja, debugowanie.

---

### **Krok 2: Projektowanie i planowanie (Dzień 1-2)**
1. **Określenie funkcji aplikacji**:
   - **SIM Swap**: Wykrywanie zmiany karty SIM (wykorzystaj API Camara lub Nokia).
   - **Quality on Demand (QoD)**: Optymalizacja jakości połączenia (np. zwiększenie przepustowości, niższe opóźnienia).
   - **Location API**: Sprawdzanie i wyświetlanie geolokalizacji urządzenia.
   - **Bezpieczeństwo**: Uwierzytelnianie i zabezpieczenia danych użytkowników.

2. **Projekt UI/UX**:
   - **Osoba 2**: Zaczyna szkicowanie prostego UI (np. ekrany logowania, monitorowania SIM swap, jakości połączenia, lokalizacji).
   - Ustal typy ekranów: główny, ustawienia, szczegóły (SIM swap, QoD, Location).

3. **Wybór technologii**:
   - **Frontend**: React (dla aplikacji webowej) lub React Native/Flutter (dla aplikacji mobilnej).
   - **Backend**: Node.js + Express lub Python (Flask/Django).
   - **Baza danych**: MySQL, PostgreSQL lub Firebase.

---

### **Krok 3: Integracja API (Dzień 3-7)**
1. **Osoba 1** – **Backend i integracja API**:
   - **SIM Swap API**:
     - Zintegruj API SIM Swap z Camara lub Nokia NaC. API powinno wykrywać, kiedy SIM jest zmieniany i przekazywać tę informację do aplikacji.
     - Sprawdź, jak poprawnie przesyłać zapytania API i odbierać odpowiedzi (JSON).
   - **QoD API**:
     - Zintegruj API QoD, które pozwala na optymalizację połączenia sieciowego (np. zmiana jakości w zależności od potrzeby aplikacji).
   - **Location API**:
     - Zintegruj API lokalizacji, aby uzyskać dane o geografii urządzenia.

2. **Osoba 2** – **Frontend**:
   - **Projektowanie UI**:
     - Stwórz widok ekranu głównego, gdzie użytkownik może sprawdzić informacje o stanie SIM (czy zmieniono), jakość połączenia i lokalizację.
     - Dostosuj UI do różnych urządzeń (mobile, desktop).

---

### **Krok 4: Backend i logika aplikacji (Dzień 8-12)**
1. **Osoba 1** – **Backend**:
   - **Logika aplikacji**:
     - Twórz backend, który przechowuje dane użytkownika (np. historia SIM swap, dane lokalizacyjne).
     - Implementuj system powiadomień o wykryciu zmiany SIM, optymalizacji QoD oraz lokalizacji.
   - **Baza danych**:
     - Utwórz bazę danych, która przechowuje dane użytkowników (np. identyfikator SIM, wyniki QoD, historia lokalizacji).

2. **Osoba 2** – **Frontend**:
   - Połącz frontend z backendem.
   - Wyświetlaj dane na ekranie głównym (SIM swap status, QoD, location).
   - Stwórz interfejs do konfiguracji ustawień, np. włączenie powiadomień, ustawienia lokalizacji.

3. **Osoba 3** – **Testowanie API i aplikacji**:
   - Testuj API, aby upewnić się, że wszystkie funkcje działają poprawnie (SIM swap, QoD, Location).
   - Testuj różne przypadki: zmiana SIM, zmiana jakości połączenia, aktualizacja lokalizacji.

---

### **Krok 5: Testowanie i debugowanie (Dzień 13-15)**
1. **Osoba 3** – **Testowanie aplikacji**:
   - Testowanie wszystkich funkcji:
     - **SIM Swap**: Sprawdź, czy wykrywanie zmiany SIM działa poprawnie.
     - **QoD**: Testuj optymalizację jakości połączenia.
     - **Location**: Testuj dokładność i aktualność lokalizacji urządzenia.
   - **Debugowanie**: Sprawdzaj błędy w aplikacji, testuj pod kątem wydajności.

2. **Osoba 1 i 2** – **Optymalizacja i poprawki**:
   - Ulepsz UI/UX na podstawie testów.
   - Popraw wszelkie problemy związane z backendem.

---

### **Krok 6: Finalizacja i prezentacja (Dzień 16-17)**
1. **Osoba 1** – **Dokumentacja techniczna**:
   - Stwórz dokumentację API (jak działa SIM swap, QoD, Location).
   - Dodaj opis backendu, jak działa logika aplikacji, jak są przechowywane dane.

2. **Osoba 2** – **Prezentacja aplikacji**:
   - Przygotuj prezentację aplikacji, podkreślając najważniejsze funkcje: bezpieczeństwo SIM swap, optymalizacja QoD i lokalizacja.
   - Upewnij się, że aplikacja jest gotowa do prezentacji (sprawdzając UI i płynność działania).

3. **Osoba 3** – **Przygotowanie testów końcowych**:
   - Ostateczne testy aplikacji i przygotowanie do demo.

---

### **Szacowany czas realizacji**: **15-17 dni** (zespół 3-osobowy)

Po tym czasie aplikacja powinna być gotowa, a Ty będziesz gotowy do zaprezentowania jej na hackathonie. Potrzebujesz dalszej pomocy przy kodowaniu lub jakiejś części aplikacji?
