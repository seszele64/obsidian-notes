---  
title: Projekt EDIF  
share: true  
cssclass: full-width  
---  
  
[TOC]  
  
## Opis  
>Zbadać sezonowość cen soi na rynku futures w Chicago (CBOT)[^1].  
  
  
## Przegląd literatury  
  
- Znacznie prostszym filtrem często stosowanym w celu oczyszczenia danych w empirycznej pracy ekonometrycznej są sezonowe zmienne dummy, które są dodawane do równań regresji, patrz Lovell (1963), lub filtr różnicy sezonowej stosowany przez Box & Jenkins (1970).  
- Box i Jenkins założyli, że istnieją pierwiastki jednostkowe przy częstotliwościach sezonowych w modelu autoregresyjnym i zasugerowali, że filtr różnicy sezonowej powinien być stosowany do momentu, aż przekształcone szeregi staną się stacjonarne.[^2]  
- Wielu autorów, w tym Dickey, Hasza i Fuller (1984), Hylleberg, Engle, Granger i Yoo. (1990), Canova i Hansen (1995), Taylor (1998) oraz Koop i VanDijk (2000), a także Arteche (1998) oraz Arteche i Robinson (2000), zaproponowali testowanie sezonowych pierwiastków jednostkowych/integracji[^3].  
  
### Sezonowość  
- Termin "sezonowość" odnosi się do skumulowanego wpływu zjawisk meteorologicznych i instytucjonalnych, które występują w sposób mniej lub bardziej spójny w skali roku.[^5]  
- Pogoda, sposób organizacji naszego kalendarza, decyzje związane z czasem i oczekiwania to cztery główne rzeczy, które powodują sezonowość.[^6]  
- Statystycy ekonomiczni uznają, że ekonomiczny szereg czasowy składa się z długookresowego trendu, ruchu cyklicznego, efektu sezonowego i ruchu nieregularnego.[^7]  
  
#### Cechy sezonowości  
- Inną cechą wahań sezonowych jest to, że chociaż powtarzają się one co roku z pewną regularnością, ich charakter może się zmieniać. Wahania sezonowe można oddzielić od trendu z powodu ich oscylacyjnego charakteru, od cyklu koniunkturalnego z powodu ich okresowości, a od anomalii z powodu ich systematyczności.[^8]  
### Model sezonowości  
- Jeżeli twórcy modelu nie biorą pod uwagę sezonowości w specyfikacji modelu, ponieważ uważają, że użycie sezonowo dostosowanych danych wyeliminowało tę potrzebę, mogą zostać doprowadzeni do błędnej specyfikacji modelu, mylących wniosków dotyczących wartości parametrów i złych prognoz.[^9]  
- sezonowy model regresyjny można zapisać jako:  
	- $Y_t = S_t + \epsilon_t$  
	- $t = 1,...,T$  
	- $S_t = \sum^S_{j=1} \gamma_j*d_{jt}$ subject to $\sum^S_{j=1} \gamma_j$ = 0  
	- gdzie dj's są zmiennymi dummy przyjmującymi wartość jedności w sezonie j i wartość zero w pozostałych sezonach; $ε_t$ WN(0, $σ^2_ε$ ) jest procesem białego szumu o zerowej średniej, homoskedastycznym i nieskorelowanym.[^10]  
  
  
  
## Literatura  
  
Sezonowość to jedna z cech charakterystycznych dla rynków towarowych, która odróżnia je od akcji, obligacji i innych konwencjonalnych aktywów finansowych.[^11]  
  
Teoria magazynowania" Kaldora 1939, Working 1948, 1949 i Telsera 1958 wyjaśnia dogodny zysk w kategoriach wbudowanej opcji czasowej. W szczególności posiadacz towaru nadającego się do przechowywania, np. ropy naftowej, gazu ziemnego, miedzi, może zdecydować, kiedy go skonsumować. Jeśli optymalne jest przechowywanie towaru do przyszłej konsumpcji, to jest on wyceniany jak aktywo, ale jeśli optymalne jest jego natychmiastowe zużycie, to towar jest wyceniany jak dobro konsumpcyjne.  
  
  
  
---  
  
### Rynek  
  
  
#### Soja  
- Lipiec, czerwiec i sierpień są zazwyczaj słabymi miesiącami dla soi. Soja podlega również zjawisku lutego, gdzie ceny mogą wykazywać słabość w miesiącu[^12]  
- Standardowe miesiące handlowe dla kontraktów terminowych na kukurydzę, soję i pszenicę odzwierciedlają sezonowe wzorce sadzenia, zbierania i wprowadzania do obrotu upraw bazowych. Te miesiące handlowe wskazują również na źródło podaży w danym czasie. W miesiącach sadzenia, wiosną w przypadku kukurydzy i soi oraz jesienią w przypadku pszenicy ozimej, źródłem ziarna dostępnego do sprzedaży lub zakupu przez użytkowników końcowych są uprawy, które zostały zebrane w poprzednim sezonie zbiorów - stare plony. W miesiącach, kiedy podaż jest niższa, zboże jest droższe niż w bardziej odległych miesiącach, kiedy sprzedawane są nowe zbiory. Podczas miesięcy ze starymi plonami, kiedy podaż jest zazwyczaj niższa, ziarno ma tendencję do bycia wycenionym wyżej niż dalej wychodzące miesiące handlowe z nowymi plonami. W przypadku soi, żniwa rozpoczynają się we wrześniu i trwają przez październik do połowy listopada. Soja ma tendencję do podążania za wzorcem, w którym ceny zaczynają spadać w okresie lipiec-sierpień, kontynuując przez "przerwę lutową", zanim osiągną swoje sezonowe maksimum w lecie. Śruta sojowa i olej sojowy wykazują takie same tendencje sezonowe jak soja.[^13]  
- Ceny soi są również zazwyczaj najniższe podczas jesiennych zbiorów.  Podobnie jak w przypadku kukurydzy, ceny i podstawy mają tendencję do wzmacniania się po zbiorach. Jednak na rynek soi ogromny wpływ mają rozpoczynające się w lutym zbiory soi w Ameryce Południowej.  Zmniejsza to prawdopodobieństwo zimowych wzrostów cen na rynku amerykańskim, chyba że w Ameryce Południowej zbiory będą mniejsze niż przeciętnie. Ceny w Stanach Zjednoczonych zaczynają rosnąć, gdy znana jest wielkość zbiorów w Ameryce Południowej i zbliża się sezon sadzenia w USA. Ceny wiosną i latem koncentrują się na warunkach upraw w USA. Wszystkie te czynniki składają się na ceny soi, które zazwyczaj osiągają szczyt w połowie lub pod koniec lata i zmniejszają się do czasu zbiorów. Wzrost cen po zbiorach nie jest tak dramatyczny dla soi jak cena kukurydzy, chyba że Ameryka Południowa doświadcza problemów związanych z pogodą.[^14]  
  
#### Ceny  
- Tabela 3: Wyniki regresji wskazujące na wpływ miesięcy kalendarzowych 1990-2013[^15]  
  
| Miesiąc | Soja |  
|-----------|---------|  
| Styczeń   | -0.179  |  
| Luty  | -0.045  |  
| Marzec | 0,061 |  
| Kwiecień | 0.210 |  
| Maj | 0.371 |  
| Czerwiec | 0.441 |  
| Lipiec | 0.445 |  
| Sierpień | 0.289 |  
| Wrzesień | -0,097 |  
| Październik | -0,272 |  
| Listopad | -0,094 |  
| Przecięcie (grudzień) | 3.512* |  
  
## Dane  
- Dane, które analizujemy w badaniu to cotygodniowe ceny zamknięcia kontraktów futures na soję na rynku CBOT, przyjmuje się, że to najistotniejszy rynek dla tego surowca.[^1]  
- Dane pochodzą z Refinitiv Reuters, obejmują 10 ostatnich lat.  
  
## Operacje na danych  
- Wykres kursy bez przekształceń 11.2012-11.2022 (v2)  
  
![](file:///tmp/lu23546313rg00.tmp/lu23546313rg74_tmp_9846d8da65df6e1.png)  
  
- Wykres pierwszych różnic zmiennej d_v2  
  
![](file:///tmp/lu23546313rg00.tmp/lu23546313rg74_tmp_c7cc397c67272564.png)  
  
    
    
  
1.  Test ADF dla szeregu bez przekształceń (v2)  
![](https://i.imgur.com/EUyk5aK.png)  
  
![](https://i.imgur.com/MtwD4G7.png)  
  
Wartość p dla testu ADF dla zmiennej (v2) z wyrazem wolnym bez trendu liniowego (const) jest wyższa (0,2145) niż poziom istotności przyjęty w badaniu (0,05). Zatem nie ma podstaw do odrzucenia hipotezy zerowej. Wniosek: brak stacjonarności.  
  
-  Test ADF dla pierwszych różnic zmiennej.  
![](file:///tmp/lu23546313rg00.tmp/lu23546313rg9q_tmp_f8125b7e53301d69.png)  
  
![](https://i.imgur.com/Z8qr0Eh.png)  
  
Wartość p dla testu ADF dla pierwszych różnic zmiennej (v2) z wyrazem wolnym bez trendu liniowego (const) jest niższa (3,532e-038) niż poziom istotności przyjęty w badaniu (0,05). Zatem istnieją podstawy do odrzucenia hipotezy zerowej. Wniosek: możliwa stacjonarności.  
  
- ACF i PACF  
  
![](file:///tmp/lu23546313rg00.tmp/lu23546313rgbb_tmp_e493df4ba44d201d.png)  
  
![](file:///tmp/lu23546313rg00.tmp/lu23546313rgbb_tmp_4c32c6700351feea.png)  
  
Najwyższym rzędem opóźnień dla badanej zmiennej (d_v2) są opóźniania rzędu 12 z uwagi na wyższą niż dla pozostałych istotność (przy poziomie 5%) dla funkcji autokorelacji cząstkowej PACF. Natomiast dla funkcji autokorelacji ACF wszystkie rzędy opóźnień charakteryzują się wysoką istotnością (na poziomie 1%).  
![](https://i.imgur.com/vnq1Off.png)  
  
![](https://i.imgur.com/MyKg17p.png)  
  
Najwyższym rzędem opóźnień dla pierwszych różnic badanej zmiennej (d_v2) są opóźniania rzędu 19 z uwagi na wysoką istotność (przy poziomie 1%) zarówno dla funkcji autokorelacji ACF jak i autokorelacji cząstkowej PACF.  
  
  
## Wnioski  
Badaniu podlegał szereg czasowy kursów soi pochodzących z CBOT. Szereg początkowo nie wykazywał stacjonarności, co wykazane zostało poprzez badanie rozszerzonym testem DF (ADF), które ujawniło, iż wartości p-value były wyższe niż poziom istotności α przyjęty na potrzeby analizy. Z kolei test ADF z wykorzystaniem pierwszych różnic zmiennej charakteryzował się wartością p-value zdecydowanie niższą niż poziom istotności α pozwalającą na stwierdzenie iż w tym przypadku może występować stacjonarność. W dalszej kolejności została przeprowadzona analiza korelogramu z uwzględnieniem testów ACF i PACF. Przeprowadzona analiza ujawniła iż celem zniwelowania efektu sezonowości należałoby wprowadzić do szeregu opóźnienia rzędu 19 z uwagi na ich wysoki poziom istotności.  
  
  
  
## Footnotes  
  
[^1]: Bain, C. (2013). Guide to Commodities: Producers, players and prices, markets, consumers and trends. John Wiley & Sons.  
[^2]: Brendstrup, B., Hylleberg, S., Nielsen, M. Ø., Skipper, L., & Stentoft, L. (2001). Seasonality in economic models. _University of Aarhus, Economics Working Paper_, (2001-16).  
[^3]: Brendstrup, B., Hylleberg, S., Nielsen, M. Ø., Skipper, L., & Stentoft, L. (2001). Seasonality in economic models. _University of Aarhus, Economics Working Paper_, (2001-16).  
[^4]: Brendstrup, B., Hylleberg, S., Nielsen, M. Ø., Skipper, L., & Stentoft, L. (2001). Seasonality in economic models. _University of Aarhus, Economics Working Paper_, (2001-16).  
[^5]: Dagum, E. B. (2001). Time Series: Seasonal Adjustment. International Encyclopedia of the Social & Behavioral Sciences, 15739–15746. doi:10.1016/b0-08-043076-7/00522-2   
[^6]: Dagum, E. B. (2001). Time Series: Seasonal Adjustment. International Encyclopedia of the Social & Behavioral Sciences, 15739–15746. doi:10.1016/b0-08-043076-7/00522-2   
[^7]: Anderson, T. W. (1994). The Statistical Analysis of Time Series. Wiley Series in Probability and Statistics. doi:10.1002/9781118186428   
[^8]: Dagum, E. B. (2001). Time Series: Seasonal Adjustment. International Encyclopedia of the Social & Behavioral Sciences, 15739–15746. doi:10.1016/b0-08-043076-7/00522-2   
[^9]: Plosser, C. I., Chow, G. C., & Lombra, R. E. (n.d.). A time series analysis of seasonality in econometric models (1978). The Structural Econometric Time Series Analysis Approach, 332–396. doi:10.1017/cbo9780511493171.010   
[^10]: Plosser, C. I., Chow, G. C., & Lombra, R. E. (n.d.). A time series analysis of seasonality in econometric models (1978). The Structural Econometric Time Series Analysis Approach, 332–396. doi:10.1017/cbo9780511493171.010   
[^11]: Routledge, B. R., Seppi, D. J., & Spatt, C. S. (2000). Equilibrium forward curves for commodities. _The Journal of Finance_, _55_(3), 1297-1338.  
[^12]: [Seasonality and how it Affects Commodities](https://www.financial-spread-betting.com/Seasonality-commodities.html)  
[^13]: [Understanding Seasonality in Grains](https://www.cmegroup.com/education/courses/introduction-to-agriculture/grains-oilseeds/understanding-seasonality-in-grains.html)  
[^14]: [Seasonal Grain Price Patterns](https://farms.extension.wisc.edu/articles/seasonal-grain-price-patterns/)  
[^15]: Jayaramu, N. (2015). Impact of seasonality on agricultural commodity price behavior. _Northwest Missouri State University_.  
[^16]: [Report - Argentina's soybean crop severely delayed due to drought, says grains exchange](Attachments/Top%20News%20_%20Argentina's%20soybean%20crop%20severely%20delayed%20due%20to%20drought,%20says%20grains%20exchange.pdf)  
[^17]: Argentina's soybean crop severely delayed due to drought, says grains exchange - [external link](https://cloud.harhara.bar/s/KCi4GYEHckFDWyy)  
[^18]: [Report - Cotton jumps about 3% on softer dollar, gains in wider markets - RTRS  News Wires](Attachments/News_%20RPT-India's%20cotton%20exports%20stall%20as%20farmers%20delay%20sales%20hoping%20for%20higher%20prices%20-%20RTRS%20_%20News%20Wires.pdf)  -   
[^19]: [Report](Attachments/News_%20Cotton%20COT.md)   
[^20]: [Report](Attachments/News_%20Cotton%20jumps%20about%203%25%20on%20softer%20dollar,%20gains%20in%20wider%20markets%20-%20RTRS%20_%20News%20Wires.pdf) - [external link](https://cloud.harhara.bar/s/SR7gLcDbiz9Yq24)  
[^21]: Sørensen, C. (2002). Modeling seasonality in agricultural commodity futures. _Journal of Futures Markets: Futures, Options, and Other Derivative Products_, _22_(5), 393-426.  
[^22]: Richter, M. C., & Sørensen, C. (2002). Stochastic volatility and seasonality in commodity futures and options: The case of soybeans. _Available at SSRN 301994_.  
[^23]: Routledge, B. R., Seppi, D. J., & Spatt, C. S. (2000). Equilibrium forward curves for commodities. _The Journal of Finance_, _55_(3), 1297-1338.  
[^24]: Brendstrup, B., Hylleberg, S., Nielsen, M. Ø., Skipper, L., & Stentoft, L. (2001). Seasonality in economic models. _University of Aarhus, Economics Working Paper_, (2001-16).  
[^25]: Dagum, E. B. (2001). Time Series: Seasonal Adjustment. International Encyclopedia of the Social & Behavioral Sciences, 15739–15746. doi:10.1016/b0-08-043076-7/00522-2   
[^26]: Plosser, C. I., Chow, G. C., & Lombra, R. E. (n.d.). A time series analysis of seasonality in econometric models (1978). The Structural Econometric Time Series Analysis Approach, 332–396. doi:10.1017/cbo9780511493171.010   
[^27]: [Oil Crops Sector at a Glance](https://www.ers.usda.gov/topics/crops/soybeans-and-oil-crops/oil-crops-sector-at-a-glance/)  
