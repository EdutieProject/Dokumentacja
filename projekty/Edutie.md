# Edutie - e-learning przyszłości
> [Dowiedz się więcej na stronie Edutie](https://edutie.nowanauka.pl)

Edutie to platforma e-learningowa która odzwierciedla koncept Nowej Nauki w postaci e-learningu. Platforma projektowana jest z myślą o spersonalizowanej nauce, jak i sprawieniu żeby uczniowie byli bardziej zainteresowani nauką.

## Profil ucznia i parametry nauki

**Profil ucznia** (nazywany również ***profilem nauczania***) to profil przypisywany użytkownikom platformy mający na celu zbieranie informacji na ich temat w celu optymalizowania procesu nauczania. Jest to **rdzeń** Edutie - na jego podstawie działa personalizacja. Dzieli się on obecnie na trzy części:
 - Cechy ucznia
 - Parametry nauczania
 - Historia nauczania

### Cechy ucznia
Można powiedzieć że są to *fizyczne* właściwości ucznia, które są prawdziwe i znajdują urzeczywistnienie w realnym świecie. Mieści się w to między innymi data urodzenia, klasa do której obecnie uczeń uczęszcza czy również rodzaj szkoły (technikum/liceum). Cechy te wpływają na sposób uczenia - przyjmujemy, że jest on zależny od wieku.

### Parametry nauczania
Parametry nauczania są odzwierciedleniem psychologicznych modeli ([zobacz model Cattella-Horna-Carrolla](../koncept/PsychologiaEdukacji.md)) mówiących między innymi o deterministyczności rozumienia wiedzy przez uczniów. Zadaniem parametrów jest usystematyzowanie sposobu śledzenia predyspozycji i inteligencji ucznia. Robimy to za pomocą przypisywania parametrów jako liczb zmiennoprzecinkowych do poszczególnych cech poznawczych.

### Historia nauczania
Historia nauczania jest zbiorem dotychczasowych wyników ucznia uzyskanych na platformie. Wraz z każdym zadaniem czy czynnością naukową w historii umieszczamy "blok" dokumentujący osiągnięcia ucznia w danym temacie. Zadaniem historii nauczania jest śledzenie:
 - **spełniania wymagań dotyczących materiału na przestrzeni czasu** (progres pod względem wiedzy)
 - **progresu w kwestii rozwoju kompetencji poznawczych** (informowanie ucznia o progresie)
 - **aktywności na platformie i jej rozłożenia w czasie** (pomoc w kwestii przydzielania powtórek) 

> Profil ucznia jako **rdzeń Nowej Nauki** w przyszłości może zostać wyekstraktowany do mikroserwisu, z którego będą mogły korzystać inne aplikacje.

## Program nauczania

Program nauczania w Edutie bazowany jest na strukturze drzewa. Idea stosowania tego typu programu bazuje na upewnianiu się, że uczeń dobrze zrozumiał temat podrzędny zanim przejdzie do tematów nadrzędnych tj. wymagających znajomości podrzędnego. Co za tym idzie, konieczne jest wykorzystywanie maksym **mastery learning'u** aby osiągnąć zamierzany efekt. 
```
     1       Temat pierwszy jest podrzędny
    / \
   2   3     Tematy 2 i 3 są nadrzędne
```
Struktura programu nauczania w Edutie jest podwójnie zagnieżdżonym drzewem, tj. drzewem, którego każdy wierzchołek zawiera w sobie drzewo. Oto hierarchia:
 1. Nauka
 2. Kurs
 3. Lekcje
 4. Segmenty lekcji (zagadnienia)

**Nauka** funkcjonuje jako kategoria przypisywana każdemu kursowi. Może być to np. fizyka, matematyka czy chemia.

**Kursy** są wydzielonym drzewem lekcji dotyczącym danego zakresu materiału. Zakres materiału powinien zawierać jeden "dział" np. może być to *Termodynamika*
 
**Lekcje** są poświęcone na zrozumienie pojedynczego zagadnienia z danego działu. Czas poświęcany na jedną lekcję powinien wynosić około **1 godziny**. Przykładem może być np. *Pierwsza zasada termodynamiki*

**Segmenty lekcji** są elementarnymi zagadnieniami poruszanymi w ramach lekcji. Przykładem może być np. *Układ termodynamiczny* albo *Energia i ciepło w układzie termodynamicznym*

Program nauczania zakłada, że uczeń powinien dobrze zrozumieć temat podrzędny zanim przejdzie do tematów nadrzędnych. Powodem jest to, że gdy uczeń z niepełnym rozumieniem tematu podrzędnego przystąpi do budowania wiedzy z tematów nadrzędnych, będzie on miał niepełne podstawy; może to skutkować złym zrozumieniem tematów nadrzędnych.

#### Segmenty lekcji - zawartość

Zawartością segmentów lekcji są zadania *(w kodzie aplikacji nazywane "learning resource")*. Każdy segment jest wprawdzie **listą zadań**. Uczeń aby *przejść* segment musi zaliczyć jedno z nich. Zadania zgrupowane za pomocą jednego segmentu lekcji mają tą samą tematykę oraz te same wymagania. Z założenia powinny one również dotyczyć tych samych zdolności kognitywnych. Każde zadanie jest również *optymalizowane* (patrz: [personalizacja](#personalizacja))

## Materiały do nauki i ich personalizacja

> **⚠ TODO**: uporządkować: segmenty i zadania

### Zadania

Zadania są elementarnym fragmentem Edutie. Można powiedzieć, że całe Edutie to w **dużym** uproszczeniu elastyczny i unowocześniony wielofunkcyjny zbiór zadań.

#### Struktura zadań

Zadania są oparte o samodzielną pracę. W tworzeniu zadań wykorzystujemy schematy popularne w świecie akademickim, które wykorzystują **higher-order learning**. Przykładem mogą być tu: *Case studies, Experimental learning, Project-based learning* czy *Problem-based learning*.

> **⚠ TODO**: Lista typów zadań

#### Zawartość zadań

 - Opis: Zadania zawierają w sobie spersonalizowany opis zagadnienia którego dotyczą. Mogą być w nim zawarte przykłady i porównania, analogie etc. Ważne aby dobrze wyjaśniały temat.
 - Zadanie: Część zadania która zawiera problem który uczeń ma rozwiązać.
 - Flowchart (opcjonalnie): Schemat przedstawiający przykładowy sposób podejścia do zagadnienia

> **⚠ TODO**: Lista możliwego dodatkowego kontentu dla zadań

#### Rozwiązywanie zadań

Uczeń rozwiązuje zadania samemu - rozwiązanie zadania jest w mniemaniu Nowej Nauki tylko skutkiem ubocznym nauki. Efektem na którym nam zależy jest myślenie  - zastosowanie tego co uczeń już potrafi wraz z przerobieniem kolejnej dawki wiedzy zawartej w opisie zadania. Dlatego formą rozwiązania jest **sprawozdanie** w którym uczeń opisuje swój tok myślenia i drogę jakiej użył by dojść do rozwiązania.

Konieczne jest zastosowanie szablonów sprawozdania i poinformowanie ucznia, o tym co powinno zawierać sprawozdanie.

### Personalizacja

Zadania są personalizowane przy użyciu ***profilu nauczania*** uczniów. Uczniowie przy wybieraniu z dostępnych zadań mogą:
 - Skorzystać z selekcji zadań - czyli wybrać dostępne już zadanie z optymalizacją najlepiej pasującą do jego profilu nauczania.
 - Stworzyć dedykowane zadanie - czyli przy pomocy AI dynamicznie wygenerować zadanie spersonalizowane pod jego profil nauczania. Te zadania następnie są dostępne w puli zadań dostępnych do selekcji.

### Dodatkowa zawartość segmentów

1. Źródła - Aby ułatwić uczniom zrozumienie w segmencie zawieramy odnośniki do zewnętrznych źródeł naukowych tj. wikipedia, youtube albo innych. Są to oczywiście źródła związane z tematem poruszanym przez segment.
2. Umiejętności - zbiór umiejętności których dotyczy temat poruszany przez segment. Na ich podstawie dokonujemy adaptacji profilu nauczania.
3. Wymagania - zbiór wymagań określających wiedzę jaką uczeń powinien przyswoić poprzez wykonanie zadania. Na ich podstawie dokonujemy oceny zadań (zgodnie z [*mastery learning*]()) i przygotowujemy feedback.

## Nawigacja nauki

Nawigacja nauki to wskazywanie uczniowi które z zagadnień najlepiej byłoby mu w danym momencie zrobić. Jest wiele sposobów na nawigowanie ucznia po materiale, i wiele kryteriów które można do tego przyjąć.

Edutie swoją definicją programu nauczania narzuca dwa rodzaje nawigacji:
 - Nawigację przez segmenty (opcjonalnie również lekcje)
 - Nawigację przez zadania

Dla powyższych precyzujemy sposoby nawigacji:
 - Nawigowanie do najbardziej dopasowanego elementu
 
 Zdatne do działania na poziomie zarówno segmentów jak i zadań, wskazywanie uczniowi najlepszego - najbardziej dopasowanego zadania/segmentu bazując na profilu nauczania.

 - Wskazywanie wyzwań

 Zdatne do działania na poziomie zadań, wskazuje zadania które nie są do końca dopasowane do parametrów nauczania ucznia lub zadania których tematyka skorelowana jest ze słabymi wynikami ze strony ucznia.

 - Sugerowanie powtórek

Zdatne do działania na poziomie segmentów, wskazywanie uczniowi dawno nieporuszanego tematu, na który potencjalnie może się natknąć w najbliższej nauce.

## Ocenianie i feedback

Ocenianie i feedback są jednym z kluczowych elementów aplikacji. Jest to fragment odpowiedzialny za dostosowanie profilu nauczania po każdym wykonanym zadaniu oraz za zapewnienie uczniowi odpowiedniego feedbacku.

Ocenianie jest niezależne od optymalizacji (personalizacji) zadań. Oceniając odnosimy się tylko do wymagań zawartych w segmencie i nie bierzemy pod uwagę optymalizacji.

### Podejście technologiczne do oceniania

Ocenianie zadań możliwe jest poprzez wykorzystanie modeli językowych sztucznej inteligencji w celu analizy tekstu sprawozdania. W zautomatyzowanym procesie AI wystawia uczniowi oceny. Jednak aby skonstruować zautomatyzowany system oceniania potrzebne jest odtworzenie **flow** które towarzyszy nauczycielom, z którego następnie powstaje **algorytm**.

> **⚠ TODO**: sprecyzować ocenianie

### Feedback

Feedback jest generowany automatycznie przez AI. Jest on ściśle powiązany z ocenianiem - *dlatego narazie go nie ma.*

> **⚠ TODO**: sprecyzować system feedbacku