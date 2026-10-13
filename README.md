# Moonbase Control: Output (custom events)

Zadanie z modułu Angular. Repozytorium zawiera kod startowy aplikacji Moonbase Control dla tej lekcji.

## Zadanie

Spraw, aby każda karta statusowa informowała `DashboardComponent`, kiedy zostanie wybrana.

### 1. Rozszerz model karty statusowej
Utwórz typ `StatusCardId`, który będzie zawierał identyfikatory wszystkich czterech kart.

Rozszerz interfejs `StatusCard` o `id`.

Dodaj unikalne `id` do każdej zamockowanej karty w `DashboardComponent`.

### 2. Przekaż identyfikator karty do `CardComponent`
W `CardComponent` utwórz wymagany input signal o nazwie `cardId`.

Przekaż odpowiedni identyfikator do każdej instancji karty za pomocą property bindingu.

### 3. Stwórz output()
W `CardComponent` utwórz output o nazwie `selected`.

Dodaj metodę, która emituje identyfikator aktualnej karty.

### 4. Wyemituj event po kliknięciu karty
Spraw, aby karta była interaktywna, używając przycisku `<button>`.

💡 Karta powinna jedynie poinformować, że została wybrana.

### 5. Obsłuż event w `DashboardComponent`
Utwórz sygnał przechowujący identyfikator wybranej karty.

Utwórz metodę, która aktualizuje ten signal.

Upewnij się że dodałeś odpowiedni binding w każdej instancji `app-card`

💡 `$event` zawiera wartość wyemitowaną przez `CardComponent`.

### 6. Wyświetl aktualnie wybraną kartę
Dodaj sekcję z akcjami poniżej kart.

Zanim użytkownik wybierze kartę, wyświetl tekst: “Select a status card to see available action”

Po wybraniu karty wyświetl jej identyfikator lub tytuł w sekcji akcji.

## Jak zacząć

1. Zrób fork tego repozytorium na swoje konto GitHub.
2. Sklonuj swój fork na komputer.
3. Zainstaluj zależności: `npm install`.
4. Uruchom aplikację: `npm start`.
5. Jeśli zadanie korzysta z danych z API, uruchom w drugim terminalu mock API: `npm run api`.

## Jak oddać zadanie

1. Zapisz zmiany w commicie i wypchnij je do swojego forka.
2. Otwórz Pull Request z forka do repozytorium `mate-academy/angular_outputs`, do brancha `main`.
3. Platforma uruchomi review Twojego Pull Requesta.
