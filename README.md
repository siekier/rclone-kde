# rclone KDE — witryna informacyjna OAuth

Prosta strona statyczna do GitHub Pages, przeznaczona dla prywatnej konfiguracji OAuth używanej przez `rclone` na Linuksie (Dolphin/KDE Plasma). Styl nawiązuje do strony `bison-ksef`, ale projekt jest od niej niezależny.

## Zawartość

- `index.html` — opis prywatnej integracji
- `prywatnosc.html` — polityka prywatności
- `warunki.html` — warunki korzystania
- `style.css` — styl strony, bez zewnętrznych bibliotek
- `.nojekyll` — publikuje pliki bez przetwarzania przez Jekyll

Strony nie zawierają JavaScriptu, trackerów, formularzy logowania, danych OAuth ani tokenów.

## Jak opublikować na GitHub

1. Zaloguj się na GitHub do konta `siekier`.
2. Utwórz **publiczne** repozytorium `rclone-kde`: https://github.com/new
3. Wybierz **Add file → Upload files**, rozpakuj archiwum ZIP i przeciągnij wszystkie pliki z jego wnętrza do katalogu głównego repozytorium. Nie wrzucaj samego ZIP-a.
4. Zatwierdź zmianę (*Commit changes*).
5. Wejdź w **Settings → Pages** i ustaw **Deploy from a branch → main → / (root)**, następnie **Save**.
6. Sprawdź trzy adresy:
   - https://siekier.github.io/rclone-kde/
   - https://siekier.github.io/rclone-kde/prywatnosc.html
   - https://siekier.github.io/rclone-kde/warunki.html
7. Opcjonalnie pozostaw włączoną zakładkę **Issues**, bo polityka prywatności odsyła do niej jako kanału kontaktu.

## Adresy do Google Cloud → Elementy marki

- **Nazwa aplikacji:** `rclone KDE`
- **Strona główna:** `https://siekier.github.io/rclone-kde/`
- **Polityka prywatności:** `https://siekier.github.io/rclone-kde/prywatnosc.html`
- **Warunki korzystania:** `https://siekier.github.io/rclone-kde/warunki.html`
- **Autoryzowane domeny:** jeśli formularz o to pyta, `siekier.github.io` (nie wklejaj pełnego adresu strony).

**Ważne:** opublikowanie stron nie jest równoznaczne z zatwierdzeniem ani weryfikacją aplikacji OAuth. Google może wymagać potwierdzenia kontroli nad domeną w Search Console; hosting na współdzielonej domenie `github.io` może komplikować ten wymóg. Jeżeli Google odrzuci adres, rozwiązaniem jest użycie własnej domeny lub odpowiedniej subdomeny z kontrolą DNS, nie tworzenie kolejnych fikcyjnych podstron.

Jeśli po uruchomieniu konfiguracja będzie używać innych uprawnień OAuth, kont innych użytkowników lub innych mechanizmów przesyłania/przechowywania danych, zaktualizuj opisy oraz politykę prywatności, aby pozostały zgodne z rzeczywistością.

## Bezpieczeństwo

Nie umieszczaj w publicznym repozytorium plików `rclone.conf`, tokenów, Client Secret ani pobranych dokumentów prywatnych.
