# Web Challenge: Landing Page pro aplikaci Gradely

**Časový limit:** 45 minut  
**Povolené zdroje:** Vaše dosavadní kódy, W3Schools.com, MDN Web Docs  
**Cíl:** Vzít texty a informace z poslední hodiny a přetvořit je do atraktivní „Landing Page“ (prezentační stránky) pro aplikaci Gradely. 

## Část 1: To už znáte (80 % práce)
Vytvořte čistý `index.html` a `style.css`. Využijte své dosavadní znalosti k sestavení základu:
1. **Obsah:** Stránka bude obsahovat hlavní nadpis (`h1`), popis aplikace, podnadpis (`h2`), seznam hlavních funkcí (`ul`) a funkční tlačítko pro stažení. (Texty si zkopírujte z našeho posledního cvičení).
2. **Formátování textu:** Nastavte celé stránce bezpatkový font (např. *Segoe UI* jako minule). Využijte třídy (např. `.center`) pro zarovnání hlavních nadpisů na střed obrazovky.
3. **Tlačítko:** Vytvořte tlačítko s výzvou „Stáhnout Gradely“. Přidejte mu zelené pozadí, bílý text, vnitřní odsazení (`padding`), zaoblené rohy (`border-radius`) a změnu barvy po najetí myši (pomocí `:hover`).

## Část 2: W3Schools Výzva (Tohle musíte dohledat)
Váš dosavadní kód funguje, ale k dokonalosti mu chybí pár moderních CSS vlastností. Vaším úkolem je najít je na internetu a implementovat.

1. **Zkrocení šířky stránky (Centrování bloku):**
   * Váš text se momentálně roztahuje od levého okraje prohlížeče až k pravému, což se na velkých monitorech špatně čte.
   * *Úkol:* Zabalte celý obsah stránky do jednoho hlavního `<div id="obsah">`. V CSS mu nastavte maximální šířku (např. `max-width: 800px;`) a zjistěte, jak tento celý blok **horizontálně vycentrovat doprostřed obrazovky**. 
   * *Nápověda:* `text-align` na tohle nefunguje, to řeší jen text. Hledejte, jak funguje vlastnost `margin` s hodnotou `auto`.
2. **Čistý seznam funkcí:**
   * U seznamu hlavních funkcí (`ul`) vás štvou výchozí černé tečky na začátku každého řádku. 
   * *Úkol:* Najděte CSS vlastnost, která tyto tečky (odrážky) trvale skryje, aby seznam vypadal spíše jako moderní blok textu.
3. **Plynulá animace tlačítka:**
   * Váš hover efekt u tlačítka způsobí, že barva "skočí" okamžitě.
   * *Úkol:* Zjistěte, jak v CSS zařídit, aby přechod mezi zelenou a modrou barvou trval plynule například `0.3s`. (Hledejte vlastnost `transition`).
4. **Efekt prostoru (Stín):**
   * Aby tlačítko pro stažení opravdu lákalo ke kliknutí, musí trochu vystupovat z plochy.
   * *Úkol:* Přidejte tlačítku v CSS jemný stín. (Hledejte vlastnost `box-shadow`).

---

## Lektorský tahák (Pouze pro vyučujícího)

Co byste měli u studentů na monitorech ideálně vidět, pokud použijí W3Schools správně:

* **Centrování bloku:** `#obsah { max-width: 800px; margin: 0 auto; }`
* **Očištění seznamu:** `ul { list-style-type: none; padding-left: 0; }` (Je potřeba vynulovat i padding, jinak tam zbyde prázdné místo).
* **Plynulý hover:** Vlastnost musí být na základním elementu `button` (ne až v hoveru). Ideálně `transition: background-color 0.3s ease;`.
* **Stín:** `box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);`
