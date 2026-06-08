## 1. Funkční požadavky (FR)

### Úvodní obrazovka (Autentizace)
Podle vizuálního návrhu úvodní stránky (přihlašovacího formuláře) systém splňuje následující požadavky:

| ID | Název požadavku | Popis požadavku | Hlavní role |
| :--- | :--- | :--- | :--- |
| **FR-01** | Přepínání režimů | Horní část rozhraní obsahuje jasně oddělené přepínače mezi režimem Přihlášení (Sign in) a Registrací (Sign up). | Hráč / Tvůrce |
| **FR-02** | Tradiční přihlášení | Formulář obsahuje textová pole pro zadání e-mailu a hesla pro uživatele s nativním Gitcraft účtem. | Hráč / Tvůrce |
| **FR-03** | Primární herní integrace | Systém nabízí dvě výrazná, prioritní tlačítka pro rychlé přihlášení pomocí herního účtu (Minecraft/Microsoft) a vývojářské platformy Modrinth. | Hráč / Tvůrce |
| **FR-04** | Sekundární přihlášení | V dolní části formuláře jsou k dispozici rychlé ikony pro přihlášení přes identity providery třetích stran (Google, Apple ID, případně další). | Hráč / Tvůrce |
### Hlavní uživatelské rozhraní (Dashboard)
Po přihlášení je uživatel přesměrován na hlavní vizuální rozcestník, který tvoří přehledné dlaždice, horní systémová lišta a spodní ovládací panel.

| ID | Název požadavku | Popis požadavku | Hlavní role |
| :--- | :--- | :--- | :--- |
| **FR-05** | Přehled projektů (Dlaždice) | Systém zobrazuje uživatelské projekty jako vizuální karty (dlaždice) obsahující název, typ projektu, ikonu a čas poslední úpravy. | Hráč / Tvůrce |
| **FR-06** | Plovoucí navigační panel | Na spodní straně obrazovky je permanentně dostupné rychlé menu s kruhovými ikonami pro bleskový přístup k hlavním funkcím. | Hráč / Tvůrce |
| **FR-07** | Uživatelský profil a Leveling | V pravém horním rohu je zobrazen avatar uživatele. Po rozkliknutí ukáže detaily účtu a postup v komunitním leveling systému. | Hráč / Tvůrce |
| **FR-08** | Kontextová nabídka (Tři tečky) | Systém obsahuje schované hlavní menu v pravém horním rohu, které se po kliknutí animovaně rozbalí do kompletní nabídky aplikací. | Hráč / Tvůrce |

### Prvky Plovoucího navigačního panelu
Spodní panel obsahuje 5 dedikovaných kruhových ikon s fixním pořadím:

| ID | Název požadavku | Popis požadavku | Hlavní role |
| :--- | :--- | :--- | :--- |
| **FR-09** | Centrální akční tlačítko (+) | Výrazné středové tlačítko slouží k okamžitému vyvolání nabídky pro založení nového projektu. | Tvůrce |
| **FR-10** | Rychlá navigace: Domů | Ikona domečku vrátí uživatele z jakékoliv podstránky zpět na hlavní přehled projektů. | Hráč / Tvůrce |
| **FR-11** | Rychlá navigace: Žebříček | Ikona stupně vítězů otevře komunitní žebříček a detaily o získaných zkušenostech (XP) a úrovních. | Hráč / Tvůrce |
| **FR-12** | Rychlá navigace: Nastavení | Ozubené kolečko otevře rychlé nastavení aplikace, rozhraní a správy propojených účtů. | Hráč / Tvůrce |
| **FR-13** | Přepínač vzhledu (Měsíček) | Ikona měsíce/slunce umožňuje uživateli jedním kliknutím změnit vizuální téma aplikace. | Hráč / Tvůrce |

## 2. Nefunkční požadavky (NFR)

| ID | Název požadavku | Popis a kritérium | Typ požadavku |
| :--- | :--- | :--- | :--- |
| **NFR-02** | Podpora tmavého režimu | Uživatelské rozhraní musí plně podporovat světlé i tmavé (Dark mode) zobrazení pro pohodlnou práci v noci. | Použitelnost (UI/UX) |
