# Edutie - e-learning przyszłości
> [Odwiedź stronę Edutie](https://edutie.nowanauka.pl)

Edutie to platforma e-learningowa która odzwierciedla koncept Nowej Nauki w postaci e-learningu. Platforma projektowana jest z myślą o spersonalizowanej nauce, jak i sprawieniu żeby uczniowie byli bardziej zainteresowani nauką.

## Profil nauczania

**Profil ucznia** (nazywany również ***profilem nauczania***) to profil przypisywany użytkownikom platformy mający na celu zbieranie informacji na ich temat w celu optymalizowania procesu nauczania. Jest to **rdzeń** Edutie - na jego podstawie działa personalizacja. Dzieli się on obecnie na trzy części:
 - Cechy ucznia
 - Parametry nauczania
 - Historia nauczania

### Cechy ucznia
Można powiedzieć że są to *fizyczne* właściwości ucznia, które są prawdziwe i znajdują urzeczywistnienie w realnym świecie. Mieści się w to między innymi data urodzenia, klasa do której obecnie uczeń uczęszcza czy również rodzaj szkoły (technikum/liceum). Zakładamy, że te cechy są istotne w przypadku dopasowywania procesu nauczania do ucznia.

### Parametry nauczania
Parametry nauczania są odzwierciedleniem psychologicznych modeli ([zobacz model Cattella-Horna-Carrolla](../koncept/PsychologiaEdukacji.md)) mówiących między innymi o deterministyczności rozumienia wiedzy przez uczniów. Zadaniem parametrów jest usystematyzowanie sposobu śledzenia predyspozycji i inteligencji ucznia. Robimy to za pomocą przypisywania parametrów jako liczb zmiennoprzecinkowych do poszczególnych cech poznawczych.

Parametry nauczania wraz z cechami ucznia są kluczowe w [optymalizacji](#personalizacja) procesu nauczania

### Historia nauczania
Zadaniem historii nauczania jest śledzenie progresu ucznia. Możemy określić dwa sposoby:
 - Śledzenie postępów kognitywnych
 - Śledzenie postępów w materiale

**Śledzenie postępów kognitywnych** określa nam zmiany w parametrach nauczania dokonywane w czasie oraz zależności między nimi.  `Przykład: uczniowi w miesiącu X dobrze idzie nauka przy użyciu parametru P1, a słabo używając parametru P2.` *Możemy śledzić przebieg nauki wraz ze zmianami parametrów, czyli to jakie wyniki uzyskuje uczeń przy wykorzystaniu P1, P2 lub ich jednoczesnym używaniu.*

**Śledzenie postępów w materiale** określa nam spełnianie wymagań dotyczących nauczania na przestrzeni czasu. `Przykład: Uczeń najpierw dostaje słabe oceny z tematu X, przy następnym podejściu dostaje lepszą ocenę.` *Możemy wykorzystać wiedzę o tym, jak zmieniała się ocena wraz z parametrami nauczania*

Historia nauczania jest kluczowa w przypadku [nawigacji](#nawigacja-nauki)

*Profil ucznia powinien być niezależny tj. odnosić się tylko do ucznia, będąc tym samym agnostycznym od wykonanych zadań. W praktyce oznacza to, że wykonana nauka jedynie modyfikuje profil ucznia (jego parametry), a sam profil "nie wie" o tym że konkretne zadanie wpłynęło na jego modyfikacje. Wyjątek stanowi śledzenie postępów w materiale.*

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
 4. Segmenty lekcji

**Nauka** funkcjonuje jako kategoria przypisywana każdemu kursowi. Może być to np. fizyka, matematyka czy chemia.

**Kursy** są wydzielonym drzewem lekcji dotyczącym danego zakresu materiału. Zakres materiału powinien zawierać jeden "dział" np. może być to *Termodynamika*
 
**Lekcje** są poświęcone na zrozumienie pojedynczego zagadnienia z danego działu. Czas poświęcany na jedną lekcję powinien wynosić około **1 godziny**. Przykładem może być np. *Pierwsza zasada termodynamiki*

**Segmenty lekcji** są elementarnymi zagadnieniami poruszanymi w ramach lekcji. Przykładem może być np. *Układ termodynamiczny* albo *Energia i ciepło w układzie termodynamicznym* Zawierają one zadania.

Program nauczania zakłada, że uczeń powinien dobrze zrozumieć temat podrzędny zanim przejdzie do tematów nadrzędnych. Powodem jest to, że gdy uczeń z niepełnym rozumieniem tematu podrzędnego przystąpi do budowania wiedzy z tematów nadrzędnych, będzie on miał niepełne podstawy; może to skutkować złym zrozumieniem tematów nadrzędnych.

# Segmenty lekcji
#### Czym jest?
Segment jest zbiorem zadań dotyczących konkretnego tematu wymagającego danych umiejętności. Aby przejść z segmentu podrzędnego do nadrzędnego uczeń musi wykonać pewną ilość zadań segmentu podrzędnego z dostatecznie dobrą oceną. Można powiedzieć że segment jako zbiór zadań zawiera *propozycje sposobów* na naukę danego materiału. 

#### Za co odpowiada?
Segment lekcji określa:
 - **Tematykę** - czyli czego będą dotyczyć materiały zebrane w tym segmencie
 - **Umiejętności** - czyli jakie umiejętności są skorelowane z tematyką segmentu
 - **Wymagania** - czyli co uczeń powinien wynieść z danego segmentu

Segment lekcji zawiera informacje związane ze specyfiką materiału, które następnie są wykorzystywane w tworzeniu materiałów do nauki. Możnaby przedstawić proces w ten sposób:
```
   Segment lekcji + Profil nauczania = Materiały do nauki
```
Gdzie *materiały do nauki* są zadaniami, znanymi również jako *Learning Resource*.

Ilość zadań wymaganych do przejścia ustalana jest odgórnie poprzez segment (dla aktualnej wersji jest to domyślnie 1), po czym nakładana jest na tą ilość korekta poprzez ***profil ucznia***, aby zmniejszyć lub zwiększyć ilośc wymaganych zadań personalizując proces nauki.

Każde zadanie jest również *optymalizowane* (patrz: [personalizacja](#personalizacja)). Personalizacja dotyczy zawarcia w treści lub opisie zadania wskazówek dobranych do danego profilu ucznia. Wskazówki mogą być wcielone w tekst lub przedstawione osobno jako dodatek do tekstu.

## Materiały do nauki - zadania

### Zadania

Zadania są elementarnym fragmentem Edutie. Można powiedzieć, że całe Edutie to w **dużym** uproszczeniu elastyczny i unowocześniony wielofunkcyjny zbiór zadań.

#### Struktura zadań

Zadania są oparte o samodzielną pracę. W tworzeniu zadań wykorzystujemy schematy popularne w świecie akademickim, które wykorzystują **higher-order learning**. Przykładem mogą być tu: *Case studies, Experimental learning, Project-based learning* czy *Problem-based learning*.

> **⚠ TODO**: Lista typów zadań

#### Zawartość zadań

 - Opis: Zadania zawierają w sobie spersonalizowany opis zagadnienia którego dotyczą i jego możliwego wykorzystania w zadaniu. Mogą być w nim zawarte przykłady i porównania, analogie etc. Ważne aby dobrze wyjaśniały temat.
 - Zadanie - treść: Część zadania która zawiera problem który uczeń ma rozwiązać.
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