Wersja 7.02

[https://github.com/hamhobbypl/morsebox/blob/main/firmware_7_02.bin](https://github.com/hamhobbypl/morsebox/blob/main/Firmware/firmware_7_02.bin)

Zmiany:
1. Poprawiony błąd w logice ustawiania BW.
2. Oznaczane są ćwiczenia copy i wyłączana przerwa po ostatnim znaku niezależnie od FW i BW. Nie ma zjawiska blokowania.
3. Dodano możliwość przełączenia na białe fonty w ćwiczeniach jest bardziej kontrastowo i czytelniej dla niektórych.
4. Skopiowano logikę ładowania karty z Config/Files na taką samą do Receive/SD Card.
5. Dodałem LOG dla KEYER.

a) żeby uruchomić loga pobieramy w SETUP czas z serwera NTP "Time". Wcześniej musiy mieć skonfigurowane WIFI w SETUP/WIFI.
b) w Logger dajemy ON. (musimy mieć na karcie SD katalog "logs", bo tam zbierane są logi).  Jeśli wszystko pójdzie OK -  utworzy się plik zgodny z bieżącym czasem i pokaże się jego nazwa.

c) wchodzimy do KEYER i jeśli jest logowanie to w belce mamy czerwony napis LOG.

d) warunki zapisu:

w keyer jeśli coś nadaliśmy i nie nadajemy przez 5s następuje zapis
jeśli wychodzimy z keyera również zapisuje to co nadaliśmy od ostatniego zapisu
w makro zapisuje po skończonym makro lub po wyjściu w trakcie.

e) podgląd loga - kursor na KEYER i long press >=1s
widzimy od końca loga i możemy przewijać ostatnie 256 linii.
loga możemy weryfikować w dowolnej chwili.

f) jeśli chcemy nowy plik loga w danej sesji wchodzimy w setup i dajemy Logger OFF i potem znowu ON. Utworzy się nowy plik. 


*******************************************************

Wersja 7.01

[https://github.com/hamhobbypl/morsebox/blob/main/firmware_7_01.bin](https://github.com/hamhobbypl/morsebox/blob/main/Firmware/firmware_7_01.bin)

Zmiany:
1. Możliwość wyboru odstępu w odbiorze pomiędzy znakami i słowami w trybie FARNSWORTH i BEATSWORTH(z zachowaniem rytmu kodu morsa).
2. Powitalne R nie jest wysyłane na KEYER.
3. Znak ~ użyty w makro keyera naciska klucz i trzyma, aż do naciśnięcia gałki enkodera. Jest to pomoc w strojeniu dla TRX nie posiadających funkcji TUNE.
Możemy sobie utworzyć np. ~TUNE i mamy dodatkową funkcję zapisaną jako macro KEYERA.


*******************************************************

Wersja 7.0

[https://github.com/hamhobbypl/morsebox/blob/main/firmware_7_0.bin](https://github.com/hamhobbypl/morsebox/blob/main/Firmware/firmware_7_0.bin)

Zmiany:
1. Przebudowa głównego MENU. Poruszanie się pomiędzy modułami nie wymaga restartu urządzenia.
2. Dodana aktywna ikona karty SD pokazująca status i dająca możliwość reload karty oraz sprawdzenia listy plików.
3. Usunięte wsparcie dla METABASE!!!
4. Zmiana w logice ustawianie prędkości WPM i FWPM w keyer. Teraz po długim naciśnięciu enkodera.
5. Zwiększona ilość MAKR w keyerze do 32 i dodane przewijanie.
6. Sieć wifi na podstawie pliku ustawia się w SETUP/WIFI i ona zostaje zapamiętana jeśli uda się połączyć. Jeśli trzeba zmienić znowu należy użyć SETUP/WIFI.
7. Dodano ćwczenie Receive/DitIfRec - analogia Morse Machine, ale po rozpoznaniu litery/cyfry naciskamy DIT zamiast kopiowania znaku.
8. Zmiana logiki ustawiania CALLSIGN, pojawia się też w Menu Głównym.
9. Nie rozpoznaje czy jest HW Keyer, wszystkim odpalą się wszystkie moduły nawet jeśli nie mają sprzętowo keyera.
10. Zwiększony limit plików do 50.
11. Inne kosmetyczne zmiany w UI.

*******************************************************

Wersja 6.09

[https://github.com/hamhobbypl/morsebox/blob/main/firmware_6_09.bin](https://github.com/hamhobbypl/morsebox/blob/main/Firmware/firmware_6_09.bin)

Zmiany:

1. Dodano możliwość przestawiania time out w ćwiczeniu Receive/Flashcrd - inspiracja Ryszard M0RPA.
2. Dodano ćwiczenie Morse Machine Send/MorseMach inspirowane lcwo.net. Po uzyskanym wyniku można utworzyć sobie po analizie plik na kartę SD ze słabymi punktami i ćwiczyć np. w Head Copy.
3. Usunięty BUG lagów enkodera w KEYER przy zmianie WPM.

*******************************************************

Wersja 6.08

[https://github.com/hamhobbypl/morsebox/blob/main/firmware_6_08.bin](https://github.com/hamhobbypl/morsebox/blob/main/Firmware/firmware_6_08.bin)


Zmiany:

1. Konfiguracja "Speed" równolegle w Tutor
2. Możliwość wyłączenia dźwięków wyniku próby w ćwiczeniach i testach "MH Sound" w menu config Tutora. 
3. Dodano ćwiczenie w którym należy liczyć ilość słów i weryfikować swoją skuteczność niekoniecznie rozumiejąc treść słów.
(Receive/CountWrd) inspiracja Ryszard M0RPA
4. Usunięty BUG nieprawidłowych spacji w Chat.



*******************************************************
Wersja 6.07

https://github.com/hamhobbypl/morsebox/blob/main/firmware_6_07.bin


Zmiany:

1. Sortowanie wyświetlania plików z karty SD


*******************************************************


Wersja 6.06


https://github.com/hamhobbypl/morsebox/blob/main/firmware_6_06.bin

Zmiany:

1. Dodano Czat umożliwiający komunikację pomiędzy urządzeniami z opgrogramowaniem MorseBOX - film z działania czat - https://youtu.be/DHyJ-UOmI7o?si=OxFVMdOVVQe5Ljb5

2. Opcje ustawień urządzenia przeniesione do głównego MENU "SETUP" w części TUTOR pozostały tylko te dotyczące TUTORA.

3. W opcjach ustawień klucza pojawiła się możliwość korzystania z trybu Ultimatic Mode.

4. W opcjach speed można zwiększyć odstęp pomiędzy nadawanymi znakami 100-500%. 

*******************************************************

Film z wersji 5 omawiający pozostałe funkcje: https://youtu.be/SKYY0fMZa9M?si=7nfEo5wuas7iSE_V




Moduł TUTOR bazuje na kodzie Copyright (c) 2020, Bruce E. Hall W8BH udostępnionym na zasadzie Open Source MIT License.
