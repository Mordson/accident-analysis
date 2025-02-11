# Projekt Analizy Wypadków Drogowych

## Struktura projektu

### Pliki projektu
- `Projekt.ipynb`: Główny notebook zawierający cały proces analizy danych, od wczytywania danych, przez czyszczenie, analizę, modelowanie, aż po wizualizację wyników.
- `app.py`: Skrypt Streamlit tworzący interaktywny dashboard do wizualizacji danych o wypadkach.
- `Dane/caracteristics.csv`: Plik CSV zawierający dane o charakterystyce wypadków.
- `Dane/vehicles.csv`: Plik CSV zawierający dane o pojazdach uczestniczących w wypadkach.
- `Dane/places.csv`: Plik CSV zawierający dane o miejscach wypadków.
- `Dane/users.csv`: Plik CSV zawierający dane o osobach uczestniczących w wypadkach.

### Etapy projektu
- **Wczytywanie danych**: Sekcja wczytująca dane z plików CSV do DataFrame'ów.
- **Wyświetlanie danych**: Sekcja wyświetlająca podstawowe informacje o danych, takie jak pierwsze wiersze i typy danych.
- **Przygotowanie danych do analizy**: Sekcja zawierająca kroki przetwarzania danych, takie jak zmiana nazw kolumn, formatowanie dat, usuwanie zbędnych kolumn i dodawanie nowych kolumn opisowych.
- **Tworzenie wykresów**: Sekcja zawierająca kod do tworzenia różnych wykresów wizualizujących dane, takich jak liczba wypadków w zależności od daty, godziny, miesiąca, miejsca itp.
- **Tworzenie modelu / modelów**: Sekcja zawierająca kod do tworzenia i trenowania modelu regresji logistycznej, w tym podział danych na zbiory uczący i testowy, standaryzacja danych, wybór najlepszych parametrów modelu za pomocą GridSearchCV oraz walidacja modelu.
- **Dashboard Streamlit**: Skrypt `dashboard.py` tworzący interaktywny dashboard do wizualizacji danych o wypadkach, zawierający różne wykresy i mapy.

## Instrukcja uruchomienia

### Kroki potrzebne do uruchomienia projektu
1. Sklonuj repozytorium projektu na swój lokalny komputer.
2. Upewnij się, że masz zainstalowane wymagane oprogramowanie (patrz poniżej).
3. Otwórz plik `Projekt.ipynb` w Jupyter Notebook lub JupyterLab.
4. Uruchom wszystkie komórki w notebooku, aby przeprowadzić pełną analizę danych.
5. Aby uruchomić dashboard Streamlit, otwórz terminal, przejdź do katalogu z plikiem `app.py` i uruchom polecenie:
   ```
   streamlit run dashboard.py
   ```

### Wymagane oprogramowanie
- Python 3.12.2
- Biblioteki Python:
  - pandas
  - matplotlib
  - seaborn
  - scikit-learn
  - streamlit

Możesz zainstalować wymagane biblioteki za pomocą poniższego polecenia:
```sh
pip install pandas matplotlib seaborn scikit-learn streamlit
```

## Źródło danych
- **Dane użyte w projekcie pochodzą z Kaggle**: https://www.kaggle.com/datasets/ahmedlahlou/accidents-in-france-from-2005-to-2016
