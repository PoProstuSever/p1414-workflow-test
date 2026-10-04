# p1414 workflow acceptance

Kontrolowane repo do odbioru synchronizacji p1414 z GitHubem.

Repo zawiera wyłącznie fikcyjne dane i workflow testowy. Nie przechowuje kodu,
sekretów ani danych środowiska produkcyjnego.

## Kontrole

- `required-check` jest wymagany przez ochronę `main`.
- `optional-check` celowo kończy się błędem i pozostaje niewymagany.

Scenariusze i wyniki odbioru są przechowywane w projekcie p1414 `tests`.
Proces pracy pochodzi z bieżących reguł p1414.

## Kontrolowany przebieg PR

Pierwsza wersja PR-a utrzymuje wymagany check w stanie oczekiwania przez 45 sekund,
a następnie kończy go błędem. Ta wersja nie nadaje się do merge.
Po niezależnym review autor przywróci wynik `pass` w tym samym PR-ze.
Odbiór ma potwierdzić aktualny SHA, zmianę stanu checków i brak duplikatów.
