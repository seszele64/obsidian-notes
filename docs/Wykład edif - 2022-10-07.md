---  
share: true  
tags:  
- wykład  
- ue/semestr-i  
---  
  
  
# Stacjonarność  
  
- definicja  
	- A simple definition of a stationary process is the following: a process is stationary if for all possible lags, k, the distribution of $y_t, y_{t+1},..., y_{t+k}$, does not depend on t.[^2]  
  
- Statistical tests for stationarity often come down to the question of whether there is a unit root—that is, whether 1 is a solution of the process’s **characteristic equation**  
	-   
  
  
- ściśle zwiazane z szeregami czasowymi  
	- w procesach stochastycznych - funkcja losowa dla argumentu t, $y_t$  
- dane panelowe też mogą być stacjonarne  
- nie badamy stacjonarności w danych przekrojowych  
	- $y_i$ - dane przekrojowe  
- występuje gdy jego podstawowe charakterystyki średnia i wariancja nie zmieniają się w czasie, a kowariancje zależą tylko od odległości między obserwacjami  
	- kowariancje  
		- obserwacje obok siebie mają podobną wartość, wartość zależy od odległości  
- w przypadku kmnk estymator jest obciążony, dlatego dane heteroskedastyczne są niereprezentatywne  
  
## Kiedy  
- proces stochastyczny nigdy nie jest ==ściśle stacjonarny==  
	- dlatego badamy **słabą stacjonarność**  
			- warunki występowania słabej stacjonarności  
				1. wartość oczekiwana jest stała w czasie  
				2. wariancja jest stała w czasie i skończona  
				3. kowariancja między okresami zależy od odległości pomiedzy nimi, a nie od wyboru konkretnego momentu w czasie  
					- ~stałość kowariancji  
			- będziemy stosować test ADF i KPSS  
  
- stopień zintegrowania szeregu, i tak musimy zbadać poziom zintegrowania  
	- I(0) - stacjonarność  
	- I(1) - niestacjonarność  
  
- pierwsze różnice  
	- sprowadzanie szeregu niestacjonarnego do postaci niestacjonarnej, w praktyce bada się do max 2 różnic (zintegrowany w stopniu drugim)  
  
- możemy wyróżnić procesy  
	- biały szum  
		- proces stacjonarny  
		- wartość oczekiwana = 0  
		- wariancja skończona $< \infty$  
		- kowariancja = 0, ~brak **autokorelacji**  
	- random walk  
	- autoregresja  
  
## random walk  
- niestacjonarny  
	- $y_t = y_{t-1}+e$  
	- $e_t$ jest zmienną losową o stałych parametrach  
- $var(y_t)=t \sigma^2$  
- sprowadzenie do stacjonarności polega na odjęciu skumulowanych (zwielokrotnionych) reszt  
  
### random walk with drift  
- randon walk + trend  
	- $y_t = y_{t-1} + T + e_t$  
- szereg niestacjonarny  
- wartość oczekiwana  
	- $t * T$  
- acf  
	- lekko opadający od samego początku  
	- powoli malejący  
- pacf  
	- klif po kilku (1; 2)  
  
## Proces autoregresyjny  
- zbiór zmiennych objaśniających, które również występują jako zmienne objaśniane  
- AR(1): $y_t = \rho_1 * Y_{t-1} + \epsilon_t$  
	- jest stacjonarny, gdy -1<$\rho$<1  
	- niestacjonarny, gdy równy -1 lub 1  
- rzeczy, które daje na #egzamin  
	- czy to jest proces stacjonarny czy nie  
	- jaki proces jest stacjonarny  
  
### proces autoregresyjny vs random walk  
- z czasem mniejsze znaczenie zakłóceń  
- w random walk wszystkie zakłócenia są równie ważne (?)  
  
## stopień integracji szeregu $Y_t$  
- szereg stacjonarny to inaczej szereg zintegrowany w stopniu I(0)  
- jeżeli wymaga różnicowania pierwszego stopnia to zintegrowany w stopniu 1  
- jeżeli wymaga różnicowania drugiego stopnia to zintegrowany w stopniu 2  
  
## badanie stacjonarności  
- test pierwiastka jednostkowego  
- niestacjonarny szereg > zintegrowany w stopniu wyższym niż 0  
- $Y_t = \beta_1*Y_{t-1} + \xi_t$  
- H0: $\beta_1 = 1$  
- H1: $\beta_1 < 1$  
	- prawdziwość h0 - zmienne w równaniu są niestacjonarne  
  
- test df nie może być stosowany dla modeli z autokorelacją składnika losowego, stosuje się wtedy test adf  
  
  
### Test ADF (Augmented Dickey–Fuller) #todo [^1]  
- tests the null hypothesis that a unit root is present in a time series sample  
- allows for higher-order autoregressive processes by including $Δy_{t−p}$ in the model  
  
  
  
  
### etapy testu adf  
...  
  
1. d  
2. d  
3. d  
4. d  
5. hipoteza  
6. odczytanie z tablic  
7. d  
8. d  
9. d  
  
- p value wysokie, test ujemny małe prawdopodobieństwo odrzucenia hipotezy o stacjonarności  
  
  
# Inne  
  
- korelogram dla zmiennych niestacjonarnych  
	- acf powoli spada  
	- pacf klif  
  
  
  
  
# Pytania  
- nieskończona wariancja  
  
[^1]: [5.3 Dickey-Fuller and Augmented Dickey-Fuller tests  Applied Time Series Analysis for Fisheries and Environmental Sciences](https://atsa-es.github.io/atsa-labs/sec-boxjenkins-aug-dickey-fuller.html)  
[^2]: Nielsen, A., 2019. Practical time series analysis: prediction with statistics and machine learning. O’Reilly Media, Inc, Sebastopol, CA.