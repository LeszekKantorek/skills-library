# skills-library

Biblioteka skilli AI instalowanych przez [`npx skills`](https://github.com/vercel-labs/skills). Dostępne skille i ich oceny znajdziesz w [CATALOG.md](CATALOG.md).

## Instalacja

```sh
npx skills add LeszekKantorek/skills-library --list
npx skills add LeszekKantorek/skills-library --skill <name>
```

`<name>` to nazwa z katalogu. Biblioteka na starcie nie zawiera importowanych skilli. Własny `library-curator` służy do utrzymania tego repozytorium i nie jest wpisem katalogu importów.

## Struktura

```text
.agents/skills/library-curator/SKILL.md  # instrukcje dla opiekuna biblioteki
skills/<name>/SKILL.md                  # importowany skill i jego zasoby
imports/<name>.md                      # techniczne review importu
README.md
CATALOG.md
```

## Import przez GitHub Issue

1. Utwórz issue przez formularz „Import skill” i podaj jeden lub więcej linków.
2. Opiekun rozwiązuje linki do konkretnych wersji, sprawdza treść, zasoby, zależności i możliwość redystrybucji. Samo zgłoszenie linku nie uruchamia obcego kodu.
3. Import trafia do PR razem z review w `imports/` i wpisem w katalogu. Aktualizacja istniejącego skilla także wymaga issue, nowej oceny i PR.
4. Po scaleniu wszystkich zaakceptowanych pozycji oznacz issue `imported` i zamknij. Całkowicie odrzucone zgłoszenie oznacz `rejected` i zamknij, zachowując uzasadnienie.

Jedynymi etykietami repozytorium są `imported` i `rejected`; są wzajemnie wykluczające. Brak etykiety oznacza otwarte zgłoszenie oczekujące lub w trakcie pracy — nie tworzymy etykiety `open`. Przy wielu linkach śledź wynik każdego z nich w issue. Jeśli tylko część zostanie odrzucona, po zakończeniu wszystkich pozycji użyj `imported` i wskaż odrzucone pozycje w podsumowaniu. Do tego czasu issue pozostaje otwarte bez etykiety.

Issue jest kolejką dla opiekuna; formularz nie uruchamia automatycznego importu. Etykiety opisują wynik, a nie poziom ryzyka.

## Risk

Ocena dotyczy konkretnej wersji oraz jej instrukcji, dołączonego kodu i zależności. Uwzględnia też działania, do których skill nakłania agenta, nawet gdy nie zawiera skryptów. Wybierz najwyższy uzasadniony poziom i opisz konkretny powód w review.

| Risk | Kryteria i przykłady | Decyzja importowa |
| --- | --- | --- |
| `low` | Instrukcje i lokalny odczyt; brak wykonywania kodu, wysyłania danych i zmian zewnętrznych. | Możliwy po review. |
| `medium` | Ograniczone, odwracalne zapisy lokalne lub przejrzyste skrypty/zależności; odczyt sieci bez przekazywania prywatnych danych. | Możliwy po opisaniu zakresu i zależności. |
| `high` | Dostęp do sekretów, wysyłanie danych, publikacja, modyfikacja usług, usuwanie danych lub szerokie uprawnienia. | Wymaga udokumentowanej akceptacji opiekuna dla tej wersji w PR i jasno opisanych zabezpieczeń. |
| `critical` | Wykradanie danych, ukryte destrukcyjne działania, złośliwe instrukcje lub obchodzenie zabezpieczeń. | Odrzuć; nie umieszczaj plików w `skills/`. |
| `unknown` | Nie udało się zbadać istotnych plików, zależności lub zachowania. To brak oceny, nie niski poziom. | Wstrzymaj import do wyjaśnienia; przy odmowie zakończ jako `rejected`. |

Ocena nie jest gwarancją bezpieczeństwa. Brak prawa do redystrybucji blokuje import niezależnie od `risk`; zapisz go jako osobne ustalenie, bez automatycznego podnoszenia poziomu.

## Review importu

Każdy import i jego aktualizacja mają `imports/<name>.md`. Pełny SHA i link do commita źródłowego wskazują dokładnie ocenioną wersję; nie wpisuj tutaj przyszłego commita biblioteki. Historia review pozostaje w Git.

```yaml
---
link: "https://github.com/OWNER/REPO/tree/FULL_SHA/path/to/skill"
name: "local-skill-name"
sha: "FULL_SOURCE_COMMIT_SHA"
commit: "https://github.com/OWNER/REPO/commit/FULL_SHA"
risk: "medium"
---
```

Pod frontmatter opisz: issue, oryginalną nazwę, pochodzenie i licencję, sprawdzone pliki, zachowanie i uprawnienia, sieć i przepływ danych, zależności, uzasadnienie ryzyka, zmiany względem oryginału, wykonane sprawdzenia i ograniczenia oraz decyzję. Nie deklaruj testów, których nie wykonano.

Dla źródła bez Git ustaw `sha` i `commit` na `null`, podaj stabilny link w `link` oraz sumę SHA-256 pobranego artefaktu w treści review. Bez identyfikowalnej kopii źródła wstrzymaj import. Dla odrzuconego skilla zachowaj review, ale nie twórz wpisu w katalogu ani katalogu w `skills/`.

## Zmiany w bibliotece

Docelowa konfiguracja `main`: wymagany PR, ochrona także administratorów, wyłączony force push i usuwanie gałęzi. Sam wymóg PR nie oznacza wymogu akceptacji drugiej osoby; pozwala to utrzymywać bibliotekę jednoosobowo. Pierwszy commit pustego repozytorium tworzy gałąź bazową, a dalsze zmiany przechodzą przez PR.
