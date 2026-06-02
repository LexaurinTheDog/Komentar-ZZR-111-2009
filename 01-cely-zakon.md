# Komentář k zákonu č. 111/2009 Sb., o základních registrech (ZZR)

> **Téma zákona:** ZZR zřizuje **čtyři základní registry** (registr obyvatel — ROB, registr osob — RPO, registr územní identifikace — RUIAN, registr práv a povinností — RPP) a zavádí institut **referenčního údaje** jako jediného platného a závazného údaje ve veřejné správě ČR. Architektonickou páteří je **referenční rozhraní** tvořené **Informačním systémem základních registrů (ISZR)** a **Informačním systémem sdílené služby (ISSS)**, jejichž správcem je **Digitální a informační agentura (DIA)**. Zákon zavádí **agendový princip** přístupu k údajům: orgán veřejné moci přistupuje k údajům výhradně prostřednictvím **agendového informačního systému (AIS)** v rámci registrované **agendy** a přidělené **role**. Bezpečnostním jádrem systému je **ORG** (převodník identifikátorů), jenž zaručuje, že žádný subjekt nemůže propojovat osobní údaje napříč agendami bez zákonné opory — tuto pravomoc má výhradně **Úřad pro ochranu osobních údajů** prostřednictvím zdrojového identifikátoru fyzické osoby. Klíčové instituty: **referenční údaj** (§ 4) s domněnkou správnosti, **editor** odpovědný za zápis, **referenční vazby** mezi registry, **agendový identifikátor fyzické osoby (AIFO)** odvozený ze zdrojového identifikátoru (§ 9–11), **reklamace** referenčních údajů (§ 14 odst. 6), **dohled DIA a ÚOOÚ**.

---

## ČÁST PRVNÍ — ZÁKLADNÍ REGISTRY

## HLAVA I — Obecná ustanovení

### § 1 — Předmět úpravy

> **§ 1**
>
> *Tento zákon*
>
> *- a) zřizuje základní registry a některé další informační systémy veřejné správy a stanoví působnosti, práva a povinnosti, které souvisejí s jejich vytvářením, správou, provozem a užíváním,*
>
> *- b) stanovuje podmínky pro sdílení údajů mezi základními registry navzájem, základními registry a agendovými informačními systémy, základními registry a informačními systémy soukromoprávních uživatelů údajů umožňujícími využívání údajů ze základních registrů nebo agendových informačních systémů (dále jen „soukromoprávní systém pro využívání údajů"), agendovými informačními systémy navzájem a mezi agendovými informačními systémy a soukromoprávními systémy pro využívání údajů.*

**Výklad:**

#### Dvojí předmět úpravy — zřízení a sdílení

§ 1 vymezuje předmět ZZR ve dvou rovinách. **Písmeno a)** zakládá **zřizovací funkci** zákona — ZZR sám o sobě je zákonem zřizujícím čtyři základní registry (taxativně vyjmenované v § 3) a další podpůrné informační systémy (ISZR, ISSS, autentizační IS, IS oprávnění k zastupování, IS územní identifikace, IS registru práv a povinností). Současně určuje subjekty, jimž svěřuje konkrétní působnosti.

**Písmeno b)** zakládá **funkci sdílecí** — zákon stanoví podmínky, za nichž mohou být údaje vedené v jednom systému využívány v systému jiném. Tím vytváří „**referenční rozhraní**" ve smyslu § 2 písm. i) ZISVS, tedy unifikovanou vrstvu, přes kterou musí veškeré sdílení procházet.

Pět typů sdílení uvedených v písmenu b) tvoří **kompletní matici výměny údajů ve veřejné správě**:

1. **ZR ↔ ZR** — mezi základními registry navzájem (např. referenční vazba mezi ROB a RUIAN přes kód adresního místa).
2. **ZR ↔ AIS** — mezi základním registrem a agendovým informačním systémem (např. ROB ↔ AIS evidence obyvatel).
3. **ZR ↔ soukromoprávní systém** — sdílení do soukromé sféry (banky, pojišťovny, advokáti se zvláštním zákonným titulem).
4. **AIS ↔ AIS** — mezi agendovými systémy (např. AIS Policie ČR ↔ AIS živnostenského úřadu).
5. **AIS ↔ soukromoprávní systém** — sdílení mezi AIS a soukromou sférou.

Toto vymezení je významné z hlediska **zákonné rezervace**: žádné sdílení mimo tuto matici a mimo referenční rozhraní není podle ZZR přípustné. Veškeré sdílení musí jít přes ISZR nebo ISSS, ledaže výslovně ZZR stanoví jinak (typicky § 5b — přímý přístup pro účely národní bezpečnosti).

#### Postavení ZZR v právním řádu

ZZR není „kodexem informačního práva veřejné správy"; tím zůstává zákon č. 365/2000 Sb., o ISVS. ZZR je **lex specialis** vůči ZISVS pro úzce vymezenou oblast — vedení referenčních údajů ve čtyřech základních registrech. Pro otázky ZZR výslovně neupravené (zveřejňování ISVS, atestace, povinnosti správce ISVS obecně) platí podpůrně ZISVS.

---

### § 2 — Obecné pojmy

> **§ 2**
>
> *V tomto zákoně se rozumí*
>
> *- a) základním registrem informační systém veřejné správy1) uvedený v § 3,*
>
> *- b) referenčním údajem údaj vedený v základním registru, který je označen jako referenční údaj,*
>
> *- c) orgánem veřejné moci státní orgán, územní samosprávný celek, fyzická nebo právnická osoba, byla-li jí svěřena působnost v oblasti veřejné správy, notář, soudní exekutor, insolvenční správce a archiv,*
>
> *- d) soukromoprávním uživatelem údajů podnikající fyzická osoba nebo právnická osoba, která je podle jiného právního předpisu oprávněna využívat údaje ze základního registru nebo z agendového informačního systému, pro působení, které není působením orgánu veřejné moci,*
>
> *- e) agendou ucelená oblast působení orgánu veřejné moci nebo ucelená oblast působení soukromoprávního uživatele údajů,*
>
> *- f) agendovým informačním systémem informační systém veřejné správy, který slouží k výkonu agendy, využívání elektronických formulářů nebo elektronické identifikaci,*
>
> *- g) informačním systémem základních registrů informační systém veřejné správy, který je součástí referenčního, sdíleného a bezpečného rozhraní informačních systémů veřejné správy54) (dále jen „referenční rozhraní“) a jehož prostřednictvím je zajišťováno sdílení údajů mezi základními registry navzájem, základními registry a agendovými informačními systémy, základními registry a soukromoprávními systémy pro využívání údajů, agendovými informačními systémy, jejichž prostřednictvím se zapisují údaje do základních registrů, a jinými agendovými informačními systémy a mezi agendovými informačními systémy, jejichž prostřednictvím se zapisují údaje do základních registrů, a soukromoprávními systémy pro využívání údajů, správa oprávnění přístupu k údajům a další činnosti podle tohoto zákona,*
>
> *- h) informačním systémem sdílené služby informační systém veřejné správy, který je součástí referenčního rozhraní a jehož prostřednictvím je zajišťováno sdílení údajů mezi agendovými informačními systémy, jejichž prostřednictvím se nezapisují údaje do základních registrů, navzájem, a mezi agendovými informačními systémy, jejichž prostřednictvím se nezapisují údaje do základních registrů, a soukromoprávními systémy pro využívání údajů, správa oprávnění přístupu k údajům a další činnosti podle tohoto zákona,*
>
> *- i) editorem orgán veřejné moci, který je oprávněn zapisovat údaje do základního registru nebo agendového informačního systému a provádět změny zapsaných údajů.*

**Výklad:**

§ 2 obsahuje **legální definice** základních pojmů ZZR. Definice vytváří mikrojazyk zákona — pojmy zde vymezené jsou v textu používány ve striktně právním významu, nikoli v běžném jazykovém smyslu.

#### Základní registr (písm. a)) — formální definice

Definice je čistě **odkazová**: základní registr je to, co § 3 jako základní registr označuje. Toto formální vymezení má klíčový význam — **počet a okruh základních registrů je taxativně určen zákonem**, žádný registr nemůže být „povýšen" na základní registr výkladem ani podzákonným předpisem. Rozšíření okruhu základních registrů by vyžadovalo novelu § 3.

Materiální vlastnosti „základnosti" plynou z dalších ustanovení: registr musí být veden v souladu s referenčním rozhraním, jeho údaje musí být sdílitelné v matici § 1 písm. b), a jeho referenční údaje mají vlastnosti podle § 4.

#### Referenční údaj (písm. b)) — jediný platný údaj v ČR

**Klíčový institut zákona.** Referenční údaj je definován dvěma podmínkami: (i) je veden v základním registru, (ii) je tam **označen** jako referenční. Toto označení není akademickým atributem, nýbrž zakládá **zvláštní právní režim** — viz § 4 odst. 4 až 7 (domněnka správnosti, dobrá víra, ochrana důvěry).

Pojem referenčního údaje obrací logiku dosavadní veřejné správy: dosud platil princip, že každá evidence vede „své" údaje, které úřad ověřuje. Po nabytí účinnosti ZZR platí, že **referenční údaj je v ČR jediný platný a závazný** — orgán veřejné moci jej nesmí ověřovat, ledaže má oprávněnou pochybnost (§ 5 odst. 2).

#### Orgán veřejné moci (písm. c)) — extenzivní pojem

Definice je **širší** než definice správního orgánu podle správního řádu. Zahrnuje:

1. **Státní orgány** — moc zákonodárná, výkonná, soudní; ústřední správní úřady, jiné správní úřady, soudy.
2. **Územní samosprávné celky** — obce a kraje (v rámci samostatné i přenesené působnosti).
3. **Fyzické a právnické osoby s veřejnou působností** — typicky veřejnoprávní korporace, profesní komory s výkonem veřejné správy (advokátní komora v kárných věcech, lékařská komora apod.).
4. **Notáři, soudní exekutoři, insolvenční správci** — výslovně zahrnuti; jde o privatizované výseky výkonu veřejné moci.
5. **Archivy** — výslovně zahrnuty; navazuje na zákon č. 499/2004 Sb., o archivnictví a spisové službě.

> **Srovnání:** § 1 odst. 1 správního řádu vymezuje správní orgán šířeji jako „orgán moci výkonné, orgán územního samosprávného celku a jiný orgán, právnická nebo fyzická osoba, pokud vykonávají působnost v oblasti veřejné správy". ZZR užívá širší pojem „orgán veřejné moci", do něhož spadají i soudy, k nimž působnost správního řádu nedopadá.

#### Soukromoprávní uživatel údajů (písm. d)) — výjimečný přístup soukromé sféry

Soukromoprávní uživatel je **podnikající FO nebo PO**, která je **zvláštním zákonem** oprávněna využívat údaje ze ZR nebo AIS. Typickými příklady jsou:

1. **Banky** (§ 38a zákona č. 21/1992 Sb., o bankách) — pro splnění povinností podle AML zákona a podle úvěrového procesu.
2. **Pojišťovny** — pro identifikaci klientů.
3. **Provozovatelé soukromých systémů elektronické identifikace** podle zákona č. 250/2017 Sb., o elektronické identifikaci.

Pojem **„pro působení, které není působením orgánu veřejné moci"** odlišuje soukromoprávního uživatele od situace, kdy soukromá osoba vykonává svěřenou veřejnou moc (typicky advokátní komora) — v takovém případě by šlo o orgán veřejné moci podle písm. c).

#### Agenda (písm. e)) — funkční pojem

**Agenda** je „ucelená oblast působení". Pojem **není totožný** s pojmem agendy podle ZISVS — zde má autonomní význam. Agenda zpravidla odpovídá jednomu zákonu nebo jeho části (např. agenda evidence obyvatel podle zákona č. 133/2000 Sb., agenda občanských průkazů, agenda cestovních dokladů, agenda živnostenského podnikání).

Agenda je **registrační jednotka** přístupu k údajům. Bez registrované agendy (§ 53–54) a bez zaregistrování pro výkon agendy (§ 55) nemůže žádný orgán veřejné moci do referenčního rozhraní vstoupit.

Důležitým rysem je, že agenda může být vykonávána i **soukromoprávním uživatelem** — typicky agenda identifikace klienta podle AML zákona.

#### Agendový informační systém (písm. f)) — brána do registrů

**AIS** je IS veřejné správy, který slouží k:

1. **výkonu agendy** (typický případ — např. AIS evidence obyvatel),
2. **využívání elektronických formulářů** (např. portál veřejné správy),
3. **elektronické identifikaci** (např. národní bod pro identifikaci a autentizaci).

AIS plní v architektuře ZZR roli **mediátoru**: orgán veřejné moci **nemůže** přistoupit k základnímu registru přímo, nýbrž musí jít přes AIS, který je k základnímu registru napojen prostřednictvím ISZR (§ 5 odst. 5). Tím se zajišťuje, že každý přístup je rozlišitelný podle agendy, role a uživatele.

#### Informační systém základních registrů a sdílené služby (písm. g) a h))

**ISZR** je páteřní integrační systém pro výměnu údajů **se zapojením základních registrů** (zápis i čtení). **ISSS** je obdobou pro AIS, které **nezapisují** do základních registrů a chtějí jen sdílet mezi sebou nebo se soukromou sférou. Oba jsou součástí **referenčního rozhraní** podle § 2 písm. i) zákona č. 365/2000 Sb..

Správcem obou systémů je **Digitální a informační agentura (DIA)** (§ 7 odst. 1).

#### Editor (písm. i)) — odpovědný zapisovatel

**Editor** je orgán veřejné moci s pravomocí zapisovat a měnit údaje v ZR nebo AIS. Klíčové vlastnosti:

1. **Výlučnost** — pro každý referenční údaj je editorem zákonem určený jeden orgán (např. pro adresu v ROB je to obecní úřad obce s rozšířenou působností přes zákon o evidenci obyvatel).
2. **Odpovědnost** — editor odpovídá za soulad zapsaných údajů se zdrojovými dokumenty (§ 4 odst. 2).
3. **Časový limit** — editor zapíše bez zbytečného odkladu, nejpozději do 3 pracovních dnů (§ 4 odst. 3 — pro ZR), resp. 10 pracovních dnů (§ 4a odst. 3 — pro AIS).

---

### § 3 — Základní registry

> **§ 3**
>
> *Základními registry jsou*
>
> *- a) základní registr obyvatel (dále jen „registr obyvatel"),*
>
> *- b) základní registr právnických osob, podnikajících fyzických osob a orgánů veřejné moci (dále jen „registr osob"),*
>
> *- c) základní registr územní identifikace, adres a nemovitostí (dále jen „registr územní identifikace"),*
>
> *- d) základní registr agend, orgánů veřejné moci, soukromoprávních uživatelů údajů a některých práv a povinností (dále jen „registr práv a povinností").*

**Výklad:**

§ 3 obsahuje **taxativní výčet** čtyř základních registrů. Výčet je **uzavřený** — žádný další registr nelze povýšit na základní bez novely tohoto ustanovení.

| Plný název | Legislativní zkratka | Běžná zkratka | Předmět |
|---|---|---|---|
| Základní registr obyvatel | registr obyvatel | **ROB** | Fyzické osoby s pobytem v ČR |
| Základní registr právnických osob, podnikajících fyzických osob a orgánů veřejné moci | registr osob | **ROS / RPO** | Právnické osoby, OSVČ, OVM |
| Základní registr územní identifikace, adres a nemovitostí | registr územní identifikace | **RUIAN** | Územní prvky, adresy, stavební objekty |
| Základní registr agend, orgánů veřejné moci, soukromoprávních uživatelů údajů a některých práv a povinností | registr práv a povinností | **RPP** | Agendy, OVM, role, oprávnění |

#### Koncepční logika čtyřkové struktury

Čtyři registry tvoří **vzájemně se doplňující datovou síť**:

- **ROB** odpovídá na otázku *„Kdo je to?"* — identifikuje fyzickou osobu.
- **Registr osob** odpovídá na otázku *„Jaký je to subjekt?"* — identifikuje právnické osoby, podnikatele a orgány veřejné moci.
- **RUIAN** odpovídá na otázku *„Kde to je?"* — identifikuje místo v prostoru.
- **RPP** odpovídá na otázku *„Co kdo dělá a smí?"* — popisuje agendy, oprávnění, právní stavy.

Tato čtyřdimenzionální struktura (osoba × subjekt × místo × oprávnění) pokrývá veškerou základní agendovou činnost veřejné správy.

#### Vzájemné vazby

Registry jsou propojeny **referenčními vazbami** — kódy odkazujícími z jednoho registru do druhého:

- ROB → RUIAN: adresa místa pobytu fyzické osoby je v ROB vedena jako kód adresního místa odkazující na RUIAN.
- ROS → RUIAN: adresa sídla osoby a místa provozovny.
- ROS → ROB: jméno fyzické osoby OSVČ je referenční vazbou na ROB.
- RPP → ROS / ROB: identifikátor OVM nebo soukromoprávního uživatele.

Žádný registr neuchovává „kopii" údaje druhého registru — vždy jen **referenční vazbu** (kód, identifikátor). To zajišťuje konzistenci: změna v jednom registru se okamžitě projevuje ve všech ostatních.

#### Pojmová past — „RPO" vs „RPP"

V odborné praxi se užívá zkratka **RPO** (Registr Právnických Osob) pro registr osob podle písm. b), zatímco **RPP** označuje registr práv a povinností podle písm. d). Tato dvě označení znějí podobně, ale označují různé registry. Zákon sám zkratky nepoužívá — pracuje s legislativními zkratkami „registr osob" a „registr práv a povinností". V tomto komentáři dodržuji konvenci běžné praxe a používám zkratky ROB, ROS/RPO, RUIAN, RPP.

---

### § 4 — Údaje základního registru

> **§ 4**
>
> *(1) Základní registr obsahuje referenční údaje, referenční vazby, identifikátory fyzických osob, popřípadě autentizační údaje, provozní údaje a jiné zákonem stanovené údaje. Referenční vazby jsou kódy nebo identifikátory, kterými je odkazováno na referenční údaje v základních registrech. Autentizační údaje jsou údaje umožňující provést ověření identity fyzické osoby.*
>
> *(2) Editor je zodpovědný za to, že jím zapsané referenční údaje jsou v souladu s údaji uvedenými v dokumentech, na jejichž základě jsou referenční údaje do příslušného základního registru zapsány; orgány veřejné moci, fyzické a právnické osoby jsou povinny poskytnout editorovi potřebnou součinnost k plnění jeho úkolů tím, že mu poskytnou údaje a podklady potřebné pro ověření správnosti zapisovaných referenčních údajů.*
>
> *(3) Editor zapíše referenční údaj do základního registru nebo provede jeho změnu bez zbytečného odkladu, nejpozději však do 3 pracovních dnů ode dne, kdy se o vzniku nebo o změně skutečnosti, kterou referenční údaj popisuje, dozví.*
>
> *(4) Referenční údaj je považován za správný, pokud není prokázán opak nebo pokud nevznikne oprávněná pochybnost o správnosti referenčního údaje. V případě pochybnosti editor nebo správce základního registru označí referenční údaj jako nesprávný; toto označení editor odstraní neprodleně poté, co ověří správnost údajů, jinak se postupuje obdobně podle odstavce 3.*
>
> *(5) Referenční údaj označený jako nesprávný má po dobu, po kterou je takto označen, pouze informativní povahu.*
>
> *(6) Má se za to, že ten, kdo vychází z referenčního údaje, je v dobré víře, že stav referenčního údaje odpovídá skutečnému stavu věci, ledaže musel vědět o jeho nesprávnosti.*
>
> *(7) Proti tomu, kdo jedná v důvěře ve správnost referenčního údaje, nemůže ten, jehož se referenční údaj týká, namítat, že referenční údaj neodpovídá skutečnosti, ledaže prokáže, že referenční údaj je nesprávný a že jeho nesprávnost nezpůsobil.*

**Výklad:**

§ 4 je **centrálním ustanovením celého zákona**. Stanoví obsahovou strukturu základního registru a — především — zakotvuje **právní režim referenčního údaje**: domněnku správnosti, povinnosti editora, ochranu dobré víry a zákaz namítání nesprávnosti vůči poctivému uživateli.

#### Pět kategorií údajů v základním registru (odst. 1)

1. **Referenční údaje** — jádro registru, údaje s plnou závazností.
2. **Referenční vazby** — kódy/identifikátory odkazující na referenční údaje v jiných registrech (např. kód adresního místa v ROB odkazuje na RUIAN).
3. **Identifikátory fyzických osob** — agendové a zdrojové identifikátory (§ 9–11).
4. **Autentizační údaje** — údaje umožňující ověření identity (např. data pro elektronickou identifikaci podle § 18 odst. 1 písm. n)).
5. **Provozní údaje** — záznamy o využití registru, datum poslední změny apod. (§ 18 odst. 5, § 26 odst. 4, § 51 odst. 5).

A dále **„jiné zákonem stanovené údaje"** — otevřená kategorie pro budoucí rozšíření.

> **Klíčové rozlišení:** **referenční údaj** má plnou závaznost a domněnku správnosti. **Provozní údaj** (čas přístupu, kód uživatele) nemá závaznost referenčního údaje a slouží k audit-trailu. **Autentizační údaj** je technickou pomůckou pro ověření identity, nikoli substantivním údajem o osobě.

#### Odpovědnost editora (odst. 2)

Editor odpovídá za **soulad zapsaného údaje se zdrojovým dokumentem** — nikoli za pravdivost zdrojového dokumentu. Editor není povinen verifikovat skutečnost (např. zda osoba opravdu bydlí na zapsané adrese); odpovídá jen za to, že to, co je v podkladovém dokumentu (občanském průkazu, listině o trvalém pobytu), je věrně zapsáno do registru.

Druhá věta zakládá **povinnost součinnosti** všech orgánů veřejné moci a osob — kdo má podklady relevantní pro správnost zápisu, je povinen je editorovi poskytnout. Tato povinnost je sankcionována nepřímo přes regulaci v jiných předpisech (pokuty za nesplnění oznamovací povinnosti).

#### Lhůta tří pracovních dnů (odst. 3)

Editor je povinen zapsat údaj nebo provést změnu **bez zbytečného odkladu, nejpozději do 3 pracovních dnů** ode dne, kdy se o vzniku nebo změně skutečnosti dozví. Tato lhůta je **maximální** — primární pravidlo je „bez zbytečného odkladu", tedy v praxi často okamžitě.

Lhůta je významně **kratší** než lhůta 10 pracovních dnů pro AIS (§ 4a odst. 3) — odráží mimořádný význam referenčního údaje.

#### Domněnka správnosti (odst. 4) — jádro referenčního principu

Odst. 4 zakládá **vyvratitelnou domněnku správnosti referenčního údaje**. Domněnka je vyvrácena dvěma způsoby:

1. **Důkaz opaku** — někdo prokáže, že údaj je nesprávný.
2. **Oprávněná pochybnost** — vznikne důvodné podezření, že údaj neodpovídá skutečnosti, byť není ještě plně prokázáno.

V obou případech **editor nebo správce ZR údaj označí jako nesprávný**. Po dobu trvání označení má údaj jen **informativní povahu** (odst. 5) — neuplatňují se na něj domněnka správnosti ani ochrana důvěry.

#### Ochrana dobré víry (odst. 6) a ochrana poctivého uživatele (odst. 7)

Tato dvě ustanovení tvoří **trojrozměrnou ochranu**:

- **Odst. 4** — kdo z údaje vychází, ten z něj „smí" vycházet (vyloučení sankce za nesprávnost údaje).
- **Odst. 6** — kdo z údaje vychází, **je v dobré víře** (vyvratitelná domněnka dobré víry). Vyvrácení je možné jen důkazem, že vědom o nesprávnosti **vědět musel**.
- **Odst. 7** — proti tomu, kdo jednal v důvěře, **nelze namítat** nesprávnost — leda by ten, jehož se údaj týká, prokázal, že (i) údaj **je nesprávný** a současně (ii) **nesprávnost nezpůsobil**.

> **Příklad:** Banka poskytne úvěr osobě A, která se prokázala občanským průkazem, jehož data jsou v souladu s ROB. Později vyjde najevo, že osoba A je ve skutečnosti osoba B (záměna identity způsobená chybou MV při zápisu do ROB). Banka jednala v důvěře v referenční údaj — má presumpci dobré víry (odst. 6) a osoba B nemůže namítat, že údaj v ROB neodpovídal skutečnosti (odst. 7). Banka má nárok na ochranu právních účinků své transakce.

> **Srovnání s materiálním principem veřejnoprávních evidencí v civilním právu:** § 980 a násl. občanského zákoníku zavádí obdobnou ochranu důvěry ve veřejné seznamy (katastr nemovitostí). Konstrukce ZZR je obdobná, ale zaměřená na sféru veřejné správy — nikoli na civilněprávní účinky.

---

### § 4a — Údaje agendového informačního systému

> **§ 4a**
>
> *(1) Agendový informační systém obsahuje údaje, které se vytvářejí nebo využívají při výkonu agendy nebo při správě a provozování agendového informačního systému.*
>
> *(2) Údaj do agendového informačního systému zapisuje editor po vytvoření údaje při výkonu agendy nebo se využije ze základního registru nebo z jiného agendového informačního systému.*
>
> *(3) Editor zapíše údaj do agendového informačního systému nebo provede jeho změnu bez zbytečného odkladu, nejpozději však do 10 pracovních dnů ode dne, kdy se dozví o vzniku nebo o změně skutečnosti, kterou údaj popisuje.*

**Výklad:**

§ 4a paralelně k § 4 upravuje pravidla pro **agendové informační systémy** (AIS). Rozdíl proti ZR:

1. **AIS nemá referenční údaje** — vede údaje, které vznikají při výkonu agendy, nikoli referenční údaje s domněnkou správnosti.
2. **Delší lhůta zápisu** — 10 pracovních dnů místo 3 (odst. 3).
3. **Možnost znovuvyužití** — údaj může do AIS vstoupit buď zápisem editora, nebo automaticky z jiného ZR/AIS přes referenční rozhraní (odst. 2).

§ 4a byl do zákona vložen zákonem č. 12/2020 Sb., o právu na digitální služby — předtím ZZR pravidla pro AIS výslovně neupravoval a spoléhal na obecnou úpravu ZISVS. Nová úprava sjednocuje pravidla zápisu napříč celou infrastrukturou eGovernmentu.

---

### § 5 — Využívání údajů orgánem veřejné moci

> **§ 5**
>
> *(1) Orgán veřejné moci využívá údaje vedené v základním registru nebo agendovém informačním systému v rozsahu potřebném k provedení úkonu orgánu veřejné moci a v rámci výčtu údajů zpřístupněných orgánu veřejné moci pro výkon agendy, v jejímž rámci je úkon orgánu veřejné moci prováděný a pro jejíž výkon je orgán veřejné moci registrovaný.*
>
> *(2) Orgán veřejné moci využívá údaje vedené v základním registru nebo údaje vedené v agendovém informačním systému, které nejsou ve tvaru předcházejícím současný stav, aniž by ověřoval jejich správnost. Od osob, po kterých je jiným právním předpisem požadováno doložení údajů vedených v základním registru nebo agendovém informačním systému, je orgán veřejné moci oprávněn požadovat poskytnutí takových údajů pouze, pokud*
>
> *- a) nejsou obsaženy ve výčtu údajů zpřístupněných orgánu veřejné moci pro výkon agendy,*
>
> *- b) jsou označeny jako nesprávné,*
>
> *- c) vznikne oprávněná pochybnost o správnosti údaje, nebo*
>
> *- d) jsou nezbytné pro bezpečnostní řízení podle jiného právního předpisu.*
>
> *(3) Orgán veřejné moci využívá údaje vedené v agendovém informačním systému, které jsou vedeny jako referenční údaje v základním registru, pouze pokud jsou ve tvaru předcházejícím současný stav.*
>
> *(4) V případě, že orgán veřejné moci, který není editorem údaje vedeného v základním registru nebo agendovém informačního systému, při své činnosti zjistí nesoulad údaje vedeného v základním registru nebo agendovém informačním systému se skutečným stavem, anebo vznikne-li u něj oprávněná pochybnost o správnosti údaje, uvědomí o tom neprodleně editora daného údaje.*
>
> *(5) Orgán veřejné moci využívá údaje vedené v základním registru nebo údaje do základního registru zapisuje prostřednictvím agendového informačního systému; jeho přístup k údajům vedeným v základním registru je zajišťován službami informačního systému základních registrů. Orgán veřejné moci využívá údaje vedené v agendovém informačním systému prostřednictvím služeb tohoto agendového informačního systému; není-li orgán veřejné moci současně správcem tohoto agendového informačního systému, je jeho přístup k údajům vedeným v agendovém informačním systému zajišťován službami informačního systému sdílené služby. Orgán veřejné moci zapisuje údaje do agendového informačního systému prostřednictvím služeb tohoto agendového informačního systému.*

**Výklad:**

§ 5 stanoví **pravidla využití referenčních a agendových údajů** orgánem veřejné moci. Toto ustanovení je v každodenní praxi nejvíce frekventované — formuluje **zásadu „neptej se občana, co stát už ví"**.

#### Zásada účelového omezení a omezení rolí (odst. 1)

Orgán veřejné moci využívá údaje pouze:

1. **v rozsahu potřebném k provedení úkonu** — princip minimalizace (odpovídá čl. 5 odst. 1 písm. c) GDPR);
2. **v rámci výčtu údajů zpřístupněných pro výkon agendy** — výčet je dán registrací agendy v RPP (§ 51 odst. 6 písm. l));
3. **pro agendu, v jejímž rámci je úkon prováděn** — princip vázanosti na agendu;
4. **pro kterou je orgán veřejné moci registrovaný** — princip vázanosti na registraci (§ 55).

Tato čtyřnásobná vazba znamená, že žádný orgán veřejné moci nemá „univerzální přístup". Jakékoli porušení (přístup k údaji mimo agendu, mimo registraci) je **nezákonným zpracováním osobních údajů** ve smyslu GDPR a ZZR.

#### Zákaz duplicitního dokládání (odst. 2) — jádro principu „write once"

Odst. 2 zakotvuje klíčové pravidlo: **orgán veřejné moci nesmí požadovat od osoby doložení toho, co je v referenčních údajích.** Výjimky jsou jen čtyři:

- **a) Údaj není zpřístupněn** pro agendu — orgán k němu nemá přístup, takže si jej musí vyžádat od osoby.
- **b) Údaj je označen jako nesprávný** — domněnka správnosti je suspendována (§ 4 odst. 5).
- **c) Oprávněná pochybnost** — orgán má důvod podezírat, že údaj neodpovídá skutečnosti.
- **d) Bezpečnostní řízení** — výjimka podle zákona č. 412/2005 Sb., o ochraně utajovaných informací.

V ostatních případech je požadavek na doložení **protizákonný** a osoba se může bránit cestou stížnosti, odvolání či žaloby.

> **Vazba na zákon č. 12/2020 Sb., o právu na digitální služby:** § 5 ZZR tvoří **technickou základnu** pro vymahatelné subjektivní právo občana na neopakované dokládání podle ZPDS. ZPDS toto právo deklaruje, ZZR jej technicky umožňuje.

#### Historické záznamy a aktuální stav (odst. 2 a 3)

Subtilní pravidlo: údaje **„ve tvaru předcházejícím současný stav"** (tj. historická verze údaje) se v ZR užívají **bez ověřování správnosti** (odst. 2 — protože jsou součástí archivovaného stavu). Ale **údaje vedené v AIS, které jsou současně referenčními údaji v ZR**, se užívají **jen v jejich historické verzi** (odst. 3) — aktuální stav je vázán výhradně na ZR.

Důvod: zabránit, aby aktuální údaj byl spravován ve dvou systémech současně s rizikem rozdílu. Aktuální verze referenčního údaje je **vždy v ZR**; AIS uchovává jen historické verze pro audit.

#### Notifikace editora (odst. 4) — povinnost součinnosti

Jakýkoli orgán veřejné moci, který při své činnosti zjistí, že údaj v ZR/AIS neodpovídá skutečnosti, **musí to neprodleně oznámit editorovi**. Toto pravidlo zavádí **horizontální solidaritu** ve veřejné správě — chyby zápisu se neopravují automaticky; každý orgán je strážcem správnosti.

V praxi se naplňuje funkcí „reklamace" v ISZR — orgán zadá podnět editorovi, který se vede jako služební úkon a editor je povinen v zákonné lhůtě zareagovat.

#### Architektonický princip — vše přes AIS a ISZR/ISSS (odst. 5)

Odst. 5 zakotvuje **architektonický zákaz přímého přístupu** k základním registrům:

1. **Orgán veřejné moci přistupuje k ZR vždy přes AIS** (nikdy přímo).
2. **AIS přistupuje k ZR vždy přes ISZR**.
3. **Mezi AIS, které nezapisují do ZR**, jde komunikace přes ISSS.

Toto vrstvené propojení zajišťuje **logování, kontrolu rolí, převod identifikátorů** (přes ORG) a **auditní stopu** každého přístupu. Bez této vrstvení by nebylo možné garantovat soulad s GDPR.

Výjimka z tohoto pravidla je v § 5b — přímý přístup pro účely národní bezpečnosti.

---

### § 5a — Využívání údajů soukromoprávním uživatelem

> **§ 5a**
>
> *(1) Soukromoprávní uživatel údajů, který je oprávněn využívat údaje vedené v základním registru nebo agendovém informačním systému právním předpisem, využívá tyto údaje k účelu stanovenému právním předpisem, v rozsahu potřebném k provedení úkonu soukromoprávního uživatele údajů a v rámci výčtu údajů zpřístupněných soukromoprávnímu uživateli údajů v rámci agendy.*
>
> *(2) Soukromoprávní uživatel údajů, který je oprávněn využívat údaje vedené v základním registru nebo agendovém informačním systému na základě souhlasu subjektu údajů, využívá tyto údaje k účelu stanovenému v souhlasu subjektu údajů, v rozsahu potřebném k provedení úkonu soukromoprávního uživatele údajů a v rámci výčtu údajů zpřístupněných soukromoprávnímu uživateli údajů souhlasem subjektu údajů.*
>
> *(3) Soukromoprávní uživatel údajů využívá údaje vedené v základním registru nebo agendovém informačním systému podle odstavců 1 a 2 prostřednictvím agendového informačního systému určeného ohlašovatelem agendy, a nebyl-li agendový informační systém ohlašovatelem agendy určen, prostřednictvím soukromoprávního systému pro využívání údajů. Ustanovení § 58 až 59 a ustanovení o oprávnění osoby poskytnout s využitím prostředku pro elektronickou identifikaci výpis ze zápisu vedeného v elektronické podobě v základním registru nebo potvrzení o tom, že určitý údaj v základním registru není veden, anebo údaje vedené o ní v základním registru podle zákona o informačních systémech veřejné správy nejsou větou první dotčeny. Soukromoprávní uživatel údajů zajistí, aby soukromoprávní systém pro využívání údajů umožnil využívání služeb informačního systému základních registrů a informačního systému sdílené služby.*
>
> *(4) Soukromoprávní uživatel údajů využívá referenční údaje vedené v základním registru, aniž by ověřoval jejich správnost.*
>
> *(5) Ustanovení § 5 odst. 3 a 4 se na soukromoprávního uživatele údajů použijí obdobně.*

**Výklad:**

§ 5a byl vložen zákonem č. 12/2020 Sb., o právu na digitální služby a komplexně upravuje **přístup soukromoprávních subjektů** k údajům v ZR/AIS.

#### Dva právní tituly přístupu

ZZR rozlišuje dva nezávislé tituly přístupu soukromoprávního uživatele:

1. **Zákonný titul** (odst. 1) — zvláštní zákon přiznává soukromoprávnímu uživateli právo přístupu. Typicky AML zákon, bankovní zákon, zákon o pojišťovnictví. Účel a rozsah jsou určeny **zákonem**.
2. **Souhlas subjektu údajů** (odst. 2) — fyzická osoba sama uděluje souhlas s přístupem soukromoprávního uživatele k jejím údajům. Účel a rozsah jsou určeny **souhlasem**.

Oba tituly podléhají testu nezbytnosti (rozsah potřebný k provedení úkonu) a vázanosti na agendu (registrovaný výčet údajů).

#### Technický kanál přístupu (odst. 3)

Soukromoprávní uživatel přistupuje k údajům buď přes:

1. **Agendový informační systém určený ohlašovatelem agendy** (typicky AIS provozovaný daným ústředním správním úřadem), nebo
2. **Vlastní soukromoprávní systém pro využívání údajů** (SPSVU) napojený na ISZR/ISSS.

SPSVU jsou typicky bankovní backend systémy napojené přes referenční rozhraní. Soukromoprávní uživatel je povinen zajistit, aby SPSVU technicky umožnil komunikaci s ISZR/ISSS.

#### Neověřování (odst. 4) — stejná ochrana jako pro OVM

Soukromoprávní uživatel **neověřuje správnost** referenčních údajů — stejné pravidlo jako pro OVM v § 5 odst. 2. Tím je soukromoprávní uživatel chráněn před povinností redundantního ověřování a požívá ochrany dobré víry podle § 4 odst. 6.

#### Subsidiární odkaz (odst. 5)

Pravidla § 5 odst. 3 (historická verze údajů z AIS) a § 5 odst. 4 (notifikace editora) se použijí **obdobně** — soukromoprávní uživatel má stejnou povinnost upozornit editora na zjištěnou nesprávnost.

---

### § 5b — Přímý přístup pro účely národní bezpečnosti

> **§ 5b**
>
> *(1) Orgán veřejné moci využívá údaje vedené v agendovém informačním systému přímým přístupem, a to i pokud jsou vyžadovány údaje o fyzické osobě, která není jednoznačně určena, je-li to potřebné pro plnění úkolu v jeho působnosti při zajišťování*
>
> *- a) bezpečnosti České republiky,*
>
> *- b) obrany České republiky,*
>
> *- c) veřejné bezpečnosti a účinné ochrany lidského života a zdraví,*
>
> *- d) předcházení, vyhledávání, odhalování trestné činnosti a stíhání trestných činů,*
>
> *- e) významného hospodářského nebo finančního zájmu České republiky nebo Evropské unie včetně takového zájmu v oblasti měnové, rozpočtové a daňové, nebo*
>
> *- f) ochrany práv osob v řízení před soudem.*
>
> *(2) Ustanovení tohoto zákona o realizaci vazeb prostřednictvím informačního systému základních registrů a informačního systému sdílené služby se při postupu podle odstavce 1 nepoužijí.*

**Výklad:**

§ 5b zakládá **výjimku z architektonického principu** § 5 odst. 5: pro účely národní bezpečnosti, vyšetřování trestné činnosti a obdobné kritické úkoly **se nepoužije** povinnost vést přístup přes ISZR/ISSS. Orgán smí přistupovat **přímo** do AIS.

Důvody jsou dvojí:

1. **Rychlost** — bezpečnostní zásah nesnese 30 sekund latence integrovaného přístupu.
2. **Utajení** — záznamy v ISZR/ISSS jsou auditovatelné a v běžném režimu poskytovatelné; v bezpečnostních věcech nelze takový auditní trail bezpodmínečně zachovat.

Výčet účelů v písm. a)–f) je **taxativní**: jiné účely neumožňují využití přímého přístupu. Současně lze přístup uplatnit i v případě, kdy **fyzická osoba není jednoznačně určena** — typicky při vyšetřování trestného činu, kdy podezřelý je popsán jen znaky.

Tato úprava je **silně sporná z hlediska ochrany osobních údajů**, protože omezuje auditní stopu. ZZR ji vyvažuje úpravou v § 60 (blokace zpřístupnění záznamů na žádost orgánu) a § 60a (přístup MV, PČR, zpravodajských služeb k záznamům i v rámci kontroly).

---

### § 7 — Správce ISZR a ISSS

> **§ 7**
>
> *(1) Správcem informačního systému základních registrů a informačního systému sdílené služby je Digitální a informační agentura (dále jen „Agentura“).*
>
> *(2) Agentura zajišťuje*
>
> *- a) provoz informačního systému základních registrů, informačního systému sdílené služby, registru obyvatel a registru práv a povinností a jejich bezpečnost,*
>
> *- b) realizaci vazeb mezi jednotlivými základními registry prostřednictvím služeb informačního systému základních registrů,*
>
> *- c) realizaci vazeb mezi základními registry a agendovými informačními systémy nebo soukromoprávními systémy pro využívání údajů prostřednictvím služeb informačního systému základních registrů,*
>
> *- d) realizaci vazeb mezi agendovými informačními systémy, jejichž prostřednictvím se zapisují údaje do základních registrů, a jinými agendovými informačními systémy nebo soukromoprávními systémy pro využívání údajů prostřednictvím služeb informačního systému základních registrů,*
>
> *- e) realizaci vazeb mezi agendovými informačními systémy, jejichž prostřednictvím se nezapisují údaje do základních registrů, navzájem nebo mezi agendovými informačními systémy, jejichž prostřednictvím se nezapisují údaje do základních registrů, a soukromoprávními systémy pro využívání údajů prostřednictvím služeb informačního systému sdílené služby,*
>
> *- f) zpřístupnění údajů vedených v základních registrech a údajů vedených v agendových informačních systémech, jejichž prostřednictvím se zapisují údaje do základních registrů, v rozsahu oprávnění vedených v registru práv a povinností prostřednictvím služeb informačního systému základních registrů,*
>
> *- g) zpřístupnění údajů vedených v agendových informačních systémech, jejichž prostřednictvím se nezapisují údaje do základních registrů, v rozsahu oprávnění vedených v registru práv a povinností prostřednictvím služeb informačního systému sdílené služby,*
>
> *- h) vedení záznamů o událostech souvisejících s provozováním informačního systému základních registrů a informačního systému sdílené služby,*
>
> *- i) propojení informačního systému základních registrů, informačního systému sdílené služby a dalších součástí referenčního rozhraní,*
>
> *- j) zveřejňování aktuálních údajů o provozních stavech základních registrů a provozně technických údajů z provozu základních registrů způsobem umožňujícím dálkový přístup,*
>
> *- k) poskytování centrální služby pro vyrozumívání o změnách údajů, které se vedou v informačním systému veřejné správy o subjektu údajů vedeném v registru obyvatel nebo o subjektu údajů vedeném v registru osob.*
>
> *(3) Agentura zajišťuje, aby údaje byly předávány prostřednictvím informačního systému základních registrů nebo informačního systému sdílené služby v nezměněné podobě.*
>
> *(4) Agentura vede pro účely správy informačního systému sdílené služby záznam o využívání údajů vedených v agendových informačních systémech, nejde-li o využívání údajů veřejně přístupných, a uchovává jej po dobu 2 let; záznam obsahuje*
>
> *- a) označení agendového informačního systému nebo soukromoprávního systému pro využívání údajů, jejichž prostřednictvím byly údaje využity, kód agendy, uživatelské jméno fyzické osoby, která je nositelem role, a označení subjektu, pro jehož účely se údaje využívají,*
>
> *- b) roli podle § 51 odst. 6 písm. c), ve které fyzická osoba údaje využila,*
>
> *- c) výčet údajů, které byly využity,*
>
> *- d) datum a čas využití údajů,*
>
> *- e) důvod a konkrétní účel využití údajů.*
>
> *(5) Agentura vydá na žádost osoby, o níž se vedou údaje v agendových informačních systémech, záznam o využívání těchto údajů. Záznam se vydává rovněž v podobě ověřeného výstupu z informačního systému veřejné správy.*
>
> *(6) Agentura není oprávněna k využívání údajů vedených v základních registrech nebo agendových informačních systémech s výjimkou využívání v rámci agendy, pro jejíž výkon byla zaregistrována.*
>
> *(7) Má-li Agentura důvodnou pochybnost, že orgán veřejné moci nebo soukromoprávní uživatel údajů neoprávněně využívá osobní údaje, informuje neprodleně Úřad pro ochranu osobních údajů (dále jen „Úřad“).*
>
> *(8) Náklady související s provozováním příslušného registru podle odstavce 2 písm. a) hradí jeho správce.*

**Výklad:**

§ 7 určuje **Digitální a informační agenturu (DIA)** jako správce páteřních systémů eGovernmentu — ISZR a ISSS, navíc i správce ROB a RPP. Tato koncentrace pravomocí je výsledkem novelizace zákonem č. 471/2022 Sb. s účinností od 1. dubna 2023. Předtím působila jako správce **Správa základních registrů (SZR)** podřízená Ministerstvu vnitra.

#### DIA — postavení v právním řádu

DIA je **ústřední správní úřad** zřízený zákonem č. 471/2022 Sb., o Digitální a informační agentuře. Působí v oblasti elektronické identifikace, digitální veřejné správy, informačních systémů veřejné správy a koordinace eGovernmentu. Je nástupcem **Správy základních registrů (SZR)**, která byla zrušena, a převzala též část kompetencí dříve vykonávaných Ministerstvem vnitra.

#### Jedenáct skupin činností Agentury (odst. 2)

Výčet v písm. a)–k) tvoří **kompletní funkční specifikaci** Agentury jako provozovatele referenčního rozhraní:

1. **Provoz a bezpečnost** (písm. a)) — fyzická a kybernetická bezpečnost ISZR, ISSS, ROB a RPP.
2. **Vazby mezi ZR navzájem** (písm. b)) — komunikace ROB ↔ ROS ↔ RUIAN ↔ RPP.
3. **Vazby ZR ↔ AIS / SPSVU** (písm. c)) — typický scénář: AIS úřadu se táže ROB na občanovy údaje.
4. **Vazby mezi AIS přes ISZR** (písm. d)) — pro AIS, které zapisují do ZR.
5. **Vazby mezi AIS přes ISSS** (písm. e)) — pro AIS, které nezapisují do ZR.
6. **Zpřístupnění údajů přes ISZR** (písm. f)) v rozsahu oprávnění z RPP.
7. **Zpřístupnění údajů přes ISSS** (písm. g)).
8. **Auditní záznamy** (písm. h)) — logování událostí.
9. **Propojení s dalšími prvky referenčního rozhraní** (písm. i)) — datové schránky, portál veřejné správy, eGON service bus.
10. **Veřejné informace o provozu** (písm. j)) — výpadky, dostupnost, statistiky.
11. **Notifikační služba** (písm. k)) — informuje občany o změnách jejich údajů v jiných ISVS (přidáno ZPDS).

#### Auditní zázname o využití AIS (odst. 4–5)

Agentura vede **záznamy o využívání údajů z AIS** (s výjimkou veřejně přístupných) a **uchovává je 2 roky**. Záznam obsahuje:

- označení AIS/SPSVU,
- kód agendy,
- uživatelské jméno (s ochranou neveřejnosti),
- subjekt, pro jehož účely byly údaje využity,
- roli, výčet využitých údajů,
- datum a čas,
- důvod a účel využití.

Na základě žádosti osoby vydá Agentura **záznam o využívání jejích údajů** (odst. 5) — jde o zakotvení **práva na transparenci přístupů** podle čl. 15 GDPR. Záznam se vydává i jako ověřený výstup z ISVS.

#### Omezení vlastních přístupů Agentury (odst. 6–7)

Agentura **sama** není oprávněna využívat údaje vedené v ZR/AIS — jen v rámci své vlastní registrované agendy (typicky agenda provozování ISZR). Tím je vyloučeno, aby provozovatel infrastruktury byl současně masivním uživatelem dat.

Má-li Agentura **pochybnost o neoprávněném využívání**, informuje neprodleně **ÚOOÚ** (odst. 7). Tato povinnost představuje **horizontální spolupráci dohledových orgánů** — DIA jako provozovatel, ÚOOÚ jako dohledový orgán nad osobními údaji.

---

### § 8 — Správce agendového informačního systému

> **§ 8**
>
> *(1) Správce4) agendového informačního systému zajišťuje realizaci vazby mezi agendovým informačním systémem a informačním systémem základních registrů za účelem zapisování a využívání údajů.*
>
> *(2) Správce agendového informačního systému zajišťuje realizaci vazeb mezi agendovým informačním systémem a jinými agendovými informačními systémy prostřednictvím informačního systému základních registrů nebo informačního systému sdílené služby za účelem využívání údajů.*
>
> *(3) Správce agendového informačního systému umožní využívání údajů vedených v agendovém informačním systému orgánu veřejné moci v rozsahu, v jakém jsou orgánu veřejné moci tyto údaje zpřístupněny pro výkon agendy, a soukromoprávnímu uživateli údajů v rozsahu, v jakém je oprávněn tyto údaje využívat podle tohoto zákona nebo podle jiného právního předpisu.*
>
> *(4) Správce agendového informačního systému zajistí používání kódu agendy přiděleného správcem registru práv a povinností při komunikaci agendového informačního systému s informačním systémem základních registrů nebo informačním systémem sdílené služby.*
>
> *(5) Správce agendového informačního systému používá vlastní identifikátory fyzických osob a právnických osob a za účelem komunikace s informačním systémem základních registrů nebo informačním systémem sdílené služby používá agendové identifikátory fyzických osob a identifikátory právnických osob vedené v registru osob.*
>
> *(6) Správce agendového informačního systému zavede mechanismus opravy nesprávného údaje vedeného v agendovém informačním systému.*
>
> *(7) Správce agendového informačního systému zajistí vyrozumění o změně údaje, který se vede v agendovém informačním systému o subjektu údajů vedeném v registru obyvatel nebo o subjektu údajů vedeném v registru osob, s využitím služby podle § 7 odst. 2 písm. k). Správce agendového informačního systému zajistí vyrozumění o změně údaje, který se vede v agendovém informačním systému o jiném subjektu údajů, s využitím vlastní služby pro vyrozumívání o změnách údajů vedených v agendovém informačním systému.*

**Výklad:**

§ 8 vymezuje **povinnosti správce AIS**. Správce AIS je orgán veřejné moci, který provozuje konkrétní AIS — např. Ministerstvo vnitra je správcem AIS evidence obyvatel, Ministerstvo financí AIS daňové správy.

#### Sedm povinností správce AIS

1. **Vazba na ISZR** (odst. 1) — technicky napojit AIS na ISZR pro zápis i čtení do ZR.
2. **Vazba na jiné AIS** (odst. 2) — zajistit propustnost přes ISZR/ISSS.
3. **Zpřístupnění údajů** (odst. 3) — umožnit přístup OVM a soukromoprávním uživatelům v rozsahu oprávnění.
4. **Používání kódu agendy** (odst. 4) — každá komunikace musí být označena kódem agendy z RPP. Bez toho ISZR/ISSS žádost odmítne.
5. **Dvojí identifikátory** (odst. 5) — uvnitř AIS používá vlastní identifikátory, navenek (přes ISZR/ISSS) **AIFO** a IČO.
6. **Mechanismus opravy** (odst. 6) — povinnost zavést proces reklamace nesprávných údajů.
7. **Notifikace o změnách** (odst. 7) — využití centrální notifikační služby Agentury.

#### Architektonický význam (odst. 5) — dvojí identifikátor

Pravidlo „**vlastní identifikátory uvnitř, agendové identifikátory navenek**" je technickým ztělesněním principu ORG. AIS si může vést své interní ID osoby (pořadové číslo v evidenci), ale **mimo svůj okruh musí používat AIFO** přidělené pro jeho konkrétní agendu. Tím nelze fragmenty osobních údajů z různých AIS propojit jednoduchou agregací — vyžaduje to požadavek na ORG.

#### Notifikace občanovi (odst. 7) — právo na transparenci

Správce AIS zajistí, aby občan (vedený v ROB) nebo subjekt v RPO byl vyrozuměn o **každé změně svých údajů** v daném AIS. Tato služba je centrálně provozována Agenturou (§ 7 odst. 2 písm. k)) a slouží jako realizace **práva na transparentní zpracování** podle čl. 13 a 14 GDPR.

---

### § 8a — Soukromoprávní uživatel údajů — povinnosti

> **§ 8a**
>
> *(1) Soukromoprávní uživatel údajů zajišťuje realizaci vazby mezi soukromoprávním systémem pro využívání údajů a informačním systémem základních registrů za účelem využívání údajů.*
>
> *(2) Soukromoprávní uživatel údajů zajišťuje realizaci vazeb mezi soukromoprávním systémem pro využívání údajů a agendovými informačními systémy prostřednictvím informačního systému základních registrů nebo informačního systému sdílené služby za účelem využívání údajů.*
>
> *(3) Soukromoprávní uživatel údajů zajistí používání kódu agendy při komunikaci soukromoprávního systému pro využívání údajů s informačním systémem základních registrů nebo informačním systémem sdílené služby.*
>
> *(4) Soukromoprávní uživatel údajů používá vlastní identifikátory fyzických osob a právnických osob a za účelem komunikace s informačním systémem základních registrů nebo informačním systémem sdílené služby používá agendové identifikátory fyzických osob a identifikátory právnických osob vedené v registru osob.*

**Výklad:**

§ 8a paralelně k § 8 upravuje **povinnosti soukromoprávního uživatele údajů**. Konstrukce je obdobná, jen místo „AIS" se mluví o „**soukromoprávním systému pro využívání údajů (SPSVU)**":

1. Vazba na ISZR (odst. 1).
2. Vazby na AIS přes ISZR/ISSS (odst. 2).
3. Používání kódu agendy (odst. 3) — i soukromoprávní uživatel musí jednat v rámci registrované agendy.
4. Dvojí identifikátor — vlastní uvnitř, AIFO/IČO navenek (odst. 4).

Soukromoprávní uživatelé tak nejsou „výjimkou" z architektury — jsou plnohodnotnými, byť omezenými, účastníky referenčního rozhraní. Banka, která využívá ROB pro AML kontrolu, musí mít SPSVU napojený přes ISZR a každý dotaz označit kódem agendy AML.

---

### § 9 — Identifikátory fyzických osob

> **§ 9**
>
> *(1) Agendový identifikátor fyzické osoby je neveřejným identifikátorem, který je jednoznačně přiřazen záznamu o fyzické osobě v agendovém informačním systému, základním registru nebo soukromoprávním systému pro využívání údajů v rámci příslušné agendy, je odvozen ze zdrojového identifikátoru fyzické osoby, kódu agendy a v případě soukromoprávního systému pro využívání údajů rovněž z identifikátoru soukromoprávního uživatele údajů a je užíván výlučně k jednoznačnému určení fyzické osoby pro účely výkonu agendy, pro kterou byl přidělen. Z agendového identifikátoru fyzické osoby nelze odvodit zdrojový identifikátor fyzické osoby a nelze z něj ani dovodit osobní nebo jiné údaje o fyzické osobě, jíž byl přiřazen.*
>
> *(2) Zdrojový identifikátor fyzické osoby je neveřejným identifikátorem. Ze zdrojového identifikátoru fyzické osoby nelze dovodit osobní ani jiné údaje o fyzické osobě, jíž byl přiřazen.*
>
> *(3) Za účelem zabránění neoprávněnému využívání údajů vedených v základních registrech nebo agendových informačních systémech orgán veřejné moci nebo soukromoprávní uživatel údajů při komunikaci základních registrů navzájem, základních registrů s agendovými informačními systémy nebo soukromoprávními systémy pro využívání údajů, agendových informačních systémů navzájem a agendových informačních systémů se soukromoprávními systémy pro využívání údajů používá identifikátory, kterými jsou*
>
> *- a) kód agendy,*
>
> *- b) agendový identifikátor fyzické osoby.*

**Výklad:**

§ 9 zakotvuje **dva typy identifikátorů fyzických osob** a jejich kryptografický vztah. Tento institut je **bezpečnostním srdcem celého systému** a představuje nejvýznamnější rozdíl mezi koncepcí ZZR a starým modelem rodného čísla.

#### Tři vrstvy identifikátorů

| Identifikátor | Zkratka | Pole užití | Veřejnost |
|---|---|---|---|
| **Zdrojový identifikátor fyzické osoby** | **ZIFO** | Pouze ÚOOÚ — pro vytváření AIFO a převod mezi nimi (§ 11) | Neveřejný |
| **Agendový identifikátor fyzické osoby** | **AIFO** | V rámci jedné agendy — komunikace AIS, ZR, SPSVU | Neveřejný |
| (Klasické identifikátory) | jméno + datum narození + adresa | V identifikačních dokladech | Veřejné v omezeném rozsahu |

#### Kryptografický vztah ZIFO ↔ AIFO

AIFO je **odvozen** ze ZIFO + kód agendy (+ v případě SPSVU + identifikátor soukromoprávního uživatele) jednosměrnou funkcí. Klíčové vlastnosti:

1. **Z AIFO nelze odvodit ZIFO** — jednosměrnost zaručuje, že ani úplné vyzrazení AIFO neohrozí jiné agendy.
2. **Z AIFO nelze odvodit osobní údaje** — AIFO je „čistý" identifikátor bez sémantického obsahu (na rozdíl od rodného čísla, z něhož lze odvodit datum narození a pohlaví).
3. **AIFO je vázané na agendu** — ten samý člověk má v agendě evidence obyvatel AIFO_A, v agendě daňové AIFO_B, v agendě zdravotního pojištění AIFO_C. Tyto identifikátory nejsou navzájem převoditelné nikým jiným než ÚOOÚ.

#### Architektonický význam — proti profilování

Agendové identifikátory **technicky znemožňují masové propojování osobních údajů napříč agendami**. Pokud by IT firma získala dump dat ze tří různých AIS, nemohla by data jednoho člověka napříč propojit — AIFO jsou v každé agendě jiné.

Pro **legitimní propojení** (typicky při výkonu agendy, kde je třeba propojit údaje z více ZR/AIS) slouží **služba převodu identifikátorů** podle § 11 — výhradně přes ÚOOÚ, na zákonný požadavek a s auditní stopou.

Tato architektura je **přímou reakcí na ústavní problematiku jednotného identifikátoru** (rodného čísla), kterou kritizoval Ústavní soud i Veřejný ochránce práv jako neslučitelnou s ochranou soukromí.

#### Pravidlo komunikace (odst. 3)

Komunikace mezi ZR, AIS a SPSVU se vede **výhradně přes kombinaci kódu agendy + AIFO** — žádné jiné identifikátory (rodné číslo, jméno) nesmí být v této komunikaci primární. Tím je zajištěno, že:

- žádost je přiřaditelná konkrétní agendě;
- osoba je identifikována jen pro účel této agendy;
- napojené systémy nemohou agregovat údaje napříč.

---

### § 10 — Pravidla užívání AIFO

> **§ 10**
>
> *(1) Fyzická osoba může být identifikována v jednotlivé agendě pouze jedním agendovým identifikátorem fyzické osoby. V případě agendy vykonávané soukromoprávním uživatelem údajů může být fyzická osoba identifikována agendovými identifikátory fyzické osoby jednoznačně přiřazenými záznamu o fyzické osobě v jednotlivých soukromoprávních systémech pro využívání údajů.*
>
> *(2) Agendový identifikátor fyzické osoby v jednotlivé agendě odvozený z jednoho zdrojového identifikátoru fyzické osoby nesmí být přidělen více fyzickým osobám.*
>
> *(3) Agendový identifikátor fyzické osoby nelze po přidělení měnit, pokud tento zákon nestanoví jinak.*
>
> *(4) Pokud dojde k přidělení stejného agendového identifikátoru fyzické osoby v dané agendě záznamům o dvou nebo více fyzických osobách, je těmto záznamům přidělen nový agendový identifikátor fyzické osoby.*
>
> *(5) Pokud dojde k přidělení dvou nebo více agendových identifikátorů fyzických osob záznamu o jedné fyzické osobě v dané agendě, postupuje se obdobně podle odstavce 4.*
>
> *(6) Zjistí-li orgán veřejné moci nebo soukromoprávní uživatel údajů nedostatky v přidělení agendového identifikátoru fyzické osoby, oznámí tuto skutečnost bez zbytečného odkladu správci agendového informačního systému nebo soukromoprávního systému pro využívání údajů, v nichž byl nedostatek zjištěn. Příslušný správce agendového informačního systému nebo soukromoprávního systému pro využívání údajů prošetří, zda lze zjištěné nedostatky odstranit v agendovém informačním systému nebo soukromoprávním systému pro využívání údajů, a pokud je to možné, nedostatky odstraní.*
>
> *(7) Zjistí-li správce agendového informačního systému nebo soukromoprávního systému pro využívání údajů nedostatky v přidělení agendového identifikátoru fyzické osoby, které nelze odstranit podle odstavce 6, oznámí tuto skutečnost bez zbytečného odkladu správci registru obyvatel. Správce registru obyvatel ve spolupráci se správcem agendového informačního systému nebo soukromoprávního systému pro využívání údajů prošetří, zda lze zjištěné nedostatky odstranit, a pokud je to možné, nedostatky odstraní; obdobně se postupuje v případě, kdy nedostatky v přidělení agendového identifikátoru fyzické osoby zjistí správce registru obyvatel. Nelze-li nedostatky odstranit postupem podle věty druhé, postupuje se podle odstavců 4 a 5.*

**Výklad:**

§ 10 zakotvuje **integritní pravidla** přidělování AIFO. Princip: **jeden člověk — jedna agenda — jeden AIFO**.

#### Dvě integritní pravidla (odst. 1, 2)

1. **V agendě má fyzická osoba jeden AIFO** (odst. 1). Pro soukromoprávní agendu — jeden AIFO na osobu **na jeden SPSVU** (různé SPSVU pro tutéž soukromoprávní agendu mohou mít své AIFO).
2. **Jeden AIFO odvozený z jednoho ZIFO nesmí být přidělen více osobám** (odst. 2). Vylučuje záměnu identit.

#### Neměnnost (odst. 3) a opravné mechanismy (odst. 4–5)

AIFO je **trvalý** identifikátor — po přidělení se nemění. Toto pravidlo je pojistkou proti administrativní svévoli a zaručuje stabilitu identifikace v čase.

Výjimky (§ 23 — nové pořízení AIFO na žádost subjektu údajů; § 10 odst. 4 a 5 — kolizní situace):

- **Kolize identifikátorů** — stejný AIFO přiřazen dvěma osobám → oba dostanou nový AIFO.
- **Multiplicita** — jedna osoba má v jedné agendě dva AIFO → konsolidace na jeden.

#### Mechanismus opravy chyb (odst. 6, 7)

Postupná eskalace:

1. **Zjistitel chyby** (OVM nebo soukromoprávní uživatel) → oznámí správci AIS/SPSVU.
2. **Správce AIS/SPSVU** se pokusí opravit ve svém systému; pokud nelze → oznámí správci ROB.
3. **Správce ROB (DIA)** ve spolupráci s správcem AIS/SPSVU řeší chybu; nelze-li → postupuje se podle odst. 4–5 (přidělení nového AIFO).

Tento mechanismus zajišťuje, že **integritní problémy se řeší centrálně přes ROB**, který je „autoritou pravdy" pro identitu fyzických osob.

---

### § 11 — Působnost Úřadu pro ochranu osobních údajů

> **§ 11**
>
> *(1) Úřad*
>
> *- a) vytváří zdrojové identifikátory fyzických osob a agendové identifikátory fyzických osob a vede jejich seznamy,*
>
> *- b) zajišťuje převod agendového identifikátoru fyzické osoby v agendě na agendový identifikátor této fyzické osoby v jiné agendě a převod mezi agendovými identifikátory fyzické osoby v rámci agendy vykonávané soukromoprávním uživatelem údajů, a to na základě zákonného požadavku.*
>
> *(2) Zdrojový identifikátor fyzické osoby používá výhradně Úřad pro vytváření agendových identifikátorů fyzických osob podle odstavce 1 písm. a) a jejich převod podle odstavce 1 písm. b).*

**Výklad:**

§ 11 svěřuje **Úřadu pro ochranu osobních údajů** klíčovou roli — provozuje **ORG (Převodník identifikátorů)** a je jediným orgánem, který může převést AIFO z jedné agendy na AIFO v jiné agendě.

#### ORG — institucionální brzda profilování

Architektonická volba ZZR pověřit **ÚOOÚ** (nikoli MV či DIA) provozováním ORG má hluboký systémový význam:

1. **Konflikt zájmů** — kdyby ORG provozoval orgán s obecnou působností v eGovernmentu (MV, DIA), hrozilo by, že jako provozovatel a zároveň „spotřebitel" by mohl konvertovat AIFO podle svých potřeb. ÚOOÚ jako dohledový orgán nemá vlastní agendový zájem.
2. **Politická nezávislost** — ÚOOÚ má ústavně zakotvenou nezávislost; jeho předseda je jmenován prezidentem na návrh Senátu.
3. **Symbolický význam** — provozováním ORG ÚOOÚ technicky kontroluje, kdo a kdy propojuje osobní údaje napříč agendami. Tím se z formálního dohledového orgánu stává **operační strážce** ochrany dat.

#### „Zákonný požadavek" jako podmínka převodu (odst. 1 písm. b))

ÚOOÚ převede AIFO **jen na základě zákonného požadavku**. Zákonným požadavkem je obvykle:

- agendová potřeba podle registrace agendy v RPP (např. orgán potřebuje propojit údaje z ROB s údaji ze zdravotního AIS);
- soudní nebo policejní požadavek v rámci trestního řízení;
- kontrolní úkon ÚOOÚ samotného.

Každý převod je logován a tvoří **auditní stopu**, kterou lze v případě sporu nebo kontroly rekonstruovat.

#### Výlučnost užívání ZIFO (odst. 2)

ZIFO je **„state secret" celého systému** — používá jej výhradně ÚOOÚ a pouze ke dvěma účelům: vytváření AIFO a jejich převod. Nikdo jiný k ZIFO přístup nemá; ZIFO neopouští servery ÚOOÚ.

Tato izolace ZIFO je technickou garancí toho, že ani útok na ÚOOÚ nevede k masovému kompromitování všech agend — útočník by získal jen ZIFO, z nichž stále nemůže odvodit osobní údaje (§ 9 odst. 2 — neodvoditelnost údajů ze ZIFO).

---

### § 12 — Identifikátor subjektů vedených v registru osob

> **§ 12**
>
> *Identifikátorem subjektu vedeného v registru osob je identifikační číslo osoby.*

**Výklad:**

§ 12 stanoví, že identifikátorem subjektu v ROS je **identifikační číslo osoby (IČO)** — osmimístné číslo, které se přiděluje právnickým osobám, OSVČ, organizačním složkám státu, OVM a dalším subjektům podle § 25.

#### IČO — kontrast s AIFO

Zásadní rozdíl proti identifikátorům fyzických osob:

| | Fyzické osoby | Právnické osoby a OSVČ |
|---|---|---|
| Identifikátor | AIFO (různý v každé agendě) | IČO (jediné, sdílené napříč agendami) |
| Veřejnost | Neveřejný | Veřejné |
| Ochrana profilování | Ano (přes ORG) | Žádná |

Proč rozdíl? Právnické osoby a podnikatelé **nemají ústavní právo na soukromí** v takovém rozsahu jako fyzické osoby. Naopak veřejnost obchodního styku vyžaduje **jednoznačnou a veřejnou identifikaci** podnikatelských subjektů. IČO proto plní opačnou funkci — má usnadnit propojování údajů o subjektu napříč evidencemi.

OSVČ jsou v této struktuře zvláštním případem — jako fyzické osoby mají AIFO (pro osobní záležitosti), jako podnikatelé mají IČO (pro podnikatelské záležitosti). Tato dvojakost je zachycena v § 26 odst. 2 písm. b) — pro OSVČ se vede odkaz na ROB i IČO v ROS.

---

### § 13 — Kód agendy

> **§ 13**
>
> *Kód agendy je veřejným identifikátorem, který je jednoznačně přiřazen záznamu o agendě v číselníku agend v registru práv a povinností.*

**Výklad:**

**Kód agendy** je veřejný identifikátor agendy v RPP. Číselník agend vede Agentura (DIA) a je veřejně přístupný — každý si může ověřit, jaké agendy jsou v ČR registrovány a kdo je vykonává.

Kód agendy je **klíčovým prvkem každé komunikace v referenčním rozhraní** (§ 9 odst. 3 písm. a)) — bez něj je požadavek na údaje z ZR nepřípustný.

> **Praktický význam:** Kód agendy umožňuje detailní auditní trail. Když DIA loguje přístup k ROB, vždy je u záznamu uveden kód agendy. Lze tak zpětně rekonstruovat, kdo k údaji přistoupil a v jaké agendě.

---

### § 14 — Vydávání ověřených výstupů, záznamů a výpisů ze základních registrů

> **§ 14**
>
> *(1) Ze základního registru se vydávají ověřené výstupy z informačního systému veřejné správy1). K ověřenému výstupu z informačního systému veřejné správy, který je vydán z registru obyvatel a který obsahuje údaj o adrese místa pobytu, kontaktní místo veřejné správy na žádost přiloží vícejazyčný standardní formulář vyhotovený podle přímo použitelného předpisu Evropské unie55).*
>
> *(2) Ze základního registru se poskytují záznamy o využívání údajů vedených v základním registru za podmínek stanovených tímto zákonem.*
>
> *(3) Není-li zákonem stanoveno jinak, správce základního registru poskytne záznam o využívání údajů vedených v základním registru pouze osobě, o které jsou tyto údaje vedeny.*
>
> *(4) Správce příslušného základního registru umožní osobě uvedené v odstavci 3 obstarat si bezplatně záznam o využívání údajů vedených v základním registru způsobem stanoveným zákonem o informačních systémech veřejné správy pro obstarání si výstupu z informačního systému veřejné správy s využitím prostředku pro elektronickou identifikaci. Správce příslušného základního registru zašle do datové schránky osoby uvedené v odstavci 3 na žádost této osoby bezplatně záznam o využívání údajů vedených v základním registru. Záznam se vydává rovněž v podobě ověřeného výstupu z informačního systému veřejné správy.*
>
> *(5) Dojde-li ke změně údaje vedeného v základním registru, s výjimkou provozního nebo autentizačního údaje, zašle bez zbytečného odkladu správce základního registru osobě uvedené v odstavci 3, které se tato změna týká, má-li zřízenu a zpřístupněnu datovou schránku, bezplatně výpis údajů, s výjimkou provozních a autentizačních údajů, z příslušného základního registru do datové schránky.*
>
> *(6) Zjistí-li osoba uvedená v odstavci 3 nesoulad údajů, které jsou o ní vedeny, s výjimkou provozních nebo autentizačních údajů, se skutečným stavem, může bezplatně požádat o změnu údajů editora příslušného údaje, a to i prostřednictvím kontaktního místa veřejné správy6). Kontaktní místo veřejné správy předá žádost editorovi příslušného údaje. Editor postupuje podle § 4 odst. 3.*

**Výklad:**

§ 14 zakotvuje **práva osoby vůči svým údajům v ZR** — práva na výpis, transparentnost, notifikaci a reklamaci. Toto ustanovení je spolu s § 58 nejvýznamnějším projevem **subjektivních práv občana** v ZZR.

#### Ověřené výstupy z ISVS (odst. 1) — CzechPOINT

Z každého základního registru se vydávají **ověřené výstupy z ISVS** (čerpáno přes kontaktní místa veřejné správy — CzechPOINT, datové schránky, portál veřejné správy). Výstupy mají charakter veřejných listin podle ZISVS a slouží jako důkaz ve správním řízení i v civilním styku.

Při ověřeném výstupu z ROB s adresou se **na žádost přiloží vícejazyčný standardní formulář** podle nařízení EU 2016/1191 — usnadňuje použití výpisu v zahraničí (zejména pro občany EU).

#### Záznamy o využití (odst. 2–3) — právo na transparenci

Záznamy o tom, **kdo přistupoval k údajům subjektu**, jsou poskytovány:

1. Standardně **jen subjektu samotnému** (odst. 3) — garantuje právo na informaci o zpracování (čl. 15 GDPR).
2. Jiným osobám jen na základě **zvláštního zákona** (typicky orgánům činným v trestním řízení).

#### Bezplatné získání záznamu (odst. 4) — vícekanálovost

Subjekt si může záznam obstarat:

1. **S využitím prostředku pro elektronickou identifikaci** (NIA, eObčanka) — typicky přes portál.gov.cz nebo Identitu občana.
2. **V podobě ověřeného výstupu** — typicky přes CzechPOINT.

Vše je **bezplatné** — tato bezplatnost je důsledným provedením GDPR (čl. 12 odst. 5 — bezplatnost prvního přístupu).

#### Notifikace při změně údaje (odst. 5) — proaktivní informování

Dojde-li ke **změně referenčního údaje**, správce ZR **automaticky zasílá výpis** do datové schránky subjektu — pokud ji má zřízenu. Toto pravidlo zavádí **proaktivní informování**, nikoli jen reaktivní (na žádost). Občan je informován o každém zápisu do svých údajů a může jej okamžitě reklamovat.

Provozní a autentizační údaje jsou z notifikace vyloučeny — jejich změna je technického charakteru a oznamování by zbytečně zahlcovalo datové schránky.

#### Reklamace (odst. 6) — právo na opravu

Zjistí-li subjekt **nesoulad svých údajů se skutečností**, může **bezplatně** požádat o opravu:

- přímo u editora příslušného údaje;
- nebo přes **kontaktní místo veřejné správy** (CzechPOINT), které žádost předá editorovi.

Editor pak postupuje podle § 4 odst. 3 — lhůta 3 pracovních dnů na zápis opravy.

> **Vztah k čl. 16 GDPR (právo na opravu):** § 14 odst. 6 ZZR je konkrétním provedením práva na opravu v prostředí veřejné správy. Lhůta 3 pracovních dnů je výrazně kratší než obecná lhůta podle GDPR (jeden měsíc) — odraz mimořádného významu referenčních údajů.

---

### § 15 — Vlastnictví registrů a IS

> **§ 15**
>
> *Základní registry, informační systém základních registrů a informační systém sdílené služby jsou majetkem státu. Zvláštní právo pořizovatele databáze, kterou je tvořen příslušný základní registr, vykonává správce příslušného základního registru.*

**Výklad:**

§ 15 řeší **vlastnické postavení** základních registrů a jejich infrastruktury:

1. **Vlastníkem je stát** (Česká republika) — nikoli konkrétní orgán. Tím se vylučují spory o vlastnictví při reorganizaci státní správy.
2. **Zvláštní právo pořizovatele databáze** podle § 88 a násl. autorského zákona vykonává **správce ZR** — tedy DIA (pro ROB a RPP), ČÚZK (pro RUIAN), Agentura (pro ROS). Toto právo umožňuje správci kontrolovat užívání databáze třetími stranami nad rámec ZZR.

Toto ustanovení má praktický význam zejména pro otázky:

- ochrany před neoprávněným kopírováním databáze;
- poskytování dat soukromé sféře (cenové podmínky);
- definice „podstatné části" databáze pro účely autorskoprávní ochrany.

---

## HLAVA II — Registr obyvatel

### § 16 — Předmět ROB

> **§ 16**
>
> *V registru obyvatel jsou o fyzických osobách uvedených v § 17 vedeny referenční údaje a další údaje, o nichž tak stanoví tento zákon.*

**Výklad:**

§ 16 stanoví **funkci ROB** — vést referenční a další údaje o fyzických osobách v zákonem vymezeném okruhu (§ 17). ROB tedy **není evidencí všech lidí žijících v ČR**, nýbrž jen těch, kteří splňují podmínky § 17 (občané ČR, cizinci s pobytem, azylanti a další zákonem stanovené osoby).

ROB tvoří **referenční datovou základnu** pro identifikaci fyzických osob ve veřejné správě. Všechny ostatní AIS, které potřebují identifikovat osobu, vedou referenční vazby do ROB a samy údaje neuchovávají duplicitně.

---

### § 17 — Subjekty údajů v ROB

> **§ 17**
>
> *Subjekty údajů vedených v registru obyvatel jsou*
>
> *- a) státní občané České republiky,*
>
> *- b) cizinci, kteří pobývají na území České republiky v rámci trvalého pobytu anebo na základě dlouhodobého víza nebo povolení k dlouhodobému pobytu,*
>
> *- c) občané jiných členských států Evropské unie, občané států, které jsou vázány mezinárodní smlouvou sjednanou s Evropským společenstvím, a občané států, které jsou vázány smlouvou o Evropském hospodářském prostoru, a jejich rodinní příslušníci, kteří pobývají na území České republiky v rámci trvalého pobytu nebo kterým byl vydán doklad o přechodném pobytu na území České republiky delším než 3 měsíce,*
>
> *- d) cizinci, kterým byla na území České republiky udělena mezinárodní ochrana formou azylu nebo doplňkové ochrany,*
>
> *- e) jiné fyzické osoby, u nichž to vyžaduje jiný právní předpis.*

**Výklad:**

§ 17 taxativně vymezuje **subjekty údajů v ROB**. Výčet je strukturován podle pobytového statutu a státního občanství:

1. **Občané ČR** (písm. a)) — vždy, bez ohledu na to, kde žijí. ROB obsahuje i občany žijící trvale v zahraničí (typicky pro výkon volebního práva).
2. **Cizinci s pobytem nad 90 dnů z třetích zemí** (písm. b)) — trvalý pobyt, dlouhodobé vízum, povolení k dlouhodobému pobytu podle zákona o pobytu cizinců.
3. **Občané EU/EHP** a jejich rodinní příslušníci (písm. c)) — pokud mají trvalý pobyt nebo přechodný pobyt nad 3 měsíce.
4. **Azylanti** (písm. d)) — osoby s azylem nebo doplňkovou ochranou podle zákona č. 325/1999 Sb., o azylu.
5. **Jiné osoby podle zvláštního zákona** (písm. e)) — otevřená klauzule pro jiné zákonem stanovené případy.

#### Kdo v ROB **není**

- **Krátkodobí turisté** (do 90 dnů) — nemají v ČR pobyt.
- **Cizinci na krátkodobé vízum** — nejsou v ROB.
- **Žadatelé o azyl** (před vydáním rozhodnutí) — pouze v AIS cizinců, nikoli v ROB.

Tyto osoby jsou nicméně evidovány v **agendových informačních systémech** (typicky AIS cizinců) — jen nejsou referenčním údajem v ROB.

#### Vazba na občanství a státní příslušnost

Pojem „**státní občan České republiky**" (písm. a)) odpovídá zákonu č. 186/2013 Sb., o státním občanství ČR. Vícenásobné občanství neovlivňuje zápis v ROB — osoba se vede podle skutečnosti, že je občanem ČR, bez ohledu na další občanství. Údaj o vícenásobném občanství se ovšem v ROB vede (§ 18 odst. 1 písm. g)).

---

### § 18 — Údaje vedené v ROB

> **§ 18**
>
> *(1) V registru obyvatel se vedou*
>
> *- a) příjmení, rodné příjmení,*
>
> *- b) jméno, popřípadě jména,*
>
> *- c) pohlaví,*
>
> *- d) adresa místa pobytu12), případně též adresa, na kterou mají být doručovány písemnosti podle jiného právního předpisu52); uvedené adresy jsou vedeny ve formě referenční vazby (kódu adresního místa) na referenční údaj o adrese v registru územní identifikace; v případě adresy, na kterou mají být doručovány písemnosti podle jiného právního předpisu52), se vede i údaj o identifikaci poštovní přihrádky, dodávací schránky nebo poštovním směrovacím číslu místa pobytu anebo adresa, která je mimo území České republiky a které nebyl přidělen kód adresního místa v registru územní identifikace; v případě adresy místa pobytu12) je tento údaj označen jako adresa úřadu, pokud je stejným způsobem označen v informačním systému evidence obyvatel nebo informačním systému cizinců,*
>
> *- e) datum, místo a okres narození, u subjektu údajů, který se narodil v cizině, datum, místo a stát, kde se narodil; údaj o místě a okrese narození na území České republiky se vede ve formě referenční vazby (kódu územního prvku) na referenční údaj v registru územní identifikace,*
>
> *- f) datum, místo a okres úmrtí, jde-li o úmrtí subjektu údajů mimo území České republiky, vede se datum úmrtí, místo a stát, na jehož území k úmrtí došlo; je-li vydáno rozhodnutí soudu o prohlášení za mrtvého, vede se den, který je v rozhodnutí uveden jako den smrti, popřípadě jako den, který nepřežil, a datum nabytí právní moci tohoto rozhodnutí; údaj o místě a okrese úmrtí na území České republiky se vede ve formě referenční vazby (kódu územního prvku) na referenční údaj v registru územní identifikace,*
>
> *- g) státní občanství, popřípadě více státních občanství,*
>
> *- h) omezení svéprávnosti,*
>
> *- i) rodinný stav nebo registrované partnerství,*
>
> *- j) čísla a druhy identifikačních dokladů a datum skončení jejich platnosti,*
>
> *- k) typ datové schránky a identifikátor datové schránky14), je-li tato datová schránka zpřístupněna,*
>
> *- l) telefonní číslo pro veřejnou mobilní telefonní síť nebo adresa elektronické pošty pro zasílání zvoleného okruhu informací,*
>
> *- m) sériové číslo, vydavatel a platnost kvalifikovaného certifikátu pro elektronický podpis,*
>
> *- n) data potřebná pro elektronickou identifikaci a autentizaci, včetně případného požadavku na doplnění fyzického prokázání totožnosti autentizací s využitím těchto dat, jde-li o subjekt údajů uvedený v § 17 písm. a),*
>
> *- o) datum a čas zablokování a odblokování dat potřebných pro elektronickou identifikaci a autentizaci, jde-li o subjekt údajů uvedený v § 17 písm. a).*
>
> *(2) Údaje uvedené v odstavci 1 písm. a) až k) jsou referenčními údaji.*
>
> *(3) Referenční údaj o čísle identifikačního dokladu slouží k elektronické identifikaci jeho držitele při komunikaci s informačními systémy veřejné správy. Data potřebná pro elektronickou identifikaci a autentizaci jsou pro účely registru obyvatel autentizačním údajem, který se vede v jednosměrně šifrované podobě, která neumožňuje přístup k jeho hodnotě, a který je neveřejný.*
>
> *(4) Identifikátorem fyzické osoby podle § 9 je agendový identifikátor fyzické osoby pro agendu registru obyvatel.*
>
> *(5) V registru obyvatel se dále vedou provozní údaje*
>
> *- a) záznam o využívání údajů vedených v registru obyvatel pro potřeby agendových informačních systémů nebo soukromoprávních systémů pro využívání údajů,*
>
> *- b) záznam o poskytnutí údajů subjektu údajů nebo jiné osobě podle § 58a, který obsahuje datum a čas poskytnutí, identifikátor souhlasu subjektu údajů s poskytnutím údajů jiné fyzické nebo právnické osobě a identifikaci toho, kdo údaje poskytl,*
>
> *- c) datum poslední změny každého údaje vedeného v registru obyvatel,*
>
> *- d) záznam o udělení nebo odvolání souhlasu subjektu údajů s poskytnutím údajů jiné fyzické nebo právnické osobě podle § 58a.*
>
> *(6) Orgán veřejné moci, který při své činnosti využívá na základě tohoto zákona nebo jiného právního předpisu některé referenční údaje vedené v registru obyvatel, je oprávněn rovněž využívat údaj podle odstavce 1 písm. d) o adrese, na kterou mají být doručovány písemnosti, a údaje podle odstavce 1 písm. j) až m) a odstavce 5 písm. c).*

**Výklad:**

§ 18 obsahuje **katalog údajů vedených v ROB** — strukturován do tří vrstev: referenční údaje (písm. a)–k)), neferenční údaje (písm. l)–o)) a provozní údaje (odst. 5).

#### Referenční údaje (písm. a)–k)) — jádro identity

Jedenáct referenčních údajů tvoří **identifikační profil osoby**:

| Údaj | Komentář |
|---|---|
| Jméno, příjmení, rodné příjmení | Základní identifikační údaje |
| Pohlaví | Vedeno separátně od jména |
| Adresa místa pobytu | Vede se jako **kód adresního místa** (vazba na RUIAN), nikoli textově |
| Datum, místo, okres narození | Místo přes vazbu na RUIAN; cizina jako stát |
| Datum, místo, okres úmrtí | Včetně dne v rozhodnutí o prohlášení za mrtvého |
| Státní občanství (i vícenásobné) | Sleduje skutečný stav |
| Omezení svéprávnosti | Vazba na § 55 a násl. občanského zákoníku |
| Rodinný stav, registrované partnerství | Vazba na matriku |
| Identifikační doklady (čísla, druhy, platnost) | OP, cestovní pas, povolení k pobytu |
| Datová schránka | Typ a ID; vazba na ISDS |

**Klíčový princip:** údaje, které **jsou samy referenčními údaji v jiném ZR**, se v ROB vedou **jen jako referenční vazba** (kód) — nikdy jako duplikát. Adresa, místo narození a místo úmrtí v ROB jsou kódy odkazující na RUIAN.

#### Neferenční údaje (písm. l)–o)) — autentizace a kontakty

- **Telefonní číslo, e-mail** (písm. l)) — pro zasílání zvolených informací (notifikace). Nejsou referenčním údajem — jejich existence ani správnost není závazná.
- **Kvalifikovaný certifikát** (písm. m)) — pro elektronický podpis; sériové číslo, vydavatel, platnost.
- **Data pro elektronickou identifikaci a autentizaci** (písm. n)) — autentizační údaj jen pro občany ČR. **Vede se v jednosměrně šifrované podobě** — což znamená, že ani správce registru nezíská heslo v plaintextu.
- **Časy blokace EID** (písm. o)) — auditní záznamy o stavu autentizačních dat.

#### AIFO pro agendu ROB (odst. 4)

Identifikátorem osoby v ROB je **AIFO pro agendu registru obyvatel** — nikoli ZIFO. Tím je i samotná evidence ROB chráněna před propojováním s dalšími AIS bez převodu přes ORG.

#### Provozní údaje (odst. 5)

Mezi provozní údaje patří mj.:

- záznam o využívání údajů z ROB (audit-trail);
- záznam o poskytnutí údajů jiné osobě podle § 58a (souhlasy);
- datum poslední změny každého údaje;
- záznam o udělení/odvolání souhlasu podle § 58a.

#### Rozšířené oprávnění čerpání (odst. 6)

OVM, který využívá některé referenční údaje, je automaticky oprávněn využívat i:

- adresu pro doručování (písm. d) druhá část),
- ID doklady (písm. j)),
- datovou schránku (písm. k)),
- certifikát (písm. m)),
- datum poslední změny (písm. c) v odst. 5).

Tato „balíčková" logika usnadňuje praktické fungování — orgán, který má přístup k jménu a adrese, automaticky získá i kontaktní údaje pro doručení.

---

### § 19 — Zapisování údajů do ROB

> **§ 19**
>
> *(1) U subjektů údajů uvedených v § 17 písm. a) je editorem Ministerstvo vnitra, které zapisuje údaje uvedené v § 18 odst. 1 písm. a) až i) prostřednictvím informačního systému evidence obyvatel a údaje uvedené v § 18 odst. 1 písm. j), § 18 odst. 1 písm. n), jde-li o data potřebná pro elektronickou identifikaci a autentizaci, § 18 odst. 1 písm. o) a v § 18 odst. 3 prostřednictvím informačního systému občanských průkazů nebo informačního systému cestovních dokladů.*
>
> *(2) U subjektů údajů uvedených v § 17 písm. b) až d) je editorem Policie České republiky nebo Ministerstvo vnitra, které zapisují údaje uvedené v § 18 odst. 1 písm. a) až j) a v § 18 odst. 3 prostřednictvím agendového informačního systému, ve kterém jsou vedeny údaje o cizincích podle jiného právního předpisu.*
>
> *(3) U subjektů údajů uvedených v § 17 písm. e) je editorem Ministerstvo vnitra, které zapisuje údaje uvedené v § 18 odst. 1 písm. a) až i) prostřednictvím informačního systému cizinců8); pokud tak stanoví jiný právní předpis, zapisuje se rovněž údaj uvedený v § 18 odst. 1 písm. j).*
>
> *(4) Jsou-li u subjektů údajů uvedených v § 17 písm. b) až e) vedeny údaje o jménu, popřípadě jménech, a příjmení, zpracovávají se tyto údaje v podobě uvedené v matričním dokladu. Nebyl-li matriční doklad vydán, zpracovávají se údaje o jménu, popřípadě jménech, a příjmení, v podobě uvedené latinkou v cestovním dokladu, v průkazu nebo v potvrzení cizince vydaném podle zákona o pobytu cizinců na území České republiky nebo zákona o azylu.*
>
> *(5) Údaje uvedené v § 18 odst.5 zapisuje do registru obyvatel automatizovanými procesy prostřednictvím informačního systému základních registrů Agentura. Záznamy podle § 18 odst.5 se zapisují v rozsahu*
>
> *- a) kód agendy, kód agendového informačního systému nebo soukromoprávního systému pro využívání údajů, prostřednictvím kterých byly údaje využity, uživatelské jméno fyzické osoby, která je nositelem role, které je neveřejné, a označení subjektu, který údaje využil nebo kterému byly poskytnuty,*
>
> *- b) datum a čas využití nebo poskytnutí údajů,*
>
> *- c) obchodní firma nebo název nebo jméno, popřípadě jména, a příjmení subjektu, kterému jsou na základě žádosti poskytovány údaje podle § 58a, datum a čas udělení nebo odvolání souhlasu subjektu údajů s poskytnutím údajů podle § 58a a identifikátor souhlasu,*
>
> *- d) agendový identifikátor fyzické osoby pro agendu registru obyvatel, jejíž údaje jsou využívány nebo poskytovány,*
>
> *- e) důvod a konkrétní účel využití nebo poskytnutí údajů.*
>
> *(6) Údaje uvedené v § 18 odst. 1 písm. k) zapisuje do registru obyvatel správce informačního systému datových schránek.*
>
> *(7) Údaje uvedené v § 18 odst. 1 písm. l) a m) a v § 18 odst. 1 písm. n), jde-li o požadavek na doplnění fyzického prokázání totožnosti autentizací s využitím dat potřebných pro elektronickou identifikaci a autentizaci, zapisuje do registru obyvatel Agentura na základě požadavku subjektu údajů uplatněného prostřednictvím portálu veřejné správy.*

**Výklad:**

§ 19 určuje **distribuovanou editorovou strukturu** ROB. Editorství je vázáno na **subjekt údajů** (kdo je zapisován) a **druh údaje** (jaký údaj se zapisuje).

#### Editor pro občany ČR (odst. 1)

**Ministerstvo vnitra** je editor pro občany ČR. Zápis se rozkládá mezi tři AIS:

1. **IS evidence obyvatel** (provozovaný MV) — písm. a)–i) v § 18 odst. 1 (jméno, příjmení, pohlaví, adresa, narození, úmrtí, občanství, svéprávnost, rodinný stav).
2. **IS občanských průkazů** nebo **IS cestovních dokladů** — písm. j) (čísla dokladů), n) (data pro EID jen u občanů ČR), o) (zablokování EID).

#### Editor pro cizince (odst. 2 a 3)

Pro cizince podle § 17 písm. b)–d) je editorem **Policie ČR** nebo **Ministerstvo vnitra** — zápis přes AIS cizinců. Pro „jiné osoby" podle § 17 písm. e) je editorem MV přes IS cizinců.

#### Pravopisné pravidlo pro cizince (odst. 4)

Jméno cizince se zpracovává **podle matričního dokladu**; nemá-li, podle cestovního dokladu/průkazu **latinkou**. Toto pravidlo řeší problematiku transliterace ze cyrilice, čínského, arabského písma atd. — pro veřejnou správu se vede jméno v jeho úředně přepsané latinkové podobě.

#### Provozní údaje a vyrozumívání (odst. 5)

Provozní údaje (§ 18 odst. 5) zapisuje **Agentura automatizovaně** přes ISZR. To znamená, že audit-trail nepíše „někdo", nýbrž systém sám — což garantuje neporušitelnost.

#### Datová schránka (odst. 6) a kontaktní údaje (odst. 7)

- **Datová schránka** — editorem je **správce ISDS** (rovněž DIA), který zapisuje typ a ID datové schránky.
- **Telefon, e-mail, EID požadavek** — editorem je **Agentura** **na žádost subjektu údajů** přes portál veřejné správy. Subjekt si tak sám spravuje své kontaktní údaje.

> **Praktický dopad:** Osoba si může na **portál.gov.cz** přihlásit, doplnit telefonní číslo a e-mail — a tyto údaje jsou okamžitě referenčním údajem v ROB. Úřady je pak mohou používat pro zasílání informací.

---

### § 20 — Správce registru obyvatel

> **§ 20**
>
> *(1) Správcem registru obyvatel je Agentura.*
>
> *(2) Agentura zajišťuje poskytování údajů z registru obyvatel podle § 58 a 58a.*
>
> *(3) Agentura kontroluje výkon přenesené působnosti na úseku registru obyvatel u územních samosprávných celků; ustanovení o kontrole výkonu přenesené působnosti krajskými úřady podle zákona o obcích tím není dotčeno.*
>
> *(4) Agentura v registru obyvatel zpracovává údaje potřebné k plnění úkolů stanovených jiným právním předpisem v rozsahu údajů podle § 18.*

**Výklad:**

§ 20 svěřuje správu ROB **Digitální a informační agentuře (DIA)** — od 1. dubna 2023. Předtím (1. července 2010 — 31. března 2023) byla správcem **Správa základních registrů (SZR)** podléhající MV.

#### Rozdělení rolí — editor vs. správce

Důležité rozlišení:

- **Editor** zapisuje a opravuje údaje (MV, Policie ČR — § 19).
- **Správce** provozuje databázi, zajišťuje její bezpečnost, dostupnost, poskytování údajů (DIA).

Editor a správce nejsou totožní subjekty — to je dáno **dělbou kompetencí** a má důsledky pro odpovědnost: za **správnost zápisu** odpovídá editor, za **provoz a bezpečnost** ROB odpovídá DIA.

#### Kontrolní role DIA (odst. 3)

DIA kontroluje **výkon přenesené působnosti** v oblasti ROB u územních samospráv — tedy obecních úřadů, které jako matriční úřady a obce s rozšířenou působností pracují s ROB. Tato kontrola **nemá vliv na obecnou kontrolu** krajských úřadů podle zákona č. 128/2000 Sb., o obcích.

---

### § 22 — Uchovávání a likvidace údajů

> **§ 22**
>
> *(1) Údaje subjektu údajů se uchovávají v registru obyvatel po dobu 50 let od smrti subjektu údajů nebo ode dne nabytí právní moci rozhodnutí soudu o prohlášení za mrtvého. Tímto ustanovením nejsou dotčena ustanovení o uchovávání údajů stanovená v jiných právních předpisech upravujících vedení agendových informačních systémů, prostřednictvím nichž jsou zapisovány údaje vedené v registru obyvatel.*
>
> *(2) Pokud není údaj podle § 18 odst. 1 písm. f) v registru obyvatel veden, údaje subjektu údajů se uchovávají v registru obyvatel po dobu 50 let od poslední aktualizace alespoň jednoho z údajů uvedených v § 18.*
>
> *(3) Po uplynutí doby stanovené v odstavcích 1 a 2 se údaje likvidují17), s výjimkou údajů podle § 18 odst.5, které se vedou ještě po dobu následujících 10 let.*

**Výklad:**

§ 22 stanoví **lhůty uchovávání**. Princip „**50 let po smrti**" odpovídá obvyklým archivním lhůtám a souvisí s ochranou autorských a souvisejících práv (§ 27 autorského zákona).

#### Tři pravidla

1. **Při známé smrti** (odst. 1) — 50 let od smrti nebo právní moci rozhodnutí o prohlášení za mrtvého.
2. **Při neznámé smrti** (odst. 2) — 50 let od poslední aktualizace (kdy osoba „administrativně zmizela").
3. **Likvidace** po 50 letech (odst. 3) — všechny údaje se zlikvidují, **kromě provozních záznamů**, které se uchovávají dalších 10 let pro auditní účely.

Toto pravidlo má řadu dopadů — od archivace osobních dat (po likvidaci nelze osobu v ROB dohledat) až po historický výzkum (do 50 let je možná genealogická badatelská práce přes záznamy v ROB).

---

### § 23 — Nové pořízení údajů

> **§ 23**
>
> *(1) Na základě podnětu subjektu údajů podaného prostřednictvím správního orgánu, který vede agendu evidence obyvatel, nebo správního orgánu, který vede agendu cizinců podle jiného právního předpisu, zajistí Agentura nové pořízení agendového identifikátoru fyzické osoby v registru obyvatel.*
>
> *(2) Ostatní údaje zlikvidované podle § 22 se nově pořídí opakovanou editací z informačního systému evidence obyvatel nebo agendového informačního systému, ve kterém jsou vedeny údaje o cizincích podle jiného právního předpisu nebo jiného příslušného agendového informačního systému, na základě podnětu subjektu údajů.*
>
> *(3) Editor registru obyvatel zapisuje údaje podle posledního stavu vedeného v agendovém informačním systému, pokud subjekt údajů neprokáže jejich změnu.*

**Výklad:**

§ 23 řeší situaci **opětovného pořízení záznamu** po jeho likvidaci. Praktické případy:

- **Osoba je prohlášena za mrtvou**, údaje zlikvidovány, ale po letech se zjistí, že je naživu (vrátila se ze zahraničí).
- **Cizinec opětovně získá pobyt v ČR** po delší době nepřítomnosti.

#### Nové AIFO (odst. 1) — proti historickému profilování

Po žádosti subjektu Agentura zajistí **nové AIFO** — nikoli obnovu starého. Tím se zajišťuje, že **historické záznamy** (např. trestní rejstřík před desetiletími) **nezůstanou propojené** s novou identifikací osoby. Tato úprava chrání před tzv. „digitálním stigmatem".

#### Obnova ostatních údajů (odst. 2)

Ostatní údaje se obnoví **editorovou cestou** — typicky z IS evidence obyvatel (pokud byl zachován tam). Pokud agendový systém nezachoval údaje, obnova není možná a osoba je zapsána „od nuly".

#### Princip posledního stavu (odst. 3)

Editor zapisuje **údaje podle posledního stavu** vedeného v AIS, **pokud subjekt neprokáže změnu**. Toto pravidlo zachovává kontinuitu s předchozími záznamy a klade břemeno prokázat změnu na subjekt.
