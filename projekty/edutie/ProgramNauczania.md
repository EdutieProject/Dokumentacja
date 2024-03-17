# Program nauczania

W tym pliku poruszona jest kwestia programu nauczania w aplikacji. Jest to zagadnienie bardziej niezależne od reszty zagadnień pojawiających się w Edutie, dlatego mało będzie tu odnośników do innych plików dokumentacji.

### Spis treści:
1. Problemy z podręcznikami
2. Organizacja tematów w drzewka - ich zalety jak i wady.
3. Struktura programu nauczania w Edutie
   - Nauka
   - Kurs
   - Lekcja
   - Segment
4. Personalizacja nauki w programie nauczania


## Problemy tradycyjnych podręczników

Ten krótki paragraf będzie dotyczyć problemów dotyczących tradycyjnego rozmieszczenia informacji znanego z podręczników i innych materiałów używanych w szkołach.

```
  1---->2---->3---->4---->5---->Powtórzenie---->6---->...
```
Powyższa para-ilustracja przedstawia przykładowy schemat tematów w typowym szkolnym podręczniku. Tematy (zagadnienia) ułożone są w sposób linearny, tj. uczeń przyswaja wiedzę w podanej kolejności idąc tym samym (dosłownie) *do przodu* z materiałem.

Ten sposób może sprawdzać się w nauce prostych tematów, ale nie pasuje do nauki bardziej złożonych rzeczy. Wymieńmy wady tego podejścia, zakładając że poszczególne tematy (reprezentowane przez numerki) są skomplikowane:
 - Zależność tematów rzadko kiedy jest linearna - jeden temat może zależeć od wielu innych, np. 4 może poruszać w mniejszym lub większym stopniu zagadnienia z 3 jak i z 1.
 - Powyżej wymienione zależności nie są przejrzyście zilustrowane - uczeń który wraca do tematu po dłuższym czasie może nie być w pełni świadomy (nie zauważać) zależności.
 - Uczniowi ciężej jest wywnioskować do czego użyteczny jest dany temat i co z niego wynika, np. gdy temat dotyczy czystej teorii ciężko jest uczyć się go bez świadomości możliwości dalszych zastosowań.

Linearny program nauczania jest zaczerpnięty z strategii nauki zwanej [mastery learning](https://en.wikipedia.org/wiki/Mastery_learning). Warto jednak zauważyć, że gdy poszczególne jednostki (tematy, zagadnienia - w ilustracji wyżej numerki) nie są dostatecznie rozdrobnione (zagadnienia nie są elementarne), to możemy przechodzić dalej z materiałem pomimo (nawet subtelnych) braków w niektórych zagadnieniach.

Braki w znajomości materiału nie są złe - stanowią one jedynie okazje do ich uzupełnienia, jednak brak świadomości o ich istnieniu może powodować potem nieefektywną naukę, a co gorsza **budowanie wiedzy na podstawie wadliwych przekonań i niezupełnie zrozumianych fundamentów**. 

## Program zorganizowany w drzewa

Aby wyzbyć się poruszonych wyżej wad linearnego programu nauczania, zorganizujmy pojedynczy *sektor* materiału w drzewo. Niech będzie to ten sam sektor.

```
     1       Temat pierwszy jest podrzędny
    / \
   2   3     Tematy 2 i 3 są nadrzędne
      / \
     4   5
         |
         6
```

W tej organizacji materiału bazujemy *gałęzie* drzewa na wspólnych zależnościach między zagadnieniami. Pokazując tą strukturę uczniowi, klaryfikujemy mu z czego wynikają dane tematy i czy są one dalej poruszane w tym *sektorze*.

 - Temat 1: Baza całego sektoru, wstęp; od niego sektor się zaczyna. Może dotyczyć elementarnych prawd jak chociażby fundamentalne prawo fizyki - np. 1 zasada dynamiki.
 - Temat 2: Zagadnienie wynikające z tematu 1.
 - Temat 3: Zagadnienie wynikające z tematu 1, ale posiadające dalsze rozwinięcie w dalszych tematach.
 - Temat 4: Zagadnienie wynikające z tematu 3, nie posiadające dalszego rozwinięcia.
 - Temat 5: Zagadnienie wynikające z tematu 3, posiadające dalsze rozwinięcie. Warto spostrzec, że skoro zagadnienie 3 wynika z 1, to temat 5 w dużym stopniu wymaga również znajomości jedynki. 

Idea stosowania tego typu programu bazuje na upewnianiu się, że uczeń dobrze zrozumiał temat podrzędny zanim przejdzie do tematów nadrzędnych tj. wymagających znajomości podrzędnego. Spełnia to założenia **mastery learningu**, o ile poszczególne zagadnienia są dobrze rozdrobnione i ułożone.

Charakterystyka drzewek:
 - Widoczna struktura zależności między zagadnieniami
 - Wyróżnienie tematów ostatecznych - tych z których już *"nic nie wynika"*
 - Uwidacznia się tzw.*"kręgosłup"* - czyli główna gałąź, w której skupiona jest teoria.
 - Cięższe umiejscawianie powtórzeń, o ile chcemy aby powtórzenie obejmowało każdy temat.
 - Skonstruowanie drzewka wymaga zrozumienia zależności między zagadnieniami 
 - Opanowując i rozumiejąc kolejne tematy, uczeń redukuje ryzyko uczenia się *budując* wiedzę na złym lub niepełnym zrozumieniu podstaw. 

*Warto zwrócić uwagę na to, że możliwe skuteczniejsze w porządkowaniu wiedzy są grafy. One jednak w przypadku dużych zbiorów zagadnień mogą być chaotyczne i dezorganizować wiedzę - zamiast jej organizowania*

## Struktura programu nauczania w Edutie

Struktura programu nauczania w Edutie jest podwójnie zagnieżdżonym drzewem, tj. drzewem, którego każdy element (wierzchołek) zawiera w sobie drzewo. Oto hierarchia:
 1. Nauka
 2. Kurs
 3. Lekcje
 4. Segmenty lekcji

**Nauka** jest matką dla tworzonych materiałów. Funkcjonuje ona jako kategoria dla kursów tj. każdy kurs musi być przypisany do jakiejś nauki. Przykłady nauk:
 - Fizyka
 - Matematyka
 - Chemia

W Edutie chcemy poruszać nauki ścisłe, dlatego będziemy skupiać się głównie na tych trzech.

**Kursy** zawierają drzewo lekcji dotyczące danego zakresu materiału. Egzystują w ramach danej nauki. Kurs z założenia powinien dotyczyć pewnego działu z danej nauki. Przykłady:
 - Termodynamika
 - Optyka
 - Geometria

Kursy będą charakteryzować się również ***tagami***. Powyższe przykłady kursów mogłyby mieć takie tagi:
 - Oficjalne
 - Matura podstawa
 - Matura rozszerzona
Poza tym, wraz z rozszerzeniem repertuaru kursów, zwiększałaby się ilość tagów. W niektórych przypadkach tagi przypisywane byłby automatycznie (np. tag *Community* charakteryzujący kurs społeczności, byłby przypisywany automatycznie), w przypadkach gdy kurs tworzony byłby przez Edukatora wyższego przywilejami będzie on mógł przypisać ręcznie niektóre tagi (np. *Matura podstawa*). Sczegóły związane z tagami są do doprecyzowania w przyszłości.

Pomimo założeń, że kurs powinien zawierać duży zakres materiału, uwzględniamy możliwość tworzenia ***małych kursów*** (niezagnieżdżonych) i przypuszczamy że znajdą one duże zastosowanie w przypadku tworzenia ich przez uczniów.
 
**Lekcje** są drzewem segmentów. Jako element kursu są odpowiedzialne za nauczenie pojedynczego tematu z danego działu. Czas jaki uczeń miałby w założeniu poświęcać na jedną lekcję miałby wynosić **od pół do 1 godziny**. Przykłady lekcji:
 - Pierwsza zasada termodynamiki
 - Podstawowe funkcje trygonometryczne
 - Model korpuskularno-falowy

### Segmenty lekcji

**Segmenty** są elementarnymi częściami zagadnienia poruszanymi osobno. Tym samym jest to najbardziej atomiczna, niepodzielna część programu nauczania w Edutie. **Segmenty lekcji zawierają kontekst teoretyczny i zadanie (aktywność).** Zgodnie z założeniami [active learning](https://en.wikipedia.org/wiki/Active_learning), nauka powinna zachodzić poprzez aktywności - dlatego nauka w segmencie jest realizowana poprzez zapewnienie uczniowi aktywności do zrealizowania wraz z jej kontekstem teoretycznym. Uczeń realizując segmenty z danej lekcji powinien przeanalizować zagadnienie rozpatrywane przez tą lekcję z różnych perspektyw i na różne sposoby - od pokazania tych sposobów są właśnie segmenty.

Aktywności domyślnie realizowane są poprzez sprawozdanie. Ten sposób został wybrany, ponieważ wedle ideom nowej nauki kładzie on nacisk na sposób rozwiązania i dojścia do rozwiązania, a nie sam wynik. To, jak sprawozdanie powinno wyglądać będzie różnić się w zależności od rodzaju aktywności.

Segmenty mają przypisany do siebie **rodzaj aktywności** jaki go dotyczy. Rodzaje aktywności poruszone są w [edukacyjnym kontekście Edutie](Edukacja.md).

## Personalizacja w programie nauczania

Drzewiasty program nauczania umożliwia tworzenie ścieżek, które nazywamy w Edutie **nawigacją**.

Dużą rolę w kontekście personalizacji gra również segment, który dynamicznie potrafi kreować aktywności i redagować opisy teoretyczne tak, aby jak najlepiej dopasować je do ucznia.

Kwestie personalizacji opisane są dokładnie [tutaj](Personalizacja.md).