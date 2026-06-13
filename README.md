# Rejestrator Audio VOX Pro (Radio Logger)

Prosty i lekki rejestrator dźwięku sterowany głosem (VOX), stworzony z myślą o rejestracji korespondencji radiowej (np. z radiotelefonów Baofeng, skanerów i innych odbiorników) pod systemami Linux (Lubuntu / Ubuntu).

Program automatycznie wykrywa dźwięk przekraczający ustawiony próg, nagrywa transmisję i zapisuje ją w osobnych plikach `.wav` z sygnaturą czasową. Posiada graficzny interfejs (GUI) oparty na Tkinter.

## Główne Funkcje

* **Detekcja VOX:** Automatyczne uruchamianie nagrywania po przekroczeniu progu głośności.
* **Bufor Wsteczny (Pre-buffer):** Program stale pamięta ostatnie kilkaset milisekund dźwięku. Dzięki temu nagranie nie jest ucięte i łapie sam początek transmisji.
* **Regulowany Limit Ciszy:** Możliwość ustawienia, jak długo po zakończeniu mowy program ma jeszcze czekać, zanim zamknie plik.
* **Podgląd Poziomu Dźwięku:** Pasek na żywo pokazujący aktualną głośność sygnału, co ułatwia kalibrację.
* **Wybór Folderu:** Możliwość wskazania dowolnego miejsca zapisu plików audio na dysku.

## Wymagania i Instalacja (Linux / Ubuntu / Lubuntu)

Do poprawnego działania program wymaga Pythona 3 oraz bibliotek do obsługi audio i interfejsu. Otwórz terminal i zainstaluj potrzebne pakiety:

```bash
sudo apt update
sudo apt install python3-pip python3-pyaudio python3-numpy python3-tk
