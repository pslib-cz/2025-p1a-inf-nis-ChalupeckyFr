# Specifikace požadavků systému Gitcraft (requirements.md)

Tento dokument obsahuje kompletní přehled funkčních a nefunkčních požadavků pro platformu Gitcraft – vizuální nástroj pro správu verzí, zálohování a kolaboraci v prostředí hry Minecraft.

---

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

### Konfigurace nového projektu (Nastavení)
Při zakládání vlastního projektu nebo editaci blueprintu se otevře konfigurační okno s předpřipravenými výchozími hodnotami (placeholdery).

| ID | Název požadavku | Popis požadavku | Hlavní role |
| :--- | :--- | :--- | :--- |
| **FR-24** | Dynamický výchozí název | Pokud uživatel nezadá název, systém automaticky vygeneruje název podle formátu: „Nový [Typ] projekt #[Číslo]“ (např. *Nový stavební projekt #1*). | Tvůrce |
| **FR-25** | Nezávislé počítadlo projektů | Systém interně eviduje pořadové číslo projektu samostatně pro každou kategorii (první stavba i první plugin budou mít shodně index #1). | Tvůrce |
| **FR-26** | Možnost skrytí indexu (#) | V nastavení řádku s názvem projektu je k dispozici přepínač, který umožní zobrazení pořadového čísla (#) v rozhraní vypnout. | Tvůrce |

### Spolupracovníci a Správa rolí (Kolaborace)
Systém umožňuje sdílení projektů s dalšími uživateli a definování jejich přístupových práv.

| ID | Název požadavku | Popis požadavku | Hlavní role |
| :--- | :--- | :--- | :--- |
| **FR-27** | Pozvání spolupracovníků | Uživatel může do projektu pozvat další lidi pomocí e-mailu, telefonního čísla nebo Gitcraft přezdívky. | Vlastník / Admin |
| **FR-28** | Role: Admin | Uživatel s touto rolí může měnit kritická nastavení (název, soukromí) a schvalovat odeslané změny do projektu. | Vlastník / Admin |
| **FR-29** | Role: Pomocník (Tvůrce) | Může lokálně upravovat projekt (stavět/kódovat) a ukládat své verze, které však podléhají schválení Adminem. | Pomocník |
| **FR-30** | Role: Návštěvník | Má právo pouze k prohlížení projektu (Read-only) bez možnosti provádět změny. | Návštěvník |
| **FR-31** | Granulární zámek složek | Admin může ručně omezit přístup (skrýt) konkrétní složky nebo soubory projektu před Návštěvníky. | Vlastník / Admin |
| **FR-32** | Vizuální schvalování změn (Block-Diff) | Při schvalování změn u staveb systém zobrazí přehled upravených bloků s možností přijmout vše, nepřijmout nic, nebo schválit jen vybrané části. | Vlastník / Admin |

### Správa soukromí (Privacy)
Nastavení viditelnosti celého projektu pro okolní svět.

| ID | Název požadavku | Popis požadavku | Hlavní role |
| :--- | :--- | :--- | :--- |
| **FR-33** | Výchozí soukromí (Private) | Každý nově vytvořený projekt je automaticky nastaven jako skrytý (Soukromý), přístupný pouze autorovi. | Tvůrce |
| **FR-34** | Veřejný projekt (Public) | Možnost přepnout projekt do režimu, kdy ho může vyhledat a prohlížet jakýkoliv uživatel platformy Gitcraft. | Vlastník / Admin |
| **FR-35** | Sdílení s přáteli | Možnost omezit viditelnost projektu pouze na uživatele, které má vlastník v Gitcraft seznamu přátel. | Vlastník / Admin |

### Technické nastavení projektu (Verze a Zálohy)
Konfigurační řádky pro definování herního prostředí a způsobu ukládání dat.

| ID | Název požadavku | Popis požadavku | Hlavní role |
| :--- | :--- | :--- | :--- |
| **FR-36** | Výběr verze Minecraftu | Možnost zvolit cílovou verzi hry (např. 1.21). Výchozí hodnotou je nejnovější stabilní vydaná verze. | Tvůrce |
| **FR-37** | Výběr herního jádra (Loader) | For mody a pluginy umožňuje zvolit platformu (Forge, Fabric, Paper atd.). Výchozí hodnota se adaptuje podle zvoleného typu projektu. | Tvůrce |
| **FR-38** | Interval auto-zálohování | Nastavení frekvence automatického ukládání na pozadí. Výchozí hodnota je nastavena na 30 minut. | Tvůrce |
| **FR-39** | Cíl zálohy (Lokální vs. Cloud) | Uživatel si zvolí, zda chce verze ukládat pouze lokálně na disk (s volbou konkrétní složky), nebo synchronizovat na bezpečný Gitcraft cloud server. | Tvůrce |
| **FR-40** | Pokročilé nastavení (Licence) | Skrytá sekce pro pokročilé uživatele, kde lze u veřejných projektů definovat typ autorské licence (např. Open-source vs. Chráněno autorským právem). | Tvůrce |

### Vizuální identita (Náhledový obrázek)
Prvek umístěný vedle názvu projektu pro rychlou vizuální orientaci v dashboardu.

| ID | Název požadavku | Popis požadavku | Hlavní role |
| :--- | :--- | :--- | :--- |
| **FR-41** | Manuální náhledový obrázek | Uživatel může k projektu nahrát jakýkoliv vlastní obrázek z počítače jako ikonu projektu. | Tvůrce |
| **FR-42** | Automatický screenshot zpod kapoty | Systém nabízí možnost automaticky vygenerovat náhledový obrázek z poslední uložené pozice (poslední pohled postavy na testovacím serveru nebo ve světě). | Tvůrce |

---

## 2. Nefunkční požadavky (NFR)

| ID | Název požadavku | Popis a kritérium | Typ požadavku |
| :--- | :--- | :--- | :--- |
| **NFR-01** | Podpora tmavého režimu | Uživatelské rozhraní musí plně podporovat světlé i tmavé (Dark mode) zobrazení pro pohodlnou práci v noci. | Použitelnost (UI/UX) |
| **NFR-02** | Plynulost animací rozhraní | Všechny přechody (včetně zanoření prvků při kliknutí na +) must běžet plynule bez záseků (cíl 60 FPS). | Výkon / Použitelnost |
