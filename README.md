# Simple DataFrames in Python (No-Pandas implementation)


Projekt ten stanowi implementację podstawowych struktur i operacji na danych (tzw. ramkach danych) przy użyciu czystego Pythona. Został przygotowany jako rozwiązanie zadania laboratoryjnego skupionego na operacjach macierzowych i algorytmach grupowania danych.

📋 Opis projektu

Głównym celem jest operowanie na zbiorze danych (macierzy), w której każda kolumna przechowuje elementy tego samego typu. System przetwarza dane z pliku tips.csv, który zawiera informacje o napiwkach w restauracji, płci klientów oraz ich preferencjach dotyczących palenia.

Projekt realizuje proces Split-Apply-Combine bez wykorzystania zewnętrznych bibliotek, co wymagało ręcznej implementacji logiki grupowania i agregacji.
🛠️ Funkcjonalności

Program oferuje następujące moduły:

    Weryfikacja danych: Funkcja check_validity sprawdza, czy struktura jest spójna (te same rozmiary wierszy) i czy typy danych w kolumnach są jednolite.

Ekstrakcja unikatów: Możliwość pobrania listy unikatowych kategorii z kolumn tekstowych.

Grupowanie (Split): Funkcja group_by dzieli ramkę danych na podzbiory na podstawie wartości w wybranej kolumnie.

Agregacja (Apply/Combine): Funkcja count (policz) pozwala na wykonanie dowolnej funkcji agregującej (np. sum, len lub mean) na zgrupowanych danych.

📊 Przykład danych

Zbiór danych tips.csv składa się z trzech kolumn:

    Napiwek: Wartość float.

Płeć: Wartość tekstowa (str).

Palacz: Wartość tekstowa (str).

🚀 Jak uruchomić?

    Upewnij się, że plik 2021-MAT-11_tips.csv znajduje się w tym samym folderze co skrypt.

    Uruchom program:
    Bash

    python main.py

⚠️ Ograniczenia techniczne

Zgodnie z wymaganiami projektowymi, kod został napisany z zachowaniem specyficznych restrykcji algorytmicznych:

    Brak korzystania z biblioteki Pandas lub NumPy.

    Zakaz używania indeksowania ujemnego oraz wycinania (slice).

Ręczne zarządzanie referencjami list w celu uniknięcia błędów kopiowania obiektów.
