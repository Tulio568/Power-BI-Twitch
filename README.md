# Power-BI-Twitch
Dashboard Power BI analizujący statystyki kanału streamingowego: średnia widownia miesięczna, czas oglądania transmisji na żywo oraz wskaźniki zaangażowania. Dane przetworzone i wyczyszczone w Power Query. Projekt obejmuje pełny pipeline: od surowych danych do gotowych wizualizacji KPI.
# 📊 Analiza statystyk kanału streamingowego — Power BI

## Opis projektu

Samodzielny projekt analityczny polegający na zebraniu, przetworzeniu i wizualizacji danych statystycznych własnego kanału streamingowego. Celem projektu było zbudowanie dashboardu umożliwiającego śledzenie kluczowych wskaźników aktywności kanału w czasie oraz identyfikację trendów oglądalności.

Projekt obejmuje pełny pipeline analityczny: od surowych danych źródłowych, przez czyszczenie i strukturyzację w Power Query, aż do gotowego modelu danych i wizualizacji KPI w Power BI.

---

## 🛠️ Narzędzia i technologie

| Narzędzie | Zastosowanie |
|---|---|
| Microsoft Excel | Przechowywanie i wstępna organizacja danych źródłowych |
| Power Query | Czyszczenie, transformacja i strukturyzacja danych |
| Power BI Desktop | Modelowanie danych, budowa wskaźników KPI, wizualizacje |

---

## 📁 Struktura projektu

```
📂 twitch-analytics-powerbi
 ├── 📄 README.md
 ├── 📊 dashboard.pbix          # Plik Power BI z gotowym dashboardem
 └── 📂 data
      └── 📄 dane_zrodlowe.xlsx  # Przetworzone dane źródłowe
```

---

## 📥 Dane źródłowe

Dane pochodzą ze statystyk własnego kanału streamingowego i obejmują następujące zmienne:

| Kolumna | Opis |
|---|---|
| Miesiąc | Okres rozliczeniowy w formacie RRRR-MM |
| Średnia liczba widzów | Średnia liczba widzów w danym miesiącu |
| Czas oglądania (godz.) | Łączny czas oglądania transmisji przez widzów |
| Liczba transmisji | Liczba przeprowadzonych transmisji na żywo w miesiącu |

---

## 🔄 Proces przetwarzania danych — Power Query

Dane źródłowe wymagały kilku kroków transformacji przed załadowaniem do modelu Power BI:

### Krok 1 - Import danych
Dane zaimportowano z pliku Excel do Power Query jako tabelę strukturalną.

### Krok 2 - Czyszczenie danych
- Usunięcie pustych wierszy i kolumn bez wartości
- Weryfikacja typów danych — konwersja kolumn liczbowych i datowych na właściwe formaty
- Wykrycie i obsługa wartości brakujących (null)

### Krok 3 - Standaryzacja wartości
- Ujednolicenie formatu dat do RRRR-MM
- Zaokrąglenie wartości liczbowych do dwóch miejsc po przecinku
- Weryfikacja spójności jednostek (godziny vs. minuty)

### Krok 4 - Strukturyzacja tabeli
- Nadanie kolumnom jednoznacznych, opisowych nazw
- Sortowanie danych chronologicznie według kolumny miesiąca
- Finalne sprawdzenie kompletności i poprawności zbioru przed załadowaniem

### Krok 5 - Załadowanie do modelu Power BI
Oczyszczona tabela załadowana jako źródło danych do Power BI Desktop.

---

## 📐 Model danych i wskaźniki KPI

W Power BI zbudowano następujące miary analityczne:

| Wskaźnik KPI | Opis |
|---|---|
| Średnia widownia miesięczna | Średnia liczba widzów w wybranym okresie |
| Trend oglądalności | Zmiana średniej widowni miesiąc do miesiąca |
| Łączny czas oglądania | Suma godzin oglądania we wszystkich transmisjach |
| Średni czas oglądania na transmisję | Czas oglądania / liczba transmisji w miesiącu |

---

## 📊 Zawartość dashboardu

Dashboard składa się z następujących elementów wizualnych:

- **Wykres liniowy** — trend średniej widowni w poszczególnych miesiącach
- **Wykres słupkowy** — porównanie czasu oglądania według miesięcy
- **Karty KPI** — aktualne wartości kluczowych wskaźników
- **Filtry czasowe** — możliwość zawężenia analizy do wybranego okresu

---

## 🔗 Link do projektu

Plik dashboardu dostępny na Dysku Google:
[Zobacz dashboard Power BI](https://drive.google.com/file/d/1UqtMTe8eCL30rSoaXjZ3IIDxF86LBejM/view?usp=sharing)

---

## 👤 Autor

**Marcin Pruski**
Projekt portfolio — samodzielne zastosowanie Power BI i Power Query w analizie danych.
