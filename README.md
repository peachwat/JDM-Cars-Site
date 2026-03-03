# Wytwarzanie-aplikacji-internetowych

# JDM Cars Project

Projekt strony internetowej poświęconej kulturze **JDM (Japanese Domestic Market)**, zrealizowany w ramach przedmiotu "Wytwarzanie aplikacji internetowych". Repozytorium zawiera dwie wersje projektu: statyczną oraz dynamiczną z wykorzystaniem bazy danych.

## O Projekcie
Serwis przybliża tematykę japońskich samochodów, ich tuningu oraz specyficznych akcesoriów. Projekt łączy nowoczesne technologie front-endowe z logiką serwerową PHP.

### Główne funkcjonalności:
* **Kompendium wiedzy o JDM**: Szczegółowe opisy marek takich jak Honda, Toyota, Nissan, Mitsubishi czy Subaru.
* **JDM Events Locator**: Interaktywne narzędzie wykorzystujące **Geolocation API** do wyszukiwania zlotów i wydarzeń motoryzacyjnych w okolicy użytkownika.
* **Filtrowanie ofert**: Dynamiczne filtrowanie listy samochodów według ceny za pomocą **jQuery UI Slider**.
* **Interaktywna Galeria**: Wykorzystanie **Owl Carousel 2** do responsywnej prezentacji zdjęć.
* **System użytkowników**: Możliwość rejestracji, logowania oraz bezpiecznego wylogowywania (Projekt 2).
* **Dynamiczne zarządzanie zdjęciami**: Galeria zintegrowana z bazą **MongoDB**, obsługująca przesyłanie i wyświetlanie treści.

## Technologia

### Frontend:
* **HTML5 / CSS3**: Semantyczna struktura i stylowanie (layout responsywny).
* **JavaScript (ES6)**: Logika kliencka i manipulacja DOM.
* **jQuery & jQuery UI**: Obsługa interaktywnych komponentów, takich jak suwaki.
* **Owl Carousel 2**: Biblioteka karuzeli obrazów.

### Backend (Projekt 2):
* **PHP**: Implementacja logiki biznesowej i wzorca **Front Controller**.
* **MongoDB**: NoSQL-owa baza danych do przechowywania danych użytkowników i metadanych zdjęć.
* **Composer**: Zarządzanie zależnościami PHP (np. biblioteka `mongodb/mongodb`).

## Struktura projektu
* **Project 1/**: Wersja statyczna strony (HTML, CSS, JS).
* **Project 2/**: Wersja dynamiczna (aplikacja PHP):
    * `src/web/`: Punkt wejścia aplikacji (`front_controller.php`) oraz zasoby statyczne.
    * `src/views/`: Szablony widoków PHP.
    * `src/business.php`: Logika operacji na danych.
    * `vendor/`: Biblioteki zainstalowane przez Composera.

## Instalacja i uruchomienie

### Projekt 1:
Wystarczy otworzyć plik `Project 1/src/web/index1.html` w przeglądarce.

### Projekt 2:
1.  Wymagane środowisko PHP oraz serwer bazy danych **MongoDB**.
2.  Zainstaluj zależności za pomocą Composera w folderze `Project 2`:
    ```bash
    composer install
    ```
3.  Skonfiguruj serwer WWW tak, aby obsługiwał plik `front_controller.php`.
4.  Aplikacja obsługuje routing przez parametr `action`, np. `?action=signup` dla rejestracji.

---
**Autor:** Evelina Rylova
**Status:** Projekt zaliczeniowy
