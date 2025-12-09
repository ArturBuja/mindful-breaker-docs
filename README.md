# 📚 Mindful Breaker - Official Documentation

To repozytorium zawiera oficjalną stronę **Polityki Prywatności** oraz **FAQ** dla aplikacji mobilnej **Mindful Breaker**.

Strona jest hostowana przy użyciu **GitHub Pages** i służy jako wymagany punkt informacyjny dla Sklepu Google Play oraz użytkowników aplikacji.

🌐 **Live Site:** [https://ArturBuja.github.io/mindful-breaker-docs/](https://ArturBuja.github.io/mindful-breaker-docs/)

---

## 📂 Struktura Strony

Projekt wykorzystuje prostą strukturę katalogów do obsługi wielu języków bez skomplikowanych frameworków.

* **`index.html`** - Inteligentny skrypt przekierowujący. Wykrywa język przeglądarki użytkownika i automatycznie kieruje do odpowiedniego folderu (np. `/pl/` lub `/en/`).
* **`/en/`** - Dokumentacja w języku angielskim (Domyślna).
    * `privacy.html` - Privacy Policy (Wymagana przez Google Play).
    * `faq.html` - Frequently Asked Questions.
* **`/pl/`** - Dokumentacja w języku polskim.
* **`/de/`, `/es/`, ...** - Pozostałe wersje językowe.
* **`/assets/`** - Wspólne style CSS (`style.css`) oraz obrazy.

---

## 🔗 Jak linkować w aplikacji?

Aby odesłać użytkownika do odpowiedniej sekcji, używamy jednego uniwersalnego linku z parametrem. Skrypt `index.html` zajmie się resztą (wykryciem języka i przekierowaniem).

| Cel | Link do użycia w kodzie Androida |
| :--- | :--- |
| **Polityka Prywatności** | `https://ArturBuja.github.io/mindful-breaker-docs/?page=privacy` |
| **FAQ** | `https://ArturBuja.github.io/mindful-breaker-docs/?page=faq` |

---

## ➕ Jak dodać nowy język?

1. Skopiuj folder `en/` i zmień jego nazwę na kod nowego języka (np. `fr` dla francuskiego).
2. Przetłumacz pliki `privacy.html` i `faq.html` wewnątrz nowego folderu.
   * *Wskazówka:* Nie musisz zmieniać stylów CSS, są ładowane z głównego folderu `assets`.
3. (Opcjonalnie) Zaktualizuj plik `index.html`, dodając nowy język do listy ręcznego wyboru na dole strony.
4. Zrób `git push` - GitHub Pages zaktualizuje się automatycznie w ciągu minuty.

---

## 📞 Kontakt

W sprawach związanych z aplikacją lub polityką prywatności:
📧 [artur.buja2@gmail.com](mailto:artur.buja2@gmail.com)

---
&copy; 2025 Mindful Breaker. Wszystkie prawa zastrzeżone.
