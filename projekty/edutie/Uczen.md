# Uczeń i nauczanie w Edutie

W tym pliku opisana jest kwestia ucznia i śledzenia jego procesu nauczania w aplikacji.

## Profil nauczania

**Profil ucznia** to domyślny profil każdego użytkownika platformy mający na celu zbieranie danych o użytkowniku w kontekście nauki. Jest to kluczowy element Edutie - na jego podstawie działa [personalizacja](Personalizacja.md). Warto przykuć do niego szczególną uwagę, ponieważ uczeń powinien być *w centrum zainteresowania* w kwestii edukacji. Jego elementami są:
 - Uczniowskie protfolio
 - Historia nauki
 - Parametry psychologiczne
 - Parametry osobowościowe

### Uczniowskie portfolio
Pomimo mało sugestywnej nazwy chodzi tu głównie o cechy jakie osoba korzystająca z aplikacji ma w kontekście bycia uczniem. Wchodzi w to klasa w jakiej się on znajduje, rodzaj szkoły do jakiej uczęszcza, jego wiek. Możemy tu również wrzucić wszelkie konkursy czy aktywności pozaszkolne jakie uczeń ma *a'la CV*. Dobrze byłby to potraktować podobnie do profilu na np. LinkedIn. 

### Historia nauczania
Historia nauczania jest zbiorem wyników ze wszystkich aktywności jakie ukończył uczeń. Wyniki te będziemy nazywać *Rezultatami nauczania*.

#### Rezultat nauczania
Rezultat nauczania powinien być swego rodzaju raportem z aktywności jaką uczeń zrealizował. Powinien on zawierać dane:
 - o tym jaką aktywność realizował uczeń
 - jakie sprawozdanie przesłał
 - jak został oceniony i dlaczego
 - jaki dostał feedback (to też wynika z powyższego)
 - szczegóły dotyczące progresu (więcej w [opisie systemu progresu](SystemProgresu.md))

Na podstawie rezultatów nauczania możemy budować *historię nauczania*. Domyślnie śledzimy globalną historię, czyli historię z całego okresu nauki w aplikacji. Parametry psychologiczne i osobowościowe podparte są globalną historią nauki, czyli są one wynikową wszystkich rezultatów nauczania.

Możemy również dynamicznie tworzyć krótkoterminowe historie nauczania, np. agregując tylko rezultaty nauczania sprzed miesiąca. Na podstawie krótkoterminowych historii możemy wywnioskowywać ostatnie rezultaty - na przykład możemy obliczać parametry na podstawie krótkoterminowych historii, wiedząc jakie uśrednione parametry określają ostatni okres nauki.

 ### Parametry psychologiczne
> *Do uzupełnienia*\
*Notatki: byłyby wykorzystywane dla: Spersonalizowanego tłumaczenia teorii, personalizacji aktywności, personalizacji podpowiedzi. Byłyby dostosowywane za pomocą: rezultatów nauczania (?), błędów*
### Parametry osobowościowe
> *Do uzupełnienia*\
*Notatki: the big 5 personality, testy na rodzaj chleba którym jesteś*
