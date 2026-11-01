# KRZEMOWY ŁEB 2077 — strona na GitHub Pages

Publiczne lustro poradnika z repozytorium [`zander12344/krzemowy_leb`](https://github.com/zander12344/krzemowy_leb).

**Strona:** https://zander12344.github.io/krzemowy-leb-2077/

## Co to jest

Interaktywna lista zakupów i poradnik budowy serwera AI:
Xeon E5-2690 v4 na LGA 2011-3 (X99), 4× RTX 3070 8 GB, 128 GB DDR4 ECC,
silnik `ik_llama.cpp` + natywny runtime Strata pod model Qwen 177B MoE.

## Indeksowanie

Strona jest zablokowana przed wyszukiwarkami: `robots.txt` (`Disallow: /`) + meta `noindex,nofollow,noarchive` w `index.html`. Link jest znany tylko osobom, ktorym go wyslano.

## Synchronizacja

`index.html` jest kopią `LISTA_ZAKUPOW_GOOGLE_DOCS.html` z głównego repozytorium.
Aktualizacja: podmień plik i wypchnij na `main` — Pages przebuduje stronę automatycznie.

Stan checklisty między urządzeniami (Rzeszów ↔ Frampol) synchronizuje się przez
`ntfy.sh` (POST + SSE + poll `since=12h`), więc działa bez backendu.

## Struktura

```
index.html    # cały poradnik + logika Live Sync (jeden plik, zero zależności)
.nojekyll     # wyłącza przetwarzanie przez Jekyll
```
