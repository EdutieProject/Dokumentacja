# Git - porady

W tym pliku mamy praktyczne porady do git'a i jego interakcji z naszym GitHubem. Jeśli masz kłopot dotyczący gita i jego używania, daj znać to dodamy tu nowy tutorial.

Spis pordaników:
 - [Generowanie tokenu dostępu](#generowanie-tokenu-dostępu)
 - [Praca na repozytoriach organizacji](#klonowanie-repozytoriów)
 - [Praca na forkach](#praca-na-forkach)
 - [Wprowadzanie zmian i konwencje](#wprowadzanie-zmian-i-konwencje)

## Generowanie tokenu dostępu

Tokeny generujemy [tutaj](https://github.com/settings/personal-access-tokens/new).

GitHub narzuca uwierzytelaninie poprzez **tokeny dostępu**. Tokeny utworzone poprzez powyższy link są niezbędne aby uwierzytelnić swój dostęp do repo.

## Klonowanie repozytoriów

Preferowanym sposobem interakcji z repozytoriami jest klonowanie ich bezpośrednio. Dzięki temu pracujemy na branchach i łatwiej jest konkurencyjnie wprowadzać zmiany. 

Zróbmy to na przykładzie tego repozytorium.

```bash
git clone https://github.com/EdutieProject/Dokumentacja.git
```

Wywołanie tego polecenia wywoła zapytanie o uwierzytelnienie. Podajemy jako login nazwę użytkownika z GitHuba (np. *sukerberk1* ), jako hasło poprzednio wygenerowany **token dostępu**.

Jeśli dostajesz odpowiedź 403 i uważasz że powinno być inaczej, odezwij się do @sukerberk1 albo @memez-michalek 

[Dowiedz się więcej](https://stackoverflow.com/questions/2505096/clone-a-private-repository-github)

## Praca na forkach

Drugim sposobem wprowadzania zmian w repozytoriach jest praca na forku. Jeżeli chcesz aby to był twój *stały* sposób interakcji z repo i z jakiegoś powodu nie możesz go sklonować, dodaj główne repo jako *remote*:

```
git remote add nn-github https://github.com/EdutieProject/Dokumentacja.git
```

Wtedy aby ściągnąć zmiany z głównego brancha repozytorium trzeba ściągnąć je używając uprzednio dodanego remote'a:

```
git pull nn-github main
```

[Dowiedz się więcej](https://stackoverflow.com/questions/3903817/pull-new-updates-from-original-github-repository-into-forked-github-repository)

## Wprowadzanie zmian i konwencje

Domyślnie zmiany powinniśmy robić oczywiście na osobnych branchach. 
```
git checkout -b feature/hello-world
```
Komenda na górze tworzy branch! Konwencja nazywania branchów każe nazywać je tzw. *kebab-casem* czyli małymi literami z myślnikami. Dodatkowo, branche powinniśmy segregować folderami, dodając przed branchem nazwę kategorii dla danego brancha. 

Sugerowane kategorie:
 - `feature/`
 - `refactor/`
 - `docs/`
 - `bug/`

*Kategorie oczywiście nie obowiązują w repo takich jak te, w którym jest tylko dokumentacja.*

Dogrywanie zmian do głównego repo robimy tworząc PR'ki - pull requesty. Możemy też tego nie robić, albo robić zmiany bezpośrednio na głównym branchu (`main`), ale z tym trzeba uważać - robimy tak tylko w przypadku małych zmian.

**Przed zrobieniem pull requesta koniecznie wgraj zmiany z głównego brancha przez `git pull origin main`!***

**W przypadku pracy na forku zmień origin na nazwę remote'a głównego repo*