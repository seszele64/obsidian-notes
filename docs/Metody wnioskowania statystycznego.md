---  
tag: books, statistics  
author: W. Makać, A. Balicki  
title: Metody wnioskowania statystycznego  
share: true  
---  
  
  
# Rozkłady typu skokowego  
  
## Rozkład zero-jedynkowy  
- Zmienna losowa X ma rozkład dwupunktowy, jeżeli przyjmuje z dodatnim prawdopodobieństwem jedynie dwie wartości $x_1$, i $x_2$, przy czym funkcja rozkładu prawdopodobieństwa ma postać:  
	- $P(X = x_1) = p$  
	- $P(X = x_2) = 1 - p = q$  
- $x_1 = 1$ określa się jako zdarzenie wyróżnione (sukces), a $x_2 = 0$ jako zdarzenie przeciwne (porażka)  
	- funkcja prawdopodobieństwa:  
		- $P(X=1) = p$  
		- $P(X=0) = 1 - p = q$  
	- charakterystyki rozkładu  
		- $\mu = p$  
		- $\sigma^2 = pq$  
		- $$\gamma_1 = \frac{1-2p}{\sqrt{pq}}$$  
  
## Rozkład dwumianowy (Bernoulliego)  
- Rozkład dwumianowy jest oparty na następującym schemacie doświadczalnym Bernoulliego  
	- Wykonujemy ciąg n identycznych doświadczeń losowych.  
	- Kolejne doświadczenia są niezależne  
	- Wynikiem każdego doświadczenia mogą być dwa wzajemnie wykluczające się zdarzenia, z których jedno nazywamy sukcesem (A), drugie zaś — porażką ($\overline{A}$)  
	- Prawdopodobieństwo sukcesu p pozostaje stałe w każdym kolejnym doświadczeniu, podobnie jak prawdopodobieństwo $1 — p = q$ porażki.  
- Zmienną losową X w próbach Bernoulliego jest liczba k sukcesów w n wykonanych doświadczeniach, gdzie k = O, 1, 2, ..., n.  
- Równość X = k oznacza, że w wyniku **n doświadczeń** zdarzenie A zrealizowało się dokładnie **k-razy**  
	- $$P(X = k) = \binom{n}{k}*p^k*q^{n-k}, \space k = 0,1,2, \dots, n$$  
		- $p^k * q^{n-k}$ jest prawdopodobieństwem jakiejkolwiek sekwencji k sukcesów (i n — k porażek) w n doświadczeniach  
	- $$q=1-p$$  
	- $$\binom{n}{k} = \frac{n!}{k!(n-k)!}$$  
		- jest liczbą kombinacji bez powtórzeń, która określa liczbę różnych sekwencji w nm doświadcze- niach, w których realizuje się dokładnie k sukcesów.  
  
  
# Rozkład Poissona i jednorodny strumień zdarzeń  
