
# Instrukcja: publikacja plików źródłowych do Agent Buildera (wersja `.ab.md` / `.ab.html`)

## Co zawiera zestaw
- Pliki **`.ab.md`** – wzmocnione pod Agent Builder (meta, chunk, kotwice, TOC, FAQ, testy retrieval).
- Pliki **`.ab.html`** – przetworzone wersje HTML do publikacji w repo i podpięcia jako źródła wiedzy.

## Jak opublikować
1. Utwórz lub wybierz repozytorium GitHub (np. `knowledge-base-agents`).
2. W katalogu `docs/` umieść trzy pliki `.ab.html` **zamiast** wcześniejszych HTML.
3. W Agent Builder → **Źródła wiedzy** → wskaż nowe pliki HTML z gałęzi `main` (lub właściwej).
4. Przetestuj retrieval korzystając z sekcji **„Testy retrieval (dla Agent Builder)”** w każdym pliku.

## Dobre praktyki
- Trzymaj **`.ab.md`** jako *źródło prawdy* (edycja ustrukturyzowana), a **`.ab.html`** jako artefakt publikacyjny.
- Nie używaj konwerterów WYSIWYG – mogą zepsuć bloki `[[meta]]` i `[[chunk]]`.
- Pliki dziel tematycznie (jeden plik = jeden obszar) – poprawia trafność retrievalu.

## Aktualizacja
Po każdej zmianie `.ab.md` przetwórz ponownie na `.ab.html` i podmień w repo.
