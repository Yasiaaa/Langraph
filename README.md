# 🤖 Landgraph – Projekt agentów AI

Projekt **Landgraph** zawiera rozwiązania oparte na agentach AI, stworzone w ramach nauki i rozwoju systemu.

---

## 📁 Struktura projektu

```
landgraph/
├── .env                  # Plik konfiguracyjny (tworzysz lokalnie)
├── tutorial/             # Materiały szkoleniowe i przykłady
├── bot1_chat/            # Chat Bot
├── bot2_image_to_recipe/ # Konwersja obrazu w przepis
├── bot3_recipe_to_pdf/   # Konwersja przepisu do PDF
├── bot4_image_gen/       # Generator obrazów
└── bot5_combined/        # Bot połączony (Bot 2 + Bot 3)
```

---

## 📚 Folder `tutorial`

Folder `tutorial` zawiera projekty i przykłady stworzone podczas kursów oraz praktyki w budowaniu agentów.

Znajdują się tam:

- testowe implementacje
- eksperymentalne konfiguracje
- przykłady działania agentów
- ćwiczenia praktyczne

Jest to część szkoleniowa projektu wykorzystywana do testów i rozwoju funkcjonalności.

---

## ⚙️ Konfiguracja środowiska

Aby projekt działał poprawnie, należy samodzielnie utworzyć plik `.env` i dodać klucz API.

### Tworzenie pliku `.env`

1. Wejdź do głównego folderu projektu (`landgraph`).
2. Utwórz plik o nazwie `.env`.
3. Dodaj w nim swój klucz API w następującym formacie:

```env
OPENAI_API_KEY=twój_token
```

**Przykład:**

```env
OPENAI_API_KEY=sk-xxxxxxxxxxxxxxxx
```

4. Zapisz plik.

> ⚠️ **Uwaga:** Plik `.env` nie powinien być publikowany w repozytorium, ponieważ zawiera poufne dane. Upewnij się, że jest dodany do `.gitignore`.

---

## 🤖 Boty

Projekt zawiera pięć botów, z których każdy realizuje inną funkcjonalność.

---

### Bot 1 – Chat Bot 💬

Bot umożliwia standardową komunikację z użytkownikiem.

- Prowadzenie rozmowy i zadawanie pytań
- Nie jest bezpośrednio powiązany z przetwarzaniem obrazów ani generowaniem przepisów

---

### Bot 2 – Konwersja obrazu w przepis 🖼️➡️🍽️

Bot automatyzuje proces tworzenia przepisów z fotografii.

- Przyjmuje obraz jako wejście
- Analizuje jego zawartość
- Generuje strukturalny przepis na podstawie obrazu

---

### Bot 3 – Konwersja przepisu do PDF 📄

Bot umożliwia wygodne przechowywanie przepisów w formacie dokumentu.

- Przyjmuje gotowy przepis
- Konwertuje go do formatu PDF
- Zapisuje dokument w postaci pliku

---

### Bot 4 – Generator obrazów 🎨

Bot generuje obrazy na podstawie opisu tekstowego.

- Tworzy grafiki zgodnie z zapytaniem użytkownika
- Nie jest ograniczony wyłącznie do tematyki przepisów

---

### Bot 5 – Bot połączony (Bot 2 + Bot 3) 🔗

Najbardziej zautomatyzowana wersja systemu przetwarzania przepisów, łącząca funkcjonalność botów 2 i 3.

- Przekształca obraz w przepis
- Generuje przepis
- Zapisuje dane w formacie JSON
- Umożliwia rozmowę wyłącznie o przepisach

---

## 📄 Licencja

Projekt stworzony w celach edukacyjnych i rozwojowych.
