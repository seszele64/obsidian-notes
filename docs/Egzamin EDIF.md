---  
tags:  
- data  
- edif  
project:  
title: Egzamin EDIF  
share: True  
hide:  
- navigation  
date created: Tuesday, November 29th 2022, 9:32:00 pm  
date modified: Monday, December 5th 2022, 7:59:53 pm  
---  
  
  
[TOC]  
  
- EGZAMIN W FORMIE TESTU (PYTANIA ZAMKNIĘTE I OTWARTE)  
	- TERMIN EGZAMINU: 30.11.2022 R  
  
   
 zagadnienia  
	 nie da nam testowania ==słabej efektywności rynku==, ani testu równości dwóch średnich stóp zwrotu (części podpunktów 7 i 8 z pliku z zagadnieniami).  
 - Będzie za to na pewno zadanie z interpretacji ==modelu korekty błędem==, przykłady stacjonarnych i niestacjonarnych, czytanie korelogramu, modele sezonowe  
  
 Pliki teams  
	 [Wykłady](https://teams.microsoft.com/_#/school/FileBrowserTabApp/Og%C3%B3lny?threadId=19:eIWpEe5ejkUTlKbbxQxzGj_fitlC22_4BC_cjmwqGYw1@thread.tacv2&ctx=channel)  
  
  
# Egzamin EDIF - Zagadnienia  
  
## Co Oznaczają Pojęcia (oraz **przyczyny** występowania)?  
  
>Zjawiska te występują często ze względu na nieliniowe zachowania uczestników rynku  
- W zależności od analizowanego instrumentu finansowego, okresu obejmującego badanie oraz horyzontu stóp zwrotu, możliwe są częściowo odmienne wyniki, niemniej jednak zaobserwowano następujące własności charakteryzujące stopy zwrotu  
  
- efekt skupiania (gromadzenia) zmienności  
	- ![](https://i.imgur.com/GpNvUgi.png)  
	- efektu skupiania (gromadzenia) zmienności (volatility clustering), co oznacza, że zarówno małe, jak i duże zmiany kursu następują seriami, a tym samym oznacza niestałość wariancji[^1] stóp zwrotu w czasie,  
	- W szeregach czasowych stóp zwrotu można bowiem wyróżnić okresy większej i mniejszej aktywności inwestorów, czyli okresy z dużymi zmianami cen (tzw. skupiska zmienności, clusters) oraz okresy o mniejszych zmianach cen. Okresy te występują seriami. Małe zmiany cen (małe co do wartości bezwzględnej stopy zwrotu) następują po małych zmianach, a duże po dużych, lecz kierunek zmian (znak stopy zwrotu) jest nieprzewidywalny. Bardzo częstym efektem jest tworzenie się wokół dużego głównego skupiska zmienności, mniejszych okresów o większej niż zazwyczaj aktywności inwestorów.  
- efekt leptokurtozy i grubych ogonów rozkładów stóp zwrotu  
	 - ![](https://i.imgur.com/S3GOqnY.png)  
	 - prawdopodobieństwo wystąpienia dużych, nietypowych zmian kursu (duże co do wartości bezwzględnej stopy zwrotu) jest większe niż gdyby stopy zwrotu pochodziły z rozkładu normalnego,  
- efekt skośności rozkładów stóp zwrotu[^2]  
	 - efektu skośności rozkładów stóp zwrotu (najczęściej obserwuje się rozkłady prawostronnie skośne, lecz nie jest to regułą),  
 - Zaobserwowano, że w większości szeregów stóp zwrotu częściej występują stopy zwrotu większe niż modalna, co tłumaczy się ==odmiennym zachowaniem inwestorów w czasie hossy i bessy== lub dokładniej odmiennymi zachowaniami w przypadku napływania dobrych i złych informacji. Skutkuje to dodatnim współczynnikiem skośności wyznaczanym dla większości szeregów empirycznych. Nie jest to jednak regułą, gdyż współczynnik skośności dla np. szeregu stóp zwrotu z indeksu WIG (z okresu od rozpoczęcia notowań do maja 2002 roku) przyjmuje wartość ujemną, co świadczy o skośności lewostronnej rozkładu empirycznego. Podczas analizy dziennych stóp zwrotu z 35 instrumentów z rynku polskiego, w 22 przypadkach uzyskano dodatni współczynnik skośności, a w 13 przypadkach - ujemny (por. Jajuga (2000a)). Także w przypadku współczynnika skośności wynik badania zależy od wybranego okresu oraz analizowanego horyzontu stóp zwrotu (por. Konarzewska (1998), (2000)). Ogólnie założyć należy, iż rozkłady stóp zwrotu mogą charakteryzować się zarówno dodatnią, jak i ujemną skośnością. W niektórych przypadkach efekt ten jest na tyle znaczny, że przyjęcie założenia o braku skośności rozkładu może znacznie fałszować obraz rzeczywistości.  
- efekt autokorelacji stóp zwrotu[^3]  
	 - ![](https://i.imgur.com/FnNaYKh.png)  
	 - szczególnie w okresach o małej zmienności  
	 - W niektórych analizowanych szeregach czasowych obserwuje się, iż kolejne stopy zwrotu są skorelowane. Po wzrostach występują częściej kolejne wzrosty, a po spadkach kolejne spadki. Najczęściej zasięg zależności korelacyjnej ograniczony jest do opóźnień o rzędzie mniejszym niż 5, ale może wynosić nawet kilkadziesiąt, bądź kilkaset, co nazywane jest wtedy „długą pamięcią procesu”.[^4]  
  
---  
  
## Finansowe Szeregi Czasowe  
  
### Pojęcia Podstawowe  
  
#### Stopa Zwrotu Zwykła  
 - $R_t = \frac{P_t - P_{t-1}}{P_{t-1}}*100\%$[^5]  
 - prosta stopa zwrotu wykorzystuje koncepcje kapitalizacji okresowej  
 - rozkład - rozkład ceny, w przedziale $[-1; +\infty)$ lub $[-100\%;+\infty)$[^6]  
  
#### Stopa Zwrotu Logarytmiczna  
 - $r_t = ln(P_t / P_{t-1}) * 100\%$[^7]  
 - wykorzystuje koncepcję kapitalizacji ciągłej  
 - rozkład - logarytmiczne przekształcenie ceny  
 - ==addytywność==  
	 - logarytmiczne stopy zwrotu są ==addytywne==, w danym okresie, dzięki temu można liczyć średnią stopę z okresu przy wykorzystaniu średniej arytmetycznej[^8]  
	 - Z właściwości logarytmów wynika ważna (zwłaszcza w przypadku badań giełdowych) cecha logarytmicznych stóp zwrotu, a mianowicie ich addytywność. Suma poszczególnych logarytmicznych stóp zwrotu z danego okresu jest tożsama z logarytmiczną stopą zwrotu uwzględniającą tylko wartość końcową i początkową w danym okresie.  
  
#### Ryzyko (odchylenie standardowe)  
 - W zakresie definiowania ryzyka wymienia się ogólnie cztery podstawowe nurty (por. Jackowicz (1996), Wojtasiak (2002)):  
	 - decyzyjny, w którym ryzyko definiowane jest poprzez konsekwencję konieczności podejmowania decyzji w celu realizacji określonych celów w sytuacji niepełnej wiedzy o przyszłości,  
	 - przyczynowy, w którym główny nacisk położony jest na przyczyny ryzyka zwane „źródłami ryzyka”,  
	 - dochodowy, w którym pojęcie ryzyka zawężone zostaje do niemożności określenia rezultatu działań, najczęściej wielkości przyszłego dochodu,  
	 - ilościowy, w którym ryzyko definiowane jest poprzez odpowiednie miary (np. poprzez odchylenie standardowe, prawdopodobieństwo, wrażliwość).  
- Rodzaje ryzyk  
	- **Ryzyko gospodarcze** (economic risk) - możliwość nieosiągnięcia spodziewanych efektów ekonomicznych działalności gospodarczej lub poniesienia strat, przekroczenia kosztów, zmniejszenia przychodów (por. Olzacka, Pałczyńska (1998)).  
	- **Ryzyko finansowe**  
		- wiąże się z możliwymi przepływami pieniężnymi, które płaci i otrzymuje podmiot. Ryzyko to wynika z powiązania tego podmiotu z otoczeniem, zwłaszcza z rynkiem finansowym (por. Jajuga (1999b)).  
		- jest prawdopodobieństwem utraty przez organizację posiadanych zasobów finansowych oraz prawdopodobieństwem utraty środków finansowych, które są już w organizacji oraz nie osiągnięcia spodziewanych zysków (por. Bizon-Górecka (2000)).  
		- można określić jako ryzyko, które wiąże się z możliwością poniesienia strat na rynkach finansowych (por. Jorion (2001)).  
	- **Ryzyko rynkowe** jest ryzykiem wynikającym ze zmian cen na rynkach finansowych i towarowych. Ryzyko to dotyczy zarówno zmian cen instrumentów bazowych (stóp procentowych, cen akcji, indeksów, walut, towarów), jak i zmian cen instrumentów pochodnych (opcji, warrantów, kontraktów terminowych, swapów). Bardzo często ryzyko to łączy się również z ryzykiem płynności instrumentów finansowych.  
	- **Ryzyko płynności** występuje w sytuacji, gdy ze względu na niedopasowanie wielkości podaży i popytu, bądź ze względu na przeciwstawne oczekiwania stron rynku, niemożliwe lub utrudnione jest kupowanie bądź sprzedawanie danego instrumentu finansowego lub towaru bez ponoszenia dodatkowych kosztów natychmiastowego otwarcia lub zamknięcia pozycji. Podejście to jest zgodne z traktowaniem ryzyka płynności w kontekście ryzyka płynności aktywów .  
	- **Ryzyko kredytowe** jest ryzykiem związanym z możliwością niedotrzymania warunków kontraktu przez drugą stronę transakcji. Może ono dotyczyć sytuacji, gdy partner zaprzestaje spłaty zobowiązań, opóźnia się z terminami spłaty lub nie wywiązuje się w inny sposób ze zobowiązań finansowych w całości lub częściowo  
	- **Ryzyko operacyjne** jest ryzykiem o charakterze systemowym (niezwiązanym z inwestowaniem), którego źródło tkwi w niewystarczającej kontroli, niesprawnych systemach, błędach człowieka, niewłaściwym zarządzaniu. Osobno wyróżnia się więc na przykład: ryzyko personelu, organizacyjne, (braku) kontroli, infrastruktury technicznej. Ryzyko to obejmuje w szczególności również ryzyko oszustwa, ryzyko regulacji, ryzyko katastrofowe (związane z siłami przyrody). Jednym z aspektów ryzyka operacyjnego jest ryzyko utraty reputacji.  
	- **Ryzyko prawne** związane jest z możliwością poniesienia strat w wyniku prowadzenie przez podmiot działalności wykraczającej poza ramy odpowiednich przepisów prawnych lub regulacji i obejmujące niemożność wyegzekwowania warunków kontraktu. Ryzyko prawne wiąże się również z sytuacją, gdy następuje nieprzewidziana zmiana prawa, prowadząca do zmiany sytuacji podmiotu. Ryzyko to można definiować również w aspekcie neutralnym, w którym zmiany prawa mogą prowadzić do uzyskania korzyści. Ryzyko to bywa uznawane za składową ryzyka operacyjnego  
	- **Ryzyko biznesu** związane z prowadzoną przez instytucję (przedsiębiorstwo) działalnością podstawową, rynkiem produktów i usług. Ryzyko to ma charakter długoterminowy i strukturalny, powstający na skutek decyzji inwestycyjnych dotyczących m.in. wyboru strategii rozwoju, strategii marketingowej, decyzji cenowych, decyzji co do poziomu przyszłej sprzedaży[^9]  
  
#### Szereg Czasowy  
  
##### Proces Stochastyczny  
 - rodzinę $X_t$ $t \in T$ zmiennych losowych określonych ==na tej samej przestrzeni probabilistycznej== nazywa się procesem stochastycznym  
	 - zazwyczaj T jest podzbiorem przedziału $[0, +\infty)$ i interpretuje się go jako czas  
	 - w ekonometrii finansowej realizację procesu stochastycznego nazywa się szeregiem czasowym i oznacza $x_t$[^10]  
  
##### Dekompozycja Szeregu Czasowego  
 - proces wyodrębniania poszczególnych składowych szeregu czasowego  
	 - $X_t = m_t + s_t + Y_t$  
		 - $X_t$ - dane pomiarowe  
		 - $m_t$ - trend  
			 - długotrwały wzrost lub spadek wartości zmiennej, bądź inna regularność - np. naprzemienne spadki oraz wzrosty wartości danych[^11]  
		 - $s_t$ - sezonowość  
			 - występuje, gdy na wartości danych w szeregu czasowym wpływają czynniki sezonowe (dzienne, miesięczne, kwartalne, roczne), wyróżnić można sezonowość addytywną i multiplikatywną[^12]  
		 - $Y_t$ - szum (proces losowy, stacjonarny)[^13]  
 - cel  
	 - Celem dekompozycji szeregu czasowego jest oszacowanie i ekstrakcja deterministycznych części szeregu - trendu $m_t$ oraz sezonowości $s_t$ w nadziei, że pozostałe dane, czyli teoretycznie zmienna losowa $Y_t$ okaże się stacjonarnym procesem losowym  
	 - W przypadku, kiedy okaże się to prawdą, tj. reszty $Y_t$ mogą być opisane stacjonarnym procesem losowym ${Y_t}$, możemy przystąpić do przewidywania przyszłego zachowania się szeregu, wykorzystując oczywiście wszystkie posiadane wiadomości: trend, okres oraz zidentyfikowany z pewną dokładnością proces losowy.[^14]  
  
---  
  
### Ekonometryczne Modele Wahań Sezonowych  
  
#### Periodogram I Spektrum Procesu  
- Any time series can be expressed as a combination of cosine and sine waves with differing periods (how long it takes to complete a full cycle) and amplitudes (maximum/minimum value during the cycle). This fact can be utilized to examine the periodic (cyclical) behavior in a time series.[^15]  
- Period  
	- T  
	- number of periods required to complete a single cycle  
- Frequency  
	- $\omega = 1/T$  
	- the fraction of the complete cycle that's completed in a single time period  
  
- example  
	- ![](https://online.stat.psu.edu/onlinecourses/sites/stat510/files/L06/graph_59.gif)  
	- The periodogram shows a dominant spike at a ==low frequency==  
	- The peak value of periodogram is the fifth value, and that corresponds to a frequency of ==0.0312500==  
	- The period for this value = ==1/0.0312500 = 32==. That is, it takes 32 time periods for a complete cycle.[^16]  
  
- Modele sezonowości ze zmiennymi zerojedynkowymi    
	 - sezonowość periodyczna bez wyrazu wolnego  
	 - sezonowość periodyczna z wyrazem wolnym[^17]  
	 - sezonowości periodyczna z wyrazem wolnym i trendem  
  
#### Metodologia Boxa I Jenkinsa (Identyfikacja procesów)  
- Inną, alternatywną metodą do opisanej wyżej, jest metoda która dopasowywuje modele ARMA i ARIMA do istniejących danych. Metoda ta została nazwana po nazwiskach dwóch statystyków Georgea Boxa oraz Gwilyma Jenkinsa, którzy rozwinęli tą metodę w latach 70-tych.  
- Algorytm Boxa-Jenkinsa składa się z trzech kroków:  
	1. Identyfikacja oraz wybór modelu: pierwszym krokiem jest upewnienie się, że analizujemy dane stacjonarne; następnie identyfikujemy sezonowość i usuwamy ją z danych aby w końcu wykorzystując wykresy funkcji autokorelacji oraz częściowej autokorelacji zdecydować jakie komponenty AR (autoregresji), I (scałkowane) lub MA (średniej ruchomej) wykorzystać do budowy modelu.  
	2. Znalezienie parametrów wybranego modelu za pomocą wybranych metod (numerycznych) tak, aby dopasowanie danych do modelu było najlepsze. Najczęstszymi metodami wykorzystywanymi w praktyce są: maximum likelihood estimation lub (nieliniowa) metoda najmniejszych kwadratów.  
	3. Sprawdzenie poprawności wyboru danego modelu. W szczególności należy sprawdzić czy proces jest stacjonarny - reszty muszą być od siebie niezależne, oraz ich średnia i wariancja musi być stała w czasie. Można  
		- narysować wykres średniej, wariancji oraz reszt versus czas (indeks) i przeprowadzić na nich test Ljunga-Boxa,  
		- narysować wykresy funkcji autokorelacji i częściowej autokorelacji reszt.[^18]  
  
#### Funkcja Autokorelacji I Autokorelacji Cząstkowej  
- ACF  
	- The covariance between $y_t$ and its value at another time period, say, $y_{t+k}$ is called the autocovariance at lag k  
		- $𝛾k = Cov(yt , yt+k) = E[(yt − 𝜇)(yt+k − 𝜇)]$  
		- The collection of the values of 𝛾k, k = 0, 1, 2,… is called the **autocovariance function**  
	- The autocorrelation coefficient at lag k for a stationary time series is  
		- $𝜌k = \frac{E[(yt − 𝜇)(yt+k − 𝜇)]}{√E[(yt − 𝜇)2]E[(yt+k − 𝜇)2]} = \frac{Cov(yt, yt+k)}{Var(yt)} = \frac{𝛾k}{𝛾0}$  
		- The collection of the values of $\rho_k$, k = 0, 1, 2,… is called the autocorrelation function (ACF)[^19]  
  
- Funkcja autokorelacji (ACF) mierzy zależności statystycznej zmiennej z jej opóźnieniem k-tego rzędu.  
	- ACF:  
		- $𝜌k = \frac{E[(yt − 𝜇)(yt+k − 𝜇)]}{√E[(yt − 𝜇)2]E[(yt+k − 𝜇)2]} = \frac{Cov(yt, yt+k)}{Var(yt)} = \frac{𝛾k}{𝛾0}$  
  
  
- PACF  
	- Funkcja cząstkowej autokorelacji (PACF) uwzględnia tylko opóźnienie do- kładnie k-tego stopnia[^20]  
  
- Interpretacja:  
	- Jeśli funkcja powoli maleje w ACF → model AR → Odcięcie w PACF zapewni porządek p dla AR (p).  
		- ![](https://i.imgur.com/vJp05RM.png)  
  
	- Jeśli funkcja powoli maleje w PACF → model MA → Odcięcie w ACF zapewni porządek p dla MA (q).  
		- ![](https://i.imgur.com/KyA4fNC.png)  
  
	- Jeśli funkcja powoli maleje w ACF i PACF → model ARMA  
		- ![](https://i.imgur.com/6pAJNbB.png)[^21]  
  
	- sezonowość  
		- Seasonal AR process  
			- ![](https://i.imgur.com/eqEGNpR.png)  
		- Seasonal MA process  
			- ![](https://i.imgur.com/qGmHtmA.png)  
		- Seasonal ARMA process  
			- ![](https://i.imgur.com/tkgqu3F.png)[^22]  
		- ![podsumowane](https://miro.medium.com/max/4800/1*BFZhxMlJLw_UgFGUVzadRA.png)  
  
  
  
#### Kryteria Informacyjne  
- Kryteria informacyjne pozwalają porównywać różne modele dla tej samej zmiennej zależnej. Najlepszym modelem jest model, dla którego ==wartość kryterium jest najniższa==.  
- Interpretacja jest tylko relatywna - ocenić możemy, że któryś model jest lepszy niż inne, ale nie możemy ocenić jak  dobry  
- Kryterium Akaike:  
	- $AIC = ln(\hat{\sigma}^2_u) + \frac{2K}{n}$  
- Kryterium Schwartza  
	- $SIC = ln(\hat{\sigma}^2_u) + \frac{K*ln(n)}{n}$  
		- większa 'kara' za liczbę parametrów w modelu[^23]  
  
---  
  
### Charakterystyki Procesów Ekonomicznych  
#### **Błądzenie Losowe I Biały Szum – Czy Są to Procesy stacjonarne?**  
  
  
##### Błądzenie Losowe  
- Najprostszy ==niestacjonarny== szereg czasowy generowany jest przez model błądzenia losowego  
- Zakłócenie $e_t$ jest zmienną losową o stałych parametrach:  
	- wartości oczekiwanej $\bar{e} = 0$  
	- wariancji $\sigma^2$  
	- zerowych autokowariancji  
- Szereg otrzymany przez obliczenie różnic jest stacjonarny.  
  
##### Biały Szum  
- proces ==stacjonarny==  
- $E(y_t) = 0$ - wartość oczekiwana 0  
- $var(y_t) = \sigma^2 < \infty$ - skończona wariancja  
- $cov(y_t, y_{t-k}) = 0$, k = 1,2....[^24]  
  
- Przykłady procesów stacjonarnych i niestacjonarnych  
	- procesy stacjonarne  
	- procesy niestacjonarne  
  
#### **Stacjonarność procesu**  
##### Warunki Ścisłej Stacjonarności  
- If a time series has a finite mean and autocovariance function it is said to be second-order stationary (or weakly stationary of order 2). If, in addition, the joint probability distribution of the observations at all times is ==multivariate normal==, then that would be sufficient to result in a time series that is strictly stationary[^25]  
  
##### **warunki Słabej stacjonarności**  
- wartość oczekiwana jest stała w czasie  
	- $E(y_t) = \mu$  
- wariancja jest stała w czasie i skończona  
	- $Var(y_t) = E(y_t - \mu)^2 = \sigma^2 < \infty$  
- kowariancja między dwoma okresami zależy wyłącznie od odległości pomiędzy nimi, a nie od wyboru konkretnego momentu w czasie  
	- $Cov(y_t, y_{t+k}) = E[(y_t - \mu)(y_{t+k}-\mu)]=\lambda_k$[^26][^27]  
  
#### Testowanie Rzędu Zintegrowania  
##### **test Pierwiastka Jednostkowego Dickey’a Fullera** (oraz Rozszerzony Test Dickeya Fullera) – Wnioskowanie, Hipotezy, Statystka Empiryczna  
  
###### Hipoteza  
- równanie szeregu autoregresyjnego: $Y_t = \beta_1 * Y_{t-1} + \xi_t$  
- $H_0: \beta_1 = 1$ - proces jest ==niestacjonarny==  
	- proces jest błądzeniem losowym  
- $H_1: \beta_1 < 1$ - proces jest ==stacjonarny==  
###### Etapy  
1. Wybór postaci modelu (z wyrazem wolnym, bez wyrazu wolnego)  
2. Estymacja równania  
	- $\Delta Y_t = \delta Y_{t-1} + \xi_t$ (bez wyrazu wolnego) lub  
	- $\Delta Y_t = \delta Y_{t-1} + \xi_t + \mu$ (z wyrazem wolnym)  
	- $\mu$ - wyraz wolny  
	- $\delta = (\beta_1 - 1)$ - pierwiastek jednostkowy  
	- skąd ten model?  
		- odejmujemy od równania modelu autoregresyjnego $Y_{t-1}$ (poprzedni okres)  
			- $Y_t = \beta_1 * Y_{t-1} + \xi_t$ / -$Y_{t-1}$  
			- $Y_t - Y_{t-1} = \beta_1 * Y_{t-1} - Y_{t-1} + \xi_t$  
			- $\Delta Y_t = (\beta_1 - 1)*Y_{t-1} + \xi_t$  
3. obczajamy autokorelację składnika losowego  
	- brak autokorelacji składnika losowego -> test DF  
	- autokorelacja składnika losowego -> test ADF  
4. Sformułowanie hipotez statystycznych:  
	- $H0: \delta=0$  
		- parametr stojący przy zmiennej $Y_{t-1}$ nieistotnie różni się od zera, zmienna $Y_t$ jest niestacjonarna (nie jest zintegrowana lub jest zintegrowana w stopniu większym niż zero).  
	- $H1: \delta < 0$  
		- parametr stojący przy zmiennej $Y_{t-1}$ jest ujemny, zmienna $Y_t$ jest ==stacjonarna== (zintegrowana w stopniu równym zeru).  
5. obliczenie wartości testu DF/ADF  
6. odczytanie wartości z tablic  
	- oznaczenia  
		- >Wartości testu DF są ujemne!  
		- $DF_e$ - wynik z testu DF  
		- $DF_d$ - dolna granica testu DF  
		- $DF_g$ - górna granica testu DF  
	- Wybór  
		- jeżeli $DF_e > DF_g$ - nie ma podstaw do odrzucenia $H_0$, $Y_t$ jest ==niestacjonarna== -> robimy dalej  
		- jeżeli $DF_e < DF_d$ - odrzucamy $H_0$, zmienna $Y_t$ jest ==stacjonarna==  
		- $DF_d < DF_e < DF_g$ - obszar niekonkluzywności testu  
7. odejmujemy $Y_{t-1}$ od równania modelu  
	- formułujemy hipotezy jak w pkt. 4  
	- obliczamy wartości testu jak w pkt. 5  
	- odczytujemy wartości jak w pkt. 6  
		- hipotezy  
			- $H_0: \delta = 0$  
				- parametr stojący przy zmiennej $\Delta Y_{t-1}$ nieistotnie różni się od zera, pierwsze przyrosty $Y_t$ nie są stacjonarne, zmienna nie jest zintegrowana lub jest zintegrowana co najmniej w stopniu drugim.  
			- $H_1: \delta < 0$  
				- parametr stojący przy zmiennej $\Delta Y_{t-1}$ jest ujemny, pierwsze przyrosty zmiennej $Y_t$ są stacjonarne (==zintegrowana w stopniu pierwszym==).  
		- wartość testu  
			- Jeżeli $DF_e > DF_g$, nie ma podstaw do odrzucenia $H_0$, pierwsze przyrosty $Y_t$ nie są stacjonarne, zmienna nie jest zintegrowana lub jest zintegrowana co najmniej w stopniu drugim.  
			- Jeżeli $DF_e < DF_d$, $H_0$ należy odrzucić na rzecz $H_1$, pierwsze przyrosty $Y_t$ są stacjonarne (zmienna $Y_t$ jest zintegrowana w stopniu pierwszym).  
			- Jeżeli $DF_d < DF_e < DF_g$ to przy użyciu testu Dickeya-Fullera nie można podjąć żadnej decyzji (przedział nieokreśloności)  
  
- test Kwiatkowskiego, Phillipsa, Schmidta i Shina (KPSS) – wnioskowanie, hipotezy, statystka teoretyczna  
  
---  
  
### Kointegracja Procesów Stochastycznych I Równowaga Długookresowa  
#### **Przyrostostacjonarność, Trendostacjonarność - definicja**  
  
##### Trendostacjonarność  
- ![](https://i.imgur.com/ytF0vPx.png)  
- Szereg trendostacjonarny jest to taki proces, który staje się stacjonarny po usunięciu trendu deterministycznego, na przykład trendu liniowego postaci $y_t = \alpha_0 + \alpha_1*t +\epsilon_t$, gdzie składnik losowy $\epsilon_t$ jest stacjonarną zmienną losową.  
- Jeśli od obu stron równania odejmiemy trend, czyli wyrażenie $\alpha_0 + \alpha_1*t$, to otrzymany proces będzie stacjonarny, zgodnie z założeniami o składniku losowym.[^28]  
  
##### Przyrostostacjonarność  
- ![](https://i.imgur.com/K4ophiU.png)  
- Szereg przyrostostacjonarny ma postać procesu błądzenia losowego ze stałą, czyli $$y_t = \mu + y_{t-1} + \epsilon_t$$  
- W tym przypadku praktyka wprowadzania zmiennej czasowej w celu usunięcia trendu jest niesłuszna, ponieważ trend kształtowania się zmiennej ulega zmianom w czasie. Taki trend nazywamy stochastycznym.[^29]  
  
#### **Regresja Pozorna – Kiedy Mamy Podejrzenie O Regresję pozorną**  
- Wstępne wnioski na temat występowania regresji pozornej można wyciągnąć na podstawie porównania współczynnika determinacji i statystyki Durbina-Watsona modelu.  
- Jeśli $R^2>DW$, to mamy podstawy spodziewać się efektu regresji pozornej  
- W przypadku regresji pozornej, reszty z modelu liniowego są niestacjonarne i wykazują autokorelację (Statystyka LM)  
  
#### **Procesy Skointegrowane (definicja)**  
- Kointegracja szeregów czasowych występuje wtedy, gdy dwa lub więcej szeregi są niestacjonarne, ale ich liniowa kombinacja jest stacjonarna.  
- Jeśli okaże się, że składnik losowy $\epsilon_t$ (czyli liniowa kombinacja $y_t$ i $x_t$) jest stacjonarny, to zmienne $y_t$ i $x_t$ są skointegrowane.  
- jeśli {$z_t$} ~ I(d) oraz {$v_t$} ~ I(d), mogą one być skointegrowane (ale nie muszą).  
- Równanie $$y_t = \alpha_0 + \alpha_1*x_t + \epsilon_t$$ nazywane jest regresją lub relacją kointegrującą, a parametr $\alpha_1$ parametrem kointegrującym.[^30]  
  
#### Testowanie Koinegracji (wnioskowanie, Hipotezy, Procedura testowa); **Wektor kointegrujący**  
  
- Testowanie kointegracji ma sens wtedy, gdy zmienne występujące w równaniu są zintegrowane oraz może istnieć ich stacjonarna kombinacja liniowa.  
  
- Kointegracja występuje wtedy, gdy dwa lub więcej szeregów są niestacjonarne, ale ich kombinacja liniowa jest stacjonarna  
	- Dwa szeregi czasowe $X_t$, $Y_t$ są skointegrowane rzędu d, b gdzie $d \geq b \geq 0$, co zapisujemy CI(d, b) jeżeli:  
		- oba szeregi są zintegrowane tego samego rzędu d  
		- istnieje kombinacja liniowa tych procesów która jest zintegrowana stopnia d-b  
  
##### Procedura  
  
- Jeżeli zmienna $x_t$ oraz $y_t$ są zintegrowane w stopniu pierwszym to można przejść do kolejnego etapu.  
- oszacowanie modelu dla poziomów wybranych zmiennych, a następnie badanie stacjonarności składnika losowego ($e_t$):  
	- $$e_t = y_t − β_0 − β_1*x_t$$  
  
##### Hipotezy  
- $H_0: e_t ∼ I(1)$  
	- $x_t$ i $y_t$ nie są skointegrowane  
- $H_1: e_t ∼ I(0)$  
	- $x_t$ i $y_t$ są skointegrowane  
  
- Statystyka testu  
	- Statystyka testu jest jest analogiczna jak w przyapdku testu ADF, ale wykorzystuje się inne statystyki testowe.  
  
#### **Jednorównaniowy Model Korekty błędem**; Dwustopniowa Procedura Engle'a-Grangera (**interpretacja**, Cel, budowa)  
  
##### Model Korekty Błędem  
  
- Model ECM należy do klasy modeli dynamicznych. Opisuje sposób, w jaki dokonują się dostosowania zmiennej objaśnianej do relacji długookresowej. Możemy go stosować, jeżeli dwa szeregi czasowe $x_t$ i $y_t$ są niestacjonarne i skointegrowane  
- Niech $x_t ~ I(1)$ oraz $y_t ~ I(1)$ a $y_t - \gamma_0 - \gamma_1 x_t ~ I(0)$ jest relacją kointegrującą, definiującą długookresową zależność między zmiennymi  
- $\Delta y_t = \alpha + \delta[y_{t-1} - \gamma_0 - \gamma_1 x_{t-1} + \sum^q_{i=1} \alpha_i \Delta y_{t--1} + \sum^p_{j=0} \beta_j \Delta x_{t-j} + \epsilon_t$  
  
- część równania związana z parametrem $\delta$ nazywamy mechanizmem korekty błędem (ECM) opisującym powrót systemu do długookresowej równowagi  
- Część równania związana z opóźnieniami zmiennej objaśnianej i zmiennych objaśniających (część ADL) ma na celu odpowiednie odwzorowanie zmienności krótkookresowej badanego zjawiska  
- interpretacja  
	- jeśli $y_{t-1} > \gamma_0 - \gamma_1 x_{t-1}$ oraz $\delta \in (-1;0)$ to $\Delta y_t$ jest ujemne, czyli $y_t$ maleje, dokładnie o fragment $\delta$ nierównowagi z poprzedniego okresu  
  
- Mechanizm ECM opisuje krótkookresowy powrót do stabilnej długookresowej równowagi, danej relacją kointegrującą  
- jeśli $\delta = 0$ to mechanizm jest nieaktywny i równanie opisuje jedynie dynamikę krótkookresową (ADL)  
- dla mechanizmu $ECM$ można wyznaczyć okres połowicznego wygaśnięcia  
	- $$HL = \frac{ln0.5}{ln(1+\delta)}$$  
- Najprostszą metodą estymacji układu ECM jest dwukrokowa metoda Engle’a - Granger’a[^31]  
  
  
  
##### Dwustopniowa Procedura Engle'a-Grangera  
  
###### Procedura  
1. sprawdzamy, czy $y_t \sim I(1)$ oraz $x_t \sim I(1)$  
2. szacujemy MNK parametry relacji kointegrującej $y_t = \gamma_1 x_t + \epsilon_t$  
3. obliczamy reszty $e_t = y_t - \hat{\gamma_t} - \hat{\gamma} x_t$ i testujemy czy są one stacjonarne, $e_t \sim I(0)$  
4. Jeśli reszty są stacjonarne (tzn. oszacowana relacja jest relacją kointegrującą), to reszty można interpretować jako odchylenia od relacji równowagi, co oznacza, że możemy oszacować pełen model ECM:  
	- $$\Delta y_t = \alpha + \delta e_{t-1} + \sum^q_{i=1} \alpha_i \Delta y_{t--1} + \sum^p_{j=0} \beta_j \Delta x_{t-j} + \epsilon_t$$  
- Otrzymujemy w ten sposób parametr kontrolujący siłę mechanizmu (czyli $\delta$) oraz oszacowania odpowiednich parametrów części dynamicznej (czyli $\alpha_i$ oraz $\beta_j$)[^32]  
  
###### Interpretacja  
- Parametr $\delta$ identyfikuje tempo powrotu do równowagi długookresowej[^33]  
	- Wielkość tę interpretujemy następująco: X% odchylenia jest korygowane po upływie jednego okresu[^34]  
  
---  
  
### Jednowymiarowe Modele Zmienności  
  
#### Modele Z Warunkową Heteroskedastyczności – Kiedy I Dlaczego Stosujemy, Wady I Zalety (ARCH, GARCH)  
  
##### ARCH  
###### Zalety:  
- uwzględnianie nieliniowego charakteru kształtowania się danego zjawiska  
- mogą odwzorowywać wiele złożonych zjawisk ekonomicznych, jednocześnie nie wymagają stosowania skomplikowanych metod estymacji  
- możliwość odwzorowywania zjawiska „grupowania wariancji”  
- szerokie zastosowanie głównie w teorii finansów  
###### Problemy I Ograniczenia:  
- problem z doborem wartości q  
- duże wartości q  
- problem z założeniem o nieujemnej wartości wariancji warunkowej  
  
###### Model Autoregresyjny Z Warunkową Heteroskedastycznością (ARCH)  
Dwa równania:  
- równania opisującego warunkową średnią  
- równania opisującego warunkową wariancję  
  
##### GARCH  
###### Wady  
- nie pozwala na uwzględnienie efektu długiej pamięci  
- brak możliwości modelowania efektu dźwigni  
###### Zalety  
- wpływ nietypowych obserwacji na wariancję wygasa w tempie geometrycznym  
- lepszy niż model ARCH do opisów o grubych ogonach  
- stosowany, gdy liczba opóźnień w modelu ARCH jest duża  
  
###### Uogólnienia Modelu ARCH, m.in. GARCH (q, p),  
- W stosunku do ARCH został po prostu wprowadzony w proces autoregresyjny. Jest to analogia uogólnienia modelu MA na ARMA. W tym podejściu zakłada się, że przy opisie kształtowania się logarytmów stóp zwrotu główne równanie procesu może być zapisane jako proces ARMA.  
  
##### Test Engle’a Efektu ARCH (wnioskowanie, Hipotezy, Procedura testowa)  
- Potwierdzenie istnienia efektu ARCH, czyli czy zwroty z danego instrumentu mają własność grupowania wariancji opisane warunkową heteroskedastycznością  
	- H0: parametry są nieistotne (nie występuje efekt ARCH)  
	- H1: parametry są istotne (występuje efekt ARCH)  
- Statystyka Testu:  
	- $LM = TR^2$  
	- T – liczba obserwacji  
	- $R^2$ – współczynnik determinacji dla równania pomocniczego  
- Jeśli obliczona wartość statystyki przekracza wartość krytyczną, hipotezę zerową o braku efektu ARCH należy odrzucić.  
- Jeśli empiryczny poziom istotności statystyki jest mniejszy niż np. 0,05, hipotezę zerową o braku efektu ARCH należy odrzucić.[^35]  
  
  
---  
  
### Hipoteza Rynku Efektywnego  
  
- Teza rozważana w finansach, zgodnie z którą w każdej chwili ceny papierów wartościowych w pełni odzwierciedlają wszystkie informacje dostępne na ich temat.  
- Trzy podstawowe grupy informacji:  
	- związane z emitentem instrumentów finansowych  
	- sektorowe  
	- makroekonomiczne  
  
#### Założenia Hipotezy Rynku Efektywnego; Co Oznacza, Że Rynek Jest Efektywny W Sensie Informacyjnym  
Założenia:  
- Minimalna zmiana cen  
- Skończona liczba dziennych transakcji  
- Cena i wartość wyznacznikiem stopy zwrotu na rynku  
- Wybór papieru wartościowego, który daje szansę większego zysk  
- Mało prawdopodobne transakcje, gdy osiągnięcie zysku nie jest możliwe  
- Inwestorzy potrafią racjonalnie przełożyć wartość na cenę  
- W zawieranych transakcjach obowiązują ceny równowagi  
- Zmiany cenowe są od siebie niezależne  
	- ceny są dostosowane do aktualnie dostępnych informacji  
	- podlegają błądzeniu losowemu  
  
Rynek efektywny w sensie informacyjnym:  
- ogłoszona informacja odbiega od wartości oczekiwanej przez rynek, a wszystkie pozostałe informacje, które były znane lub oczekiwane przez rynek są już zdyskontowane w cenach  
  
#### Implikacje Hipotezy Rynku Efektywnego  
  
##### Rynek Efektywny a Analiza Techniczna  
- Podstawowe założenia analizy technicznej są sprzeczne z hipotezą rynku efektywnego  
- Jeśli rynek jest efektywny w formie słabej to ceny w pełni odzwierciedlają wszystkie informacje rynkowe  
- Analiza techniczna oparta na historycznych danych rynkowych jest bezwartościowa  
  
##### Rynek Efektywny a Analiza Fundamentalna  
- Analiza fundamentalna zakłada, że w każdej chwili możliwe jest określenie wartości wewnętrznej papieru wartościowego, która jest zależna od wpływu szeregu czynników ekonomicznych  
- Decyzje inwestycyjne należy podejmować na podstawie porównania ustalonej wartości wewnętrznej papieru wartościowego z jego bieżącą wartością rynkową  
- Analiza fundamentalna wykorzystuje informacje, których dotyczy hipoteza rynku efektywnego w formie półsilnej  
  
##### Rynek Efektywny a Analiza Makroekonomiczna  
- Na rynku efektywnym analiza makroekonomiczna oparta wyłącznie o dane historyczne nie daje możliwości budowy strategii inwestycyjnej generującej ponadprzeciętne stopy zwrotu  
- Badania empiryczne sugerują występowanie długookresowych trendów cen aktywów, lecz by móc je wykorzystać niezbędna jest zdolność prawidłowego prognozowania przyszłych wartości zmiennych będących źródłem ruchów cen  
  
##### Rynek Efektywny a Zarządzanie Portfelem  
- Liczne testy efektywności rynku w formie silnej wykazują, że większość zarządzających portfelami nie jest w stanie zagwarantować ponadprzeciętnych stóp zwrotu  
  
#### Rynek Efektywny W Sensie Informacyjnym. Formy Efektywności  
  
##### Słaba efektywność(warunki Stosowalności, założenia)  
- Ceny walorów odzwierciedlają wszystkie istotne informacje zawarte w notowaniach historycznych  
- Na podstawie samego ruchu cen w przeszłości, inwestor nie jest w stanie przewidywać przyszłych zmian notowań walorów, aby osiągnąć ponadprzeciętne zyski  
- Nie jest możliwe uzyskanie ponadprzeciętnych zysków z tytułu wykorzystania informacji tkwiących w cenach  
  
##### Średnia Efektywność (warunki Stosowalności, założenia)  
- Ceny papierów wartościowych odzwierciedlają nie tylko wiadomości, które można odczytać z notowań historycznych, ale także wszystkie inne publiczne informacje  
- Brak możliwości osiągania ponadprzeciętnych zysków wyłącznie na podstawie ogólnie dostępnych informacji  
- Dostępne inwestorom informacje zostały już odzwierciedlone w cenach akcji przez działający mechanizm rynkowy  
  
##### Silna Efektywność (warunki Stosowalności, założenia)  
- Zarówno publicznie dostępne dane, jak i wiadomości poufne i prywatne znajdują szybkie odzwierciedlenie w cenach walorów.  
- Nie tylko inwestorzy bazujący na analizach powszechnie dostępnych informacji, ale również gracze, którzy są w posiadaniu informacji poufnych nie są w stanie uzyskać ponadprzeciętnych zysków[^36]  
  
---  
  
### Anomalie Rynku Kapitałowego  
  
#### Podstawowe Efekty Kalendarzowe (warunki, założenia)  
- Związane są z możliwością osiągnięcia ponadprzeciętnej stopy zwrotu w danym okresie czasu. Mogą podważać lub zakłócać hipotezę efektywności – rynek staje nieefektywny w sensie informacyjnym.  
  
#### Przykłady Efektów  
  
- efekt miesiąca w roku (month-of-the year effect)  
	- Np. Stopy zwrotu w styczniu są przeciętnie znacznie wyższe niż w innych miesiącach roku  
- efekt tygodnia w miesiącu (week-of-the month effect)  
- efekt dnia w tygodniu (day-of-the week effect)  
	- Np. poniedziałkowe stopy zwrotu są przeciętnie niższe niż w pozostałych dniach tygodnia  
- efekt godziny w ciągu dnia (hour-of-the day effect)  
	- Np. niższe stopy zwrotu w pierwszej godzinie trwania sesji w poniedziałek, wyższe zaś w pierwszej godzinie trwania sesji w pozostałych dniach[^37]  
  
---  
  
### Literatura  
1. Charemza W., Deadman D.: Nowa ekonometria, Warszawa: PWE, 1997  
2. Kufel T.: Ekonometria. Rozwiązywanie problemów z wykorzystaniem programu GRETL, Warszawa: PWN, 2011  
3. Maddala G.S.: Ekonometria, Warszawa: PWN, 2006  
4. Osińska M.: Ekonometria finansowa: Warszawa: PWE, 2006  
5. Witkowska D., Matuszewska A., Kompa K.: Wprowadzenie do ekonometrii dynamicznej i finansowej, SGGW, Warszawa, 2008  
  
[^1]: w ogólności wariancja może w ogóle nie istnieć  
[^2]: Jajuga (2000), Jondeau i Rockinger (2000), Premaratne i Bera (2001)  
[^3]: [Zastosowanie modeli klasy ARCH do opisu własności szeregu stóp zwrotu indeksu WIG](http://kpiontek.ue.wroc.pl/kp-fiapgarch.pdf)  
[^4]: <http://www.fire.ue.wroc.pl/pracownicy/KPiontek_doktorat.pdf>  
[^5]: Fałdziński, M. (2014). _Teoria wartości ekstremalnych w ekonometrii finansowej_. Wydawnictwo Naukowe Uniwersytetu Mikołaja Kopernika.  
[^6]: Tarczyński, W., Witkowska, D., & Kompa, K. (2013). _Współczynnik beta. Teoria i praktyka_. Pielaszek Research.  
[^7]: <http://www.fire.ue.wroc.pl/pracownicy/KPiontek_doktorat.pdf>  
[^8]: Doman, M., & Doman, R. (2009). _Modelowanie zmienności i ryzyka: metody ekonometrii finansowej_. Oficyna a Wolters Kluwer business.  
[^9]: Prędki, A. (Ed.). (2017). _Narzędzia analityczne w naukach ekonomicznych: Wybrane zastosowania_. Fundacja Uniwersytetu Ekonomicznego w Krakowie.  
[^10]: [Analiza Szeregów Czasowych/Dekompozycja szeregu czasowego](https://el.us.edu.pl/ekonofizyka/index.php/Analiza_Szereg%C3%B3w_Czasowych/Dekompozycja_szeregu_czasowego)  
[^11]: [6.1 The Periodogram  STAT 510](https://online.stat.psu.edu/stat510/lesson/6/6.1)  
[^12]: [Analiza szeregów czasowych](https://www.cs.put.poznan.pl/jstefanowski/aed/TPtimeseries.pdf)  
[^13]: [Analiza Szeregów Czasowych/Dekompozycja szeregu czasowego](https://el.us.edu.pl/ekonofizyka/index.php/Analiza_Szereg%C3%B3w_Czasowych/Dekompozycja_szeregu_czasowego#Metoda_Boxa-Jenkinsa)  
[^14]: Montgomery, D. C., Jennings, C. L., & Kulahci, M. (2015). _Introduction to time series analysis and forecasting_. John Wiley & Sons.  
[^15]: <https://web.sgh.waw.pl/~jmuck/Ekonometria/EkonometriaPrezentacja2018Z_5.pdf>  
[^16]: <https://spureconomics.com/interpreting-acf-and-pacf-plots/>  
[^17]: Wykłady  
[^18]: [Analiza Szeregów Czasowych/Procesy stochastyczne](https://el.us.edu.pl/ekonofizyka/index.php/Analiza_Szereg%C3%B3w_Czasowych/Procesy_stochastyczne#Stacjonarno.C5.9B.C4.87_procesu_stochastycznego)  
[^19]: Gruszczyński, M., Kuszewski, T., & Podgórska, M. (Eds.). (2009). _Ekonometria i badania operacyjne: podręcznik dla studiów licencjackich_. Wydawnictwo Naukowe PWN.  
[^20]: <https://docplayer.pl/docview/92/109881171/#file=/storage/92/109881171/109881171.pdf>  
[^21]: <http://www.ekonometria.wne.uw.edu.pl/uploads/Main/GankoJanaczek.pdf>  
[^22]: Notatki Michała  
[^23]: Notatki Michała  
[^24]: Vogelvang, B. (2005). _Econometrics: theory and applications with Eviews_. Pearson Education.