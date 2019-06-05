# Smog-PM10
Analiza i modelowanie smogu PM10 w Polsce.

Analiza wykorzystuje co godzinne pomiary stężenia PM10 na kiludziesięciu stacjach pomiarowych w Polsce zmierzone  od stycznia 2016 do maja 2018. Obserwacje zostały pobrane ze stron EU. 
Zostały one uzupełnione o zmienne meteorologiczne i szereg zmiennych o charakterze przestrzennym. Do analizy wykorzystano metody data science.

W przedstawionym notebooku wykorzystano zmodyfikowane dane - średnie dobowe. Wykonano podstawowe mapy służące do oceny stopnia zanieczyszcenia, 
mapę średnich rocznych wartości PM10 oraz mapę liczby dni z wartościami powyżej 50 µg/m3 Analizie  poddano różne czynniki. 
Wykazano, że w skali roku podstawowymi czynnikami zmniejszającymi smog są temperatura, pokrycie terenu takie jak woda i zieleń, a także istnienie korytarzy powietrznych. Natomiast czynnikami zwiększającymi smog 
są:wilgotność, liczba samochodów, pokrycie terenu w postaci obszarów zamieszkałych i dróg.
Wykazano, że zarówno skala smogu jak i jego specyfika różnią się bardzo między zimą i latem. W zimie specyfika smogu jest identyczna ze smogiem w skali roku i charkteryzuje się większymi wartościami. Latem 
czynnikami ograniczającymi smog jest wilgotność i wiatr oraz pokrycie terenu (woda i zieleń), natomiast głównymi czynnikami zwiększającymi smog są 
temperatura, samochody i pokrycie terenu (obszary zamieszkane i drogi). Wyznaczono ilościowe miary wagi poszczególnych czynników.

Zbudowany model dla całego roku pozwala na predykcję wartości smogu PM10 korzystając wyłącznie z danych meteorologicznych (wiatru, temperatury i wilgotności), taki 
model tłumaczy 70% zmienności dobowego stężenia PM10  (RMSE: 14.79, R^2 Validation Score: 0.70). Został on wykorzystany do stworzenia modelowanych
rozkładów w 2017 roku i porownania ich z wartościami rzeczywistymi.

