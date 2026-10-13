# Moonbase Control: Output (custom events)

Zadanie z modułu Angular. Repozytorium zawiera kod startowy aplikacji Moonbase Control dla tej lekcji.

## Zadanie

Spraw, aby każda karta statusowa informowała komponent `Dashboard`, kiedy zostanie wybrana.

W kodzie startowym komponent `Card` otrzymuje cały obiekt karty przez input `card`. Każda karta ma już pole `id`, a jej szablon jest elementem `<button>`.

### 1. Dodaj typ identyfikatora karty
Utwórz typ `StatusCardId`, który zawiera identyfikatory wszystkich czterech kart. Użyj go jako typu pola `id` w interfejsie `StatusCard`.

### 2. Stwórz output()
W komponencie `Card` utwórz output o nazwie `selected`. Dodaj metodę, która emituje `card().id`.

### 3. Wyemituj event po kliknięciu karty
Wywołaj tę metodę po kliknięciu przycisku karty.

💡 Karta powinna jedynie poinformować, że została wybrana.

### 4. Obsłuż event w komponencie `Dashboard`
Utwórz sygnał przechowujący identyfikator wybranej karty. Utwórz metodę, która aktualizuje ten sygnał. Dodaj binding do outputu `selected` w każdej instancji `app-card`.

💡 `$event` zawiera wartość wyemitowaną przez komponent `Card`.

### 5. Wyświetl aktualnie wybraną kartę
Dodaj poniżej kart sekcję z informacją o wybranej karcie. Zanim użytkownik wybierze kartę, wyświetl tekst: "Select a card to see available actions." Po wybraniu karty wyświetl jej identyfikator.

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
