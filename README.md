# p1414 workflow acceptance

Kontrolowane repo do odbioru synchronizacji p1414 z GitHubem.

Repo zawiera wyłącznie fikcyjne dane i workflow testowy. Nie przechowuje kodu,
sekretów ani danych środowiska produkcyjnego.

## Kontrole

- `required-check` jest wymagany przez ochronę `main`.
- `optional-check` celowo kończy się błędem i pozostaje niewymagany.

Scenariusze i wyniki odbioru są przechowywane w projekcie p1414 `tests`.
Proces pracy pochodzi z bieżących reguł p1414.
