![SamsungGalaxyA21](zadanie2.PNG)

| Plik | Za co odpowiada | Odpowiednik w Django |
| :--- | :--- | :--- |
| `MainActivity` | Zawiera kod sterujący zachowaniem głównego ekranu, ładowaniem widoku oraz reakcją na działania użytkownika. | `views.py` |
| `activity_main.xml` | Definiuje strukturę wizualną ekranu – rozmieszczenie i wygląd poszczególnych elementów interfejsu. | `templates/index.html` |
| `AndroidManifest.xml` | Główny plik konfiguracyjny aplikacji. Określa jej nazwę, ikonę, wymagane uprawnienia oraz ekran uruchamiany jako pierwszy. | `settings.py` oraz `urls.py` |
| `strings.xml` | Przechowuje wszystkie napisy i komunikaty wyświetlane w aplikacji, co ułatwia zarządzanie tekstem i tłumaczeniami. | Pliki tłumaczeń (`.po`) lub stałe tekstowe |
| `app/build.gradle.kts` | Konfiguracja konkretnego modułu aplikacji, w tym lista zewnętrznych bibliotek, wersja programu oraz docelowe wersje systemu Android. | `requirements.txt` |
| `colors.xml` | Zbiór zdefiniowanych kolorów używanych w różnych miejscach interfejsu aplikacji. | Zmienne w plikach `static/` (CSS) |
| `libs.versions.toml` | Centralny rejestr przechowujący numery wersji wszystkich bibliotek i wtyczek używanych w projekcie. | `requirements.txt` / `pyproject.toml` |

![Za awarię (`NullPointerException`) odpowiada linia `buttonStart.setOnClickListener(...)` w metodzie `onCreate` w pliku `MainActivity.java`, ponieważ metoda `findViewById` została wywołana przed `setContentView` i zwróciła wartość `null`.](Zadanie_6_i_7.PNG)


Zadanie 8: Licznik zmniejsza się z obrotem ekranu oraz chce on zająć cały ekran, zmniejsza się ponieważ jak wspomniałem musi zająć ekran