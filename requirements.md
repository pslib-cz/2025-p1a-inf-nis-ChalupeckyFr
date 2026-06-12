## 1. Funkční požadavky (FR)

### Úvodní obrazovka (Autentizace)
Podle vizuálního návrhu přihlašovacího formuláře systém splňuje následující požadavky na přístup:

| ID | Název požadavku | Popis požadavku | Hlavní role |
| :--- | :--- | :--- | :--- |
| **FR-01** | Přepínání režimů | Horní část rozhraní obsahuje jasně oddělené přepínače mezi režimem Přihlášení (Sign in) a Registrace (Sign up). | Hráč / Tvůrce |
| **FR-02** | Tradiční přihlášení | Formulář obsahuje textová pole pro zadání e-mailu a hesla pro uživatele s nativním Gitcraft účtem. | Hráč / Tvůrce |
| **FR-03** | Primární herní integrace | Systém nabízí dvě výrazná, prioritní tlačítka pro rychlé přihlášení pomocí herního účtu (Minecraft/Microsoft) a platformy Modrinth. | Hráč / Tvůrce |
| **FR-04** | Sekundární přihlášení | V dolní části formuláře jsou k dispozici rychlé ikony pro přihlášení přes identity providery třetích stran (Google, Apple ID, Discord atd.). | Hráč / Tvůrce |

### Hlavní uživatelské rozhraní (Dashboard)
Po přihlášení je uživatel přesměrován na vizuální rozcestník projektů se zeleným herním motivem a čistou pracovní plochou.

| ID | Název požadavku | Popis požadavku | Hlavní role |
| :--- | :--- | :--- | :--- |
| **FR-05** | Přehled projektů (Dlaždice) | Systém zobrazuje projekty jako vizuální karty (dlaždice) obsahující název, typ, vlastní ikonu a čas poslední úpravy. | Hráč / Tvůrce |
| **FR-06** | Uživatelský profil a Leveling | V pravém horním rohu je zobrazen avatar uživatele. Po rozkliknutí ukáže detaily účtu a postup v komunitním leveling systému. | Hráč / Tvůrce |
| **FR-07** | Kontextová nabídka (Tři tečky) | Systém obsahuje schované hlavní menu v pravém horním rohu, které se po kliknutí animovaně rozbalí do kompletní nabídky aplikací. | Hráč / Tvůrce |

### Plovoucí navigační panel (Spodní menu)
Na spodní straně obrazovky je permanentně dostupné rychlé menu s kruhovými ikonami pro bleskový přístup k funkcím:

| ID | Název požadavku | Popis požadavku | Hlavní role |
| :--- | :--- | :--- | :--- |
| **FR-08** | Centrální akční tlačítko (+) | Výrazné středové tlačítko slouží k okamžitému vyvolání animované nabídky pro založení nového projektu. | Tvůrce |
| **FR-09** | Rychlá navigace: Domů | Ikona domečku vrátí uživatele z jakékoliv podstránky zpět na hlavní přehled projektů. | Hráč / Tvůrce |
| **FR-10** | Rychlá navigace: Žebříček | Ikona stupně vítězů otevře komunitní žebříček a detaily o získaných zkušenostech (XP) a úrovních. | Hráč / Tvůrce |
| **FR-11** | Rychlá navigace: Nastavení | Ozubené kolečko otevře rychlé nastavení aplikace, rozhraní a správy propojených účtů. | Hráč / Tvůrce |
| **FR-12** | Přepínač vzhledu (Měsíček) | Ikona měsíce/slunce umožňuje uživateli jedním kliknutím změnit vizuální téma aplikace. | Hráč / Tvůrce |

### Vytvoření nového projektu (Rychlé ikony)
Po stisknutí centrálního akčního tlačítka (+) se okolní prvky animovaně zanoří a do popředí vystoupí čtyři velké modré ikony pro výběr základního zaměření projektu.

| ID | Název požadavku | Popis požadavku | Hlavní role |
| :--- | :--- | :--- | :--- |
| **FR-13** | Animované zanoření dashboardu | Systém při aktivaci nového projektu vizuálně utlumí a posune stávající prvky dolů a plynule vykreslí rychlé ikony kategorií. | Tvůrce |
| **FR-14** | Rychlá ikona: Stavění | Nabídne dlaždici pro projekty primárně zaměřené na herní světy a mapy. | Tvůrce |
| **FR-15** | Rychlá ikona: Mody | Nabídne dlaždici pro správu klientských nebo serverových modifikací. | Tvůrce |
| **FR-16** | Rychlá ikona: Pluginy | Nabídne dlaždici pro vývoj a správu serverových pluginů. | Tvůrce |
| **FR-17** | Rychlá ikona: Resource Packy | Nabídne dlaždici pro správu texturových a zvukových balíčků. | Tvůrce |
| **FR-18** | Kombinovaná struktura projektu | Systém vnitřně umožní, aby jeden projekt obsahoval více typů dat najednou (např. Stavbu i Mod současně). | Tvůrce |

### Pokročilý průvodce tvorbou (Okno podle Canvy)
Ať už uživatel klikne na jakoukoliv z předchozích čtyř rychlých ikon, systém otevře celoobrazovkové modální okno s detailním katalogem šablon a podkategorií.

| ID | Název požadavku | Popis požadavku | Hlavní role |
| :--- | :--- | :--- | :--- |
| **FR-19** | Zavření průvodce (Křížek) | Okno obsahuje v pravém horním rohu křížek pro bezpečné stornování akce a návrat na dashboard. | Tvůrce |
| **FR-20** | Hierarchické levé menu | Levý sloupec zobrazuje hlavní kategorie (Stavění, Mody, Pluginy, Resource Packy). Kategorie, na kterou uživatel klikl, se automaticky rozbalí a ukáže podkategorie menším písmem. | Tvůrce |
| **FR-21** | Podkategorie pro Stavění | Pod hlavní položkou Stavění se zobrazí specifické filtry: Mapy, Escape Rooms, Redstone, Domy a ikona/tlačítko „Další“. | Tvůrce |
| **FR-22** | Volba „Vytvořit vlastní“ | V pravé hlavní části okna je na prvním místě vždy umístěna možnost začít na zelené louce (zcela čistý nový projekt). | Tvůrce |
| **FR-23** | Katalog Blueprintů (Šablon) | Pravá část okna nabízí vizuální přehled hotových blueprintů a komunitních základů práce, které může uživatel jedním kliknutím zkopírovat (forknout) a začít z nich stavět vlastní verzi. | Tvůrce |

## 2. Nefunkční požadavky (NFR)

| ID | Název požadavku | Popis a kritérium | Typ požadavku |
| :--- | :--- | :--- | :--- |
| **NFR-01** | Podpora tmavého režimu | Uživatelské rozhraní musí plně podporovat světlé i tmavé (Dark mode) zobrazení pro pohodlnou práci v noci. | Použitelnost (UI/UX) |
| **NFR-02** | Plynulost animací rozhraní | Všechny přechody (včetně zanoření prvků při kliknutí na +) musí běžet plynule bez záseků (cíl 60 FPS). | Výkon / Použitelnost |
