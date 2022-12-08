# Zadání soutěže 2022

Zkontrolujte si stav baterie robota!

## Zadání

_Zadání si v klidu přečtěte, pokud něco nebude jasné, ihned se ptejte_

- Rozsviťte celého robota fialově (diody na gimbalu i na těle) (EP: stačí tělo). Takto bude svítit po dobu konání následujících úkolů.
- Přehajte libovoný zvuk.
- Na začátku s robotem opište pravoúhlý trojúhelník, tak aby se robot vrátil do výchozí pozice. První hranu veďte pod úhlem 0° a druhou pod kladným úhlem. Délka odvěsen bude 60 cm a pravý úhel se bude nacházet v místě výchozí pozice. Robot se bude dívat stále stejným směrem.
- Následujte modrou čáru. Čáru robot uvidí ze své úvodní pozice, nemusíte ji tedy na začátku hledat. Pokud narazíte na křižovatku, vydejte se cestou vpravo. Správná cesta na křižovatkách bude vždy pod úhlem 90°. Pokud čáru už neuvidíte, proveďte rotaci o 90° vpravo. Pokud tam bude čára, následujte ji. Pokud tam čára nebude, otočte se o 90° vlevo (od původní čáry) a pokračujte po čáře, kterou tam uvidíte. Tuto rotaci provádějte na místě, kde čára končí (_ne, kde robot čáru přestal vidět_).
- Pokud neuvidíte čáru, ale budete vidět marker s číslem (uvidíte ho přímo před sebou), nerotujte. Místo toho objeďte marker (je jedno z jaké stray a je jedno jakým obrazcem ho objedete), tolikrát dokola, kolik je číslo na markeru. Okolo markeru bude dostatek místa pro vaše manévry.
- Po obkroužení markeru přehrajte libovolný zvuk (značka že už je hotovo, hodnoceno 0 body)



## Bodování

Vzhledem k chybovosti rozpoznávání budete mít až 3 pokusy (bude-li to mít smysl) na to projet trať. Počítat se bude nejúspěšnější pokus.

- Za každý splěný úkol dostanete 1 bod (rozsvícená světla, zvuk, trojúhelník)
- Za každou splněnou překážku získáte 1 bod (křižovatka, výpadek čáry)
- Obkroužený marker 2 body
- Dráha se jede na čas. V případě shodného zisku bodů rozhodne o pořadí čas projetí tratě a kvality zdrojového kódu
- Nápověda za -2 body
- Pokud narazíte do tratě (krabice) nebo do markeru (posunout krabici, nebo shodit marker) -1 bod
- Váš zásah do jízdy robota (posunutí, když se ztratí) -2 body
- Zdrojový kód bude ohodnocen 0 až 3 body

## Povolené pomůcky

- Můžete požívat jakékoliv přechozí lekce a dostupné materiály (ať už odkazované nebo nalezené na internetu)
- Zakázáno je pouze komunikovat s živými lidmi (robotů se ptát můžete ;) )


## Na co si dát pozor

### Python hlásí `Syntax error`

Dejte si pozor, jestli na řádce s chybou, nebo na předchozí řádce nechybí dvojtečka na konci řádku, pokud se jedná o další blok. Nový blok vytvářejí příkazy například `if`, `while`, `for`, `def`.

### Python hlásí chybu na řádku, která ani není v programu

Zkontrolujte počty argumentů funkcí (kolik hodnot dáváte do funkce). Např. dáváte do funkce jen jeden vstup a funkce očekává dva.

### Robot vůbec (hrozně špatně) nerozeznává číslice

Restartujte robota.

### Pozor na správné odsazení bloků kódu (správně viz např.)

```python

if True:
    prikaz1
    prikaz2
else:
    prikaz3

for i in range(10):
    prikaz_se_provede_10x

```
