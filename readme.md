Znajduje się tutaj program jako rozwinięcie aplikacji do znajdowanie znajomych na kursie na platformę Streamlit Community Cloud z modułu 7-zad1
=======
# Zmiany w stosunku do wersji v3:
## dodanie funkcji wyboru arkusza danych csv 
## Dodanie funkcji odpowiedzialnych za stworzenie nowego modelu treningowego dostosowanej do stremlit  
wybór nazwy pliku modelu treningowego  
wybór ilości klastrów w modelu treningowym
## dodanie funkcji odpowiedzialnej za przygotowanie opisów grup w modelu treningowym dostosowanej do streamlit  
wybór nazwy pliku opisów modelu treningowego  
możliwość dodania klucza api open ai w przypadku braku pliku env  
## dodanie menu wyboru powyższych funkcji i obsługa ewentualnych wyjątków

## Instalacja i uruchomienie

za pomocą dockera: docker build -t znajdowanie_znajomych .

manualna: Aby zainstalować aplikację bez dockera należy uruchomić konsolę (w przypadku windowsa cmd, linuxa bash) i wpisać: pip install --upgrade pip pip install -r requirements.txt



Aby zainstalować aplikację, uruchom konsolę (CMD w Windows, Terminal w Linux/macOS) i postępuj zgodnie z wybraną metodą:

Krok 1: Pobranie projektu na dysk

Wybierz jedną z opcji:
   ```bash
   git clone https://github.com/ryszarddddl/ankieta_znajdowanie_znajomych
   ```
   ```
   wget https://github.com/ryszarddddl/ankieta_znajdowanie_znajomych
   ```
   
   Kliknij zielony przycisk "Code" na górze strony i wybierz "Download ZIP" lub "Open with GitHub Desktop".
   
Krok 2: Instalacja i start
Opcja A: Docker (Zalecane)

Zainstaluj Docker Desktop: https://docs.docker.com/desktop/
W konsoli przejdź do folderu projektu: cd Estymator_Czasu_Pol_maratonu
Zbuduj obraz: 
```
docker build -t znajdowanie_znajomych .
```
Uruchomienie:
   Otwórz Docker Desktop, wejdź w zakładkę Images i kliknij Run przy znajdowanie_znajomych.
   W ustawieniach (Optional settings) wpisz port (np. 8501).
   Adres do aplikacji znajdziesz w zakładce Containers. W razie problemów zapytaj Gordona (AI wbudowane w Docker Desktop).

Opcja B: Instalacja manualna

Pobierz Pythona (zalecana wersja 3.11): https://www.python.org/downloads/
W konsoli zainstaluj wymagane biblioteki:
   ```
   pip install --upgrade pip
   pip install -r requirements.txt
   ```
      
Używaj kodu z rozwagą.
Uruchomienie: Wpisz w konsoli: 
   ```
   streamlit run src/aplikacja.py
   ```  



