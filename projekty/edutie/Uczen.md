# Uczeń i nauczanie w Edutie

W tym pliku opisana jest kwestia ucznia i śledzenia jego procesu nauczania w aplikacji.

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