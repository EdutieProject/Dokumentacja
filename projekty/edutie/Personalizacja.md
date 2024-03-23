# Personalizacja

Personalizacja jest jedną z kluczowych kwestii Edutie. Ma ona sprawić, że użytkownik - uczeń - będzie konsumował naukę w bardziej przyjaznym i przyjemniejszym wydaniu. Personalizacja ma na celu zmianę zdania ucznia o nauce i przekonanie go, że nie jest ona żmudnym obowiązkiem, a okazją aby nauczyć się nowych, ciekawych rzeczy.

W Edutie rozpatrujemy takie sposoby personalizacji:
 - [W segmentach](#personalizacja-w-segmentach): 
   - Personalizacja kontekstu teoretycznego
   - Personalizacja aktywności
   - Personalizacja podpowiedzi
 - [Nawigacja wśród segmentów](#nawigacja---segmenty)

## Personalizacja w segmentach
Segment jest najbardziej elementarnym ogniwem programu nauczania w aplikacji. Można się dowiedzieć czym on jest w [opisie programu nauczania](ProgramNauczania.md). Tutaj będziemy bazować na wiedzy stamtąd.

Aby personalizować segment korzystamy z technologii AI - dużych modeli językowych. Personalizacja bazuje na ***Strategiach personalizacji***

#### Strategia Personalizacji - czym jest ?

Strategia personalizacji to opis wprowadzany do modelu językowego, który bierze go pod uwagę przy generowaniu treści. Wprowadzany przez strategię personalizacji opis ma na celu dostosowanie generowanego materiału pod ucznia. Dokonujemy selekcji strategii w oparciu o indywidualne rozpatrywanie warunków jakie dana strategia musi spełniać w oparciu o profil ucznia ([zobacz kontekst ucznia](Uczen.md)).

### Kontekst teoretyczny

> *Do uzupełnienia*\
Notatki: dynamiczne generowanie, funkcja zeszytu, funckja tłumaczeń

### Aktywność

> *Do uzupełnienia*\
Notatki: liczba wymaganych aktywności, dynamiczne generowanie aktywności, użycie strategii,

### Podpowiedzi

> *Do uzupełnienia*\
Notatki: dynamiczne generowanie, użycie strategii

## Nawigacja - segmenty
Kolejnym sposobem personalizacji nauki jest nawigowanie, konkretnie wśród drzewa segmentu. Polega ono na wskazywaniu która ścieżka (który segment) jest najlepszym wyborem jako następnie wybrany. 

#### Poziom trudności - jak go określamy?
Kluczowym w nawigacji jest określenie poziomu trudności - robimy to dynamicznie bazując na profilu ucznia, w szczególności na historii naucznia. Więcej o profilu ucznia dowiesz się w [kontekście ucznia](Uczen.md).

Kategorie nawigacji:
 - Wyzwanie : z odblokowanych niezaliczonych elementów wybierz najtrudniejszy
 - Nowość : z odblokowanych niezaliczonych elementów wybierz najłatwiejszy
 - Powtórka : z zaliczonych elementów wybierz, ten którego uczeń najbardziej mógł zapomnieć (?)

> *Precyzyjne określenie działania sposobów nawigacji do uzupełnienia*