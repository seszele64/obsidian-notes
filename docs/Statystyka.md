---  
tag: books, books/statistics  
title: Statystyka  
author: M. Sobczyk  
share: true  
---  
  
# Rozkłady  
  
- Rozkładem empirycznym zmiennej nazywamy przyporządkowanie kolejnym wartościom zmiennej ($x_i$) odpowiadających im liczebności ($n_i$)  
- Rozkłady  
	- Rozkład, którego krzywa liczebności (dla cechy ciągłej) lub diagram (dla cechy skokowej) ma jedno maksimum, nazywa się rozkładem jednomodalnym. Wśród rozkładów jednomodalnych można wyróżnić **rozkłady symetryczne**, **umiarkowanie asymetryczne** i **skrajnie asymetryczne**. W rozkładzie symetrycznym jednomodalnym liczebnościodpowiadające wartościom zmiennej rozkładają się symetrycznie wokół liczebności największej  
		- Rozkładem symetrycznym o jednym maksimum jest rozkładnormalny  
	- Rozkłady asymetryczne mogą być umiarkowanie asymetryczne i skrajnie asymetryczne, a te z kolei prawoskośne i lewoskośne. Rozkłady asymetryczne charakteryzują się tym, że prostopadła do osi odciętych poprowadzona z punktu maksimum krzywejliczebności dzieli powierzchnię pod krzywą na dwie nierówne części. Jeśli większa powierzchnia wraz z dłuższym „ramieniem” krzywej znajduje się po prawej stronie punktu maksimum, to rozkład jest prawoskośny.  
	- Rozkłady mające tylko jedno „ramię” noszą nazwę skrajnie asymetrycznych. Są one rozkładami jednostronnymi względem wartości cechy o maksymalnej liczebności.  
	- Jeśli krzywa liczebności lub diagram rozkładu ma dwa maksima, to rozkład taki nazywamy bimodalnym. Rozkłady mające więcej niż dwa  maksima lokalne nazywamy wiełomodalnymi  
  
## Opisowe charakterystyki rozkładów  
  
1. miary Średnie (zwane też miarami poziomu wartości zmienej, miarami położenia lub przeciętnymi) służące do określania tej wartości zmiennej opisanej przez rozkład, wokół której skupiają się wszystkie pozostałe wartości zmiennej  
2. miary rozproszenia (zmienności, zróżnicowania, dyspersji) służące do badania stopnia zróżnicowania wartości zmiennej,  
3. miary asymetrii (skośności) służące do badania kierunku zróżnicowania wartości zmiennej  
4. miary koncentracji służące do badania stopnia nierównomierości rozkładu ogólnej sumy wartości zmiennej pomiędzy poszczególne jednostki zbiorowości lub do analizy stopnia skupienia poszczególnych jednostek wokół średniej  
  
# Miary średnie  
  
- Miary średnie dzieli się na dwie grupy:   
	- średnie klasyczne  
		- ## Średnia arytmetyczna,  
			- Średnia arytmetyczna. Średnią arytmetyczną nazywamy sumę wartości zmiennej wszystkich jednostek badanej zbiorowości podzielo- ną przez liczbę tych jednostek  
			- Jeżeli warianty zmiennej występują z różną częstotliwością, to oblicza się Średnią arytmetyczną ważoną.  
				- Wagami są liczebności odpowiadające poszczególnym wariantom  
		- ## Średnia harmoniczna,  
			- Średnia harmoniczna jest odwrotnością Średniej arytmetycznej z odwrotności wartości zmiennych  
				- $$H = \frac{N}{\sum^N_{n=1} \frac{1}{x_i}}$$  
				- Średnią harmoniczną stosuje się wówczas, kiedy wartości zmiennej podane są w jednostkach względnych, np. w km/h, kg/osobę, wagi zaś — w jednostkach występujących w licznikach tych jednostek względnych.  
					- np. prędkość pojazdu (zmienna: w km/h, waga: w km), — gęstość zaludnienia (zmienna: w osobach/km”, waga: w osobach), —- spożycie artykułu X na 1 osobę (zmienna: w kg/osobę, waga: w kg).  
						- Załóżmy, że gęstość zaludnienia dwu 60-tysięcznych miastach wynosiła odpowiednio: 400 osób/km^2 i 600 osób/km^2. Jaka była przeciętna gęstość zaludnienia obu tych miast?  
							- $H = \frac{2}{1/400 + 1/600} = 2400/5 = 480$ osób/km^2  
		- ## Średnia geometryczna  
			- Średnia geometryczna jest pierwiastkiem n-tego stopnia z iloczynu n wartości danej zmiennej  
			-   
	- pozycyjne  
		- dominanta (modalna, wartość najczęstsza)  
			- Dominanta (modalna, wartość najczęstsza). Dominantq nazywamy taką wartość zmiennej, która w danym rozkładzie empirycznym występuje najczęściej. Wynika z tego, że wartość dominanty można ustalić jedynie z rozkładów jednomodalnych.  
		- kwantyle.  
			- kwartyle (dzielące zbiorowość na cztery części),  
				- kwartyl pierwszy  
				- kwartyl drugi (mediana)  
					- W przypadku szeregów wyliczających, składających się z reguły z niewielkiej liczby jednostek, medianę oblicza się najczęściej za pomocą wzoru  
						- $Me = \frac{x_{N+1}}{2}$, gdy N jest nieparzyste  
						- $Me = \frac{1}{2} * (x_{N/2} + x_{N/2+1})$, gdy N jest parzyste  
						-   
			- kwintyle (na pięć części), decyle (nadziesięć części)   
			- centyle, zwane też percentylami (na sto części)  
				- Centyli jest 99, a pięćdziesiąty centyl jest równy medianie. Na przykład 39 centyl jest taką wartością, że 0,39 wszystkich jednostek badanej zbiorowości ma wartości od niej niższe, a 0,61 jednostek — wartości wyższe.  
  
- w przypadku rozkładu umiarkowanie asymetrycznego zachodzi między nimi następujący związek:  
	- $$\bar{x} - D = 3*(\bar{x} - Me)$$  
		- gdzie $D$ - dominanta, $\bar{x}$ - średnia, $Me$ - mediana  
  
# Miary zmienności  
  
- Dyspersją (rozproszeniem) nazywamy zróżnicowanie jednostek zbiorowości statystycznej ze względu na wartość badanej cechy. Siłę ż dyspersji oceniamy za pomocą pozycyjnych i klasycznych miar zmienności. Do miar pozycyjnych należą: em- piryczny obszar zmienności (zwany też rozstępem lub amplitudą wahań) oraz odchylenie ćwiartkowe.  
  
- Grupę miar klasycznych tworzą: od- chylenie standardowe, wariancja oraz odchylenie przeciętne. Do miar zmienności załiczamy również. współczynnik zmienności, który — w zależności od techniki obliczania — może być klasyczną lub pozycyjną miarą dyspersji.  
	- Miary zmienności można również podzielić na   
		- **bezwzględne** (absolutne)  
			- Empiryczny obszar zmienności jest różnicą między największą i najmniejszą wartością zmiennej w badanej zbiorowości:  
				- $R = x_{max} - x_{min}$  
			- Odchylenie przeciętne określa, o ile wszystkie jednostki danej zbiorowości różnią się Średnio ze względu na wartość zmiennej odśredniej arytmetycznej tej zmiennej.  
				- $d = \frac{1}{N} * \sum^N_{i=1}|x_i - \bar{x}|$  
			- Odchylenie ćwiartkowe Q  
				- $$Q = \frac{Q_3 - Q_1}{2}$$  
			- Wariancja to średnia arytmetyczna z kwadratów odchyleń poszczególnych wartości cechy od średniej arytmetycznej całej zbiorowości  
				- $$s^2 = \frac{1}{N}\sum^N_{t=1}(x_i - \bar{x})^2$$  
			- **typowy obszar zmienności**  
				- $$\bar{x} - s < x_{typ} < \bar{x} + s$$  
			- pomiędzy odchyleniami: ćwiartkowym,  przeciętnym i standardowym zachodzi relacja:  
				- $Q < d < s$  
			-   
		- **względne** (relatywne)  
			- współczynnik zmienności  
				- Względną miarą dyspersji jest współczynnik zmienności, wyrażany w procentach. Służy on do porównywania zmienności cech mierzonych w różnych jednostkach, a także do porównywania kilku zbiorowości pód względem tej samej cechy, ale będącej na różnym poziomie (pkreślonym średnią arytmetyczną lub inną miarą średnią).  
				- Współczynnik zmienności jest ilorazem bezwzględnej miary dyspersjii odpowiednich wartości średnich. Jest on wyrażony w procentach. Ponieważ w analizie rozkładu wartości cechy korzystamy 4 różnych miar zróżnicowania i różnych miar przeciętnych, można obliczać współczynniki zmienności kilkoma metodami  
					- $$V_s = \frac{s}{\bar{x}} * 100$$  
					- $$V_d = \frac{d}{\bar{x}} * 100$$  
					- $$V_Q = \frac{Q}{Me} * 100$$  
					- $$V_{Q_1Q_3} = \frac{Q_3 - Q_1}{Q_3 + Q_1}$$  
  
# Miary asymetrii  
  
- wskaźnik asymetrii  
	- wzór  
		- $$W_s = \bar{x} - D$$  
		- $As = \frac{\bar{x} - D}{s}$  
		- $As = {\bar{x} - D}{d}$  
		- $As = \frac{Q_3 + Q_1 - 2*Me}{Q_3 - Q_1}$  
	- Wartości współczynników asymetrii.z reguły zawierają się w granicach <-1, +1>  
	- dla rozkładu symetrycznego $\bar{x} = D$ ^vreyki  
	- dla asymetrii lewostronnej wskaźnik asymetrii jest ujemny $\bar{x} < D$ ^qqnkcl  
	- dla asymetrii prawostronnej wskaźnik asymetrii jest dodatni $\bar{x} > D$ ^cc7zzo  
  
- asymetria lewostronna  
	- $\bar{x} > Me > D$  
	- ![M. Sobczyk - Statystyka, 2 . rozdział - Opisowa analiza struktury zjawisk masowych > ^qqnkcl](M.%20Sobczyk%20-%20Statystyka,%202%20.%20rozdzia%C5%82%20-%20Opisowa%20analiza%20struktury%20zjawisk%20masowych#%5Eqqnkcl)  
	- $(Q_3 - Q_2) - (Q_2 - Q_1) < 0$  
- asymetria prawostronna  
	- $\bar{x} < Me < D$  
	- ![M. Sobczyk - Statystyka, 2 . rozdział - Opisowa analiza struktury zjawisk masowych > ^cc7zzo](M.%20Sobczyk%20-%20Statystyka,%202%20.%20rozdzia%C5%82%20-%20Opisowa%20analiza%20struktury%20zjawisk%20masowych#%5Ecc7zzo)  
	- $(Q_3 - Q_2) - (Q_2 - Q_1) > 0$  
- rozkład symetryczny  
	- $\bar{x} = D = Me$  
	- ![M. Sobczyk - Statystyka, 2 . rozdział - Opisowa analiza struktury zjawisk masowych > ^vreyki](M.%20Sobczyk%20-%20Statystyka,%202%20.%20rozdzia%C5%82%20-%20Opisowa%20analiza%20struktury%20zjawisk%20masowych#%5Evreyki)  
  
