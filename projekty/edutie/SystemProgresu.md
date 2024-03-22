# System progresu
Ten plik poświęcony jest opisowi systemu progresu w aplikacji Edutie.
System progresu jest ściśle powiązany z [programem nauczania Edutie](ProgramNauczania.md) - bazuje on na jego elementach.

### Spis treści: 
1. Zaliczenie - podstawa progresu
2. Progres w programie nauczania
3. Progres mierzony indywidualnie

## Zaliczenie

Podstawą progresu jest ***zaliczenie*** - czyli osiągnięcie wymagań sprecyzowanych w danym segmencie. Zaliczenia odbywają się w obrębie segmentu - najbardziej atomicznej części programu nauczania.

#### Wymagania nauczania

Zaliczenie przydzielane jest na podstawie wymagań nauczania sprecyzowanych w segmencie. Wymagania w definicji powinna zawierać konkretnie sprecyzowane jakie ***zrozumienie*** uczeń powinien posiąść w trakcie wykonywania aktywności w tym segmencie. Poprzez model językowy analizujemy sprawozdanie i rozstrzygamy w jakim stopniu wymaganie zostaje spełnione.

#### Ocenianie

Oceniamy ucznia na podstawie spełniania wymagań nauczania w skali ***1-6***. Ocenianie oparte jest na modelu językowym i poniższej *definicji* skali:
 - 1 : Uczeń nie wykazuje żadnego zrozumienia określonego w wymaganiu
 - 2 : Uczeń wykazuje fundamentalnie niepoprawne zrozumienie określone w wymaganiu
 - 3 : Uczeń wykazuje niepełne zrozumienie określone w wymaganiu, popełniając przy tym błędy
 - 4 : Uczeń wykazuje niepełne zrozumienie określone w wymaganiu, nie popełniając przy tym błędów
 - 5 : Uczeń wykazuje pełne zrozumienie określone w wymaganiu popełniając przy tym błędy
 - 6 : Uczeń wykazuje pełne zrozumienie określone w wymaganiu nie popełniając przy tym błędów

**⚠** Oceny zaliczające w tej skali to oceny 5 i 6.

## Progres w programie nauczania

#### Zaczynając od zewnątrz:
Kurs jako najwyższy hierarchią element programu nauczania nie jest obięty systemem progresu. To, czy uczeń ma dostęp do kursu nie powinno być warunkowane osiągnięciami z innych kursów. Może być to conajwyżej warunkowane poziomami dostępu do kursu ustalonymi przez twórcę.

#### Wewnątrz drzewek:

Podstawowa struktura programu nauczania to podwójnie zagnieżdżone drzewo. Rozważmy wewnętrzne drzewo tj. drzewo segmentów.

W drzewie segmentów *zaliczenie* danego segmentu ustalane jest poprzez zaliczenie określonej przez [personalizację](Personalizacja.md) liczby aktywności należącej do poprzedniego segmentu.

W drzewie nadrzędnym tj. drzewie lekcji progres następuje podobnie - po wypełnieniu całego drzewa podrzędnego w formie lekcji (zaliczeniu wszystkich segmentów z lekcji) można przejść do następujących elementów (następujących lekcji). Wygląda to tak:
```
  ✅
  / \
 ❓  ❓
    / \
   ❌ ❌
```

Na tym schemacie przedstawione jest drzewo w którym:
✅ - to element zaliczony
❓ - to elementy odblokowane
❌ - to elementy aktualnie niedostępne 

## Progres mierzony indywidualnie

Ważne jest również odnotowywanie progresu ucznia jako takiego. Robimy to na podstawie rezultatów nauczania, które opisane są w [kwestiach ucznia](Uczen.md). Ustrukturyzowana historia nauczania tj. chronologicznie uporządkowane rezultaty pozwalają śledzić progres ucznia aby zapewnić mu feedback na temat jego postępów.