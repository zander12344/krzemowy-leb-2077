# KRZEMOWY ŁEB 2077 — Strony na GitHub Pages

Publiczne lustro projektu z repozytorium prywatnego [`zander12344/krzemowy_leb`](https://github.com/zander12344/krzemowy_leb).

## Dedykowane widoki:

1. **Strona Seby (LBL) — Centrum Zamówień & Laptop AI:**  
   👉 [https://zander12344.github.io/krzemowy-leb-2077/](https://zander12344.github.io/krzemowy-leb-2077/) (`index.html`)  
   Dedykowana strona dla Seby: proste linki do zamówień, statusy paczek, budżet oraz instrukcja korzystania z gotowego serwera na laptopie w domu (Wi-Fi) i w trasie (4G przez Tailscale).

2. **Panel Techniczny Alexa (RZ) — Master Inżynierski:**  
   👉 [https://zander12344.github.io/krzemowy-leb-2077/alex.html](https://zander12344.github.io/krzemowy-leb-2077/alex.html) (`alex.html`)  
   Pełen panel dowodzenia dla Alexa: telemetria zamówień Seby na żywo (Live Sync), kalkulator budżetu, interaktywna mapa płyty ASUS X99-E WS, BIOS, procedury Linux/CUDA, kody Q-Code oraz szablony ofert Signal.

## Indeksowanie i Prywatność

Obie strony są zablokowane przed wyszukiwarkami: `robots.txt` (`Disallow: /`) + meta `noindex,nofollow,noarchive`. Linki są znane tylko osobom uprawnionym.

## Live Sync

Obie strony wymieniają stan na żywo w czasie rzeczywistym przez `ntfy.sh` (POST + SSE + poll `since=12h`). Zmiana statusu lub notatki u Seby natychmiast pojawia się w panelu Alexa i odwrotnie.

## Struktura

```
index.html    # Strona Seba LBL (zamówienia, koszyk, laptop Wi-Fi/4G)
alex.html     # Strona Alex RZ (pełen panel techniczny, montaż, BIOS, Q-Code, Signal)
.nojekyll     # Wyłącza Jekyll na GitHub Pages
robots.txt    # Blokada robotów indeksujących
```
