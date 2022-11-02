---  
tag: books, statistics  
author: W. Makać, A. Balicki  
title: Metody wnioskowania statystycznego  
share: true  
---  
  
# Zdarzenia  
  
- Powtarzalne doświadczenia lub obserwacje nazywać będziemy krótko — doświadczeniami.  
- Różne wyniki możliwe de zrealizowania się w powtarzalnych doświadczeniach nazywamy zdarzeniami, a zdarzenie, które w wyniku przeprowadzonego doświadczenia może zrealizować się lub nie nazywamy zdarzeniem losowym.  
-   
- Pierwotnym pojęciem w rachunku prawdopodobieństwa jest **zdarzenie elementarne**, czyli niepodzielny wynik doświadczenia losowego, realizujący się tylko na jeden sposób.  
	- W odróżnieniu od zdarzeń elementarnych, definiuje się pojęcie **zdarzenia złożonego**, które może realizować się na więcej niż jeden sposobów, czyli może być rozłożone na kilka zdarzeń elementarnych.  
- Zdarzenie odpowiadające zbiorowi pustemu zdarzeń elementarnych nazywamy zdarzeniem niemożliwym (symbol $\emptyset$ lub O).  
	-  Jest to zdarzenie, które w danym doświadczeniu zajść nie może, np. wyrzucenie siedmiu oczek w rzucie kostką, I ma charakter zdarzenia hipotetycznego.  
- O dwóch zdarzeniach, A i B, mówimy, że są **wykluczające się**, jeżeli nie zawierają żadnego wspólnego zdarzenia elementarnego, czyli iloczyn tych dwóch zdarzeń jest zdarzeniem niemożliwym, $A \cap B = \emptyset$. Są to zatem zdarzenia, które **nie mogą realizować się jednocześnie**. W przeciwnym przypadku zdarzenia nie będą się wykluczały.  
- Jeżch zdarzenia A, wykluczają się parami, a ich suma jest zdarzeniem pewnym, to stanowią one **zupełny układ zdarzeń**.   
- Zdarzeniem przeciwnym (dopełnieniem) do zdarzenia A nazywamy zdarzenie $\overline{A}$ (nie-A), składające się z tych wszystkich zdarzeń elementarnych, które nie należą do zdarzenia A, tzn. $\overline{A} = E - A$  
	- Oba te zdarzenia tworzą układ zupełay zdarzeń, tj. $A \cup \overline{A} = E$ oraz $A \cap \overline{A} = \emptyset$  
- Jeżeli zdarzenie B nie ma wpływu na zajście zdarzenia A, to zdarzenie A nazywamy **niezależnym** od zdarzenia B.  
	- Relacja niezależności jest symetryczna, co oznacza, że jeżeli zdarzenie A jest niezależne od B, to i B jest niezależne od A.  
- **Zdarzenia A i B są więc zależne**, jeżeli **prawdopodobieństwo jednego z nich zależy od zajścia** lub niezajścia drugiego zdarzenia.  
	-   
	    
- ## Przestrzeń  
	- Jeżeli chcemy mówić o doświadczeniach w sposób teoretyczny i jednoznaczny, to dla każdego doświadczenia związanego z określonym zespołem warunków należy określić **zbiór zdarzeń elementarnych** lub inaczej przestrzeń próbek E.  
		- Jeżeli przestrzeń próbek zawiera tylko skończoną liczbę zdarzeń slementarmych bądź gdy zawiera ich nieskończenie wiele, ale można je ustawić w pojedynczy ciąg e1, e2, ... (tzw. zbiór przeliczalny), to nazywamy ją **przestrzenią dyskretną** lub skokową.  
		- Przestrzeń próbek może teź być nieprzeliczalna. Nazywamy ja wtedy **przestrzenią ciągłą**.  
	- Gdy zbiór £ jest skończony i zawiera dokladnie m elementów, możemy na nim określić $$2^n = \sum^n_{i=0}\binom{n}{i}$$  
  
# Pojęcie i własności prawdopodobieństwa  
  
- Prawdopodobieństwem zdarzenia A nazywamy iloraz liczby zdarzeń elementarnych n(A) sprzyjających zajściu zdarzenia A do liczby n wszystkich zdarzeń elementarnych  
	- $$P(A) = \frac{n(A)}{n}$$  
	- Jakkolwiek byśmy określili zdarzenie, jest oczywiste, że liczba n(A) musi spełniać nierówność $0 \leq n(A) \leq n$, z czego wynika, że prawdopodobieństwo P(A) jest liczbą wymierną z przedziału <0,1>.  
- Prawdopodobieństwem nazywamy funkcję P odwzorowującą ciało zdarzeń Z w zbiór liczb rzeczywistych, P: Z -> [0,1], posiadającą następujące własności:  
	- Dla każdego zdarzenia A e Z, prawdopodobieństwo P(A) tego zdarzenia spełnia nierówność: $$0 \leq P(A) \leq 1$$  
	-  Prawdopodobieństwo zdarzenia pewnego jest równe jeden: $$P(E) = 1$$  
	- Jeżeli dwa zdarzenia nie wykluczają się, to: $$P(A \cup B) = P(A) + P(B) - P(A \cap B)$$  
- Prawdopodobieństwo warunkowe  
	- Oznaczając symbolem A|B zdarzenie polegające na zajściu zdarzenia A, przy założeniu, że zaszło zdarzenie B, prawdopodobieństwo, zwane warunkowym P(A|B), zapiszemy:  
		- $$P(A|B) = \frac{P(A \cap B)}{P(B)}, \space P(B)>0$$  
		- $$P(B|A) = \frac{P(A \cap B)}{P(A)}, \space P(A)>0$$  
	- Ze wzorów (2.12) t (2.13) wynika, że prawdopodobieństwo łącznego zajścia, tj. iloczynu, zdarzeń A i B jest równe (tzw, twierdzenie o prawdopodobień- stwach złożonych):  
		- $$P(A \cap B) = P(B) * P(A|B) = P(A) * P(B|A)$$  
	- Można więc określić, uwzględniając równość (2.14), warunek wzajemnej nie- zależności zdarzeń A i B w postaci równości  
		- $$P(A \cap B) = P(A) * P(B)$$  
	- Mówimy, że trzy zdarzenia są niezależne parami, jeśli spełnione są równości:  
		- $$P(A \cap B) = P(A) * P(B)$$  
		- $$P(B \cap C) = P(B) * P(C)$$  
		- $$P(A \cap C) = P(A) * P(C)$$  
- Wzór Bayesa  
	- $$P(A_i | B) = \frac{P(A_i)*P(B|A_i)}{\sum^n_{i=1} P(A_1)*P(B|A_i)}$$  
	- Wzór ten nazywany jest też wzorem na prawdopodobieństwa a posteriori (przyczyn), gdyź określa prawdopodobieństwo realizacji zdarzenia A; po nastąpieniu zdarzenia B, w odróżnieniu od prawdopodobieństwa a priori (skutków), którego znajomość — zgodnie z nazwą - zakładamy z góry.