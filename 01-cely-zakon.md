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

#### F. Kazuistika

**1. Modelová situace.** Krajský úřad (poskytovatel dotací z evropského fondu) chce přímo z obecního stavebního úřadu získávat hromadně data o stavebnících formou pravidelného exportu z jejich databáze do tabulky, bez napojení přes ISZR/ISSS. Účastníci: krajský úřad (žadatel o data), obecní stavební úřad (správce vlastní evidence), DIA (správce referenčního rozhraní). Důkazy: registrace agend obou úřadů v RPP, popis datového toku, smluvní/technická dokumentace navrhovaného exportu.

**2. Právní otázka.** Lze sdílet údaje mezi dvěma orgány veřejné správy mimo pět typů sdílení a mimo referenční rozhraní vymezené v § 1 písm. b)?

**3. Použitelné právo.**
- *Komentované ustanovení:* § 1 písm. b) — taxativní matice pěti typů sdílení údajů, vše přes referenční rozhraní.
- *Související ustanovení téhož zákona:* § 5 odst. 5 (přístup výhradně přes AIS a ISZR/ISSS), § 5b (jediná výslovná výjimka — přímý přístup pro bezpečnost), § 2 písm. g), h) (definice ISZR a ISSS).
- *Související předpisy:* zákon č. 365/2000 Sb. (ZISVS) — § 2 písm. i) o referenčním rozhraní, jako lex generalis; GDPR čl. 6 (zákonnost zpracování).
- *Judikatura:* obecná zásada legality výkonu veřejné moci (čl. 2 odst. 3 Ústavy, čl. 2 odst. 2 Listiny) — orgán smí činit jen to, co zákon dovoluje; nosně potvrzeno konstantní judikaturou Ústavního soudu k mezím veřejné moci.

**4. Subsumpce.** Navržený přímý export ZÚ ↔ ZÚ mimo referenční rozhraní nespadá do žádného z pěti typů sdílení v § 1 písm. b): jde sice o sdílení mezi orgány veřejné moci, ale ZZR vyžaduje, aby probíhalo přes AIS a ISZR/ISSS (typ „AIS ↔ AIS"). Podmínka „mimo referenční rozhraní" tedy splněna není; přímý export je s § 1 písm. b) v rozporu.

**5. Řešení.** Sdílení je nezbytné realizovat jako vazbu AIS ↔ AIS přes ISSS (úřady, jejichž AIS nezapisují do ZR) nebo ISZR. Krajský úřad musí mít agendu registrovanou v RPP a požadovaná data ve výčtu zpřístupněných údajů. Přímý hromadný export je nepřípustný; vedl by k nezákonnému zpracování osobních údajů. Procesně: ohlášení/registrace agendy, technické napojení AIS přes referenční rozhraní, kód agendy u každého dotazu.

**6. Varianty.** (a) Pokud by šlo o úkol při zajišťování bezpečnosti ČR nebo odhalování trestné činnosti, uplatnil by se § 5b a přímý přístup by byl přípustný. (b) Pokud by „krajský úřad" byl soukromoprávním uživatelem (např. banka), sdílení by spadalo do typu „AIS ↔ soukromoprávní systém", opět jen přes referenční rozhraní.

#### G. Protiargumenty a rizika

- *Protiargument:* „Oba subjekty jsou orgány veřejné moci, mezi sebou si data sdílet mohou." — Neutralizace: § 1 písm. b) nezakládá volné sdílení mezi OVM; stanoví, že každé sdílení musí jít kanálem referenčního rozhraní. Mimo něj chybí zákonný titul zpracování.
- *Protiargument:* „§ 1 je jen úvodní deklarace předmětu, nezakládá povinnosti." — Neutralizace: § 1 nutno číst systematicky s § 5 odst. 5 a definicemi v § 2; teprve výklad celku ukazuje rezervaci sdílení pro referenční rozhraní. § 1 sám o sobě je deklaratorní, ale rámuje výklad operativních ustanovení.
- *Slabé místo:* hranice „referenčního rozhraní" je definována odkazem na ZISVS; v hraničních případech (sdílení mimo ZR a AIS, např. čistě interní agenda) je nutné posoudit, zda vůbec jde o sdílení ve smyslu ZZR.

#### H. Praktický závěr

§ 1 vymezuje, CO zákon dělá (zřizuje registry, stanoví podmínky sdílení) a vytváří uzavřenou matici pěti typů sdílení. V praxi slouží jako výkladové vodítko: jakékoli sdílení údajů ze ZR/AIS musí být podřaditelné jednomu z pěti typů a musí jít přes referenční rozhraní.

**Checklist (advokát / soud / správní orgán / adresát normy):**
- [ ] Spadá zamýšlené sdílení do jednoho z pěti typů podle § 1 písm. b)?
- [ ] Probíhá přes referenční rozhraní (ISZR/ISSS), nebo jde o výjimku § 5b?
- [ ] Je pro něj registrována agenda a má subjekt přístup k požadovaným údajům?
- [ ] Není-li podmínka splněna, hrozí nezákonné zpracování osobních údajů.

**Typicky rozhodné důkazy / podklady:** registrace agend v RPP, technický popis datového toku, doklad o napojení přes ISZR/ISSS, evidence kódů agend.

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

**Judikatura (z místních zdrojů):**

- *NSS* [9 Azs 42/2024 - 46](https://vyhledavac.nssoud.cz/DokumentOriginal/Text/724875) — 17. 9. 2024
  > „informační systém cizinců je agendovým informačním systémem ve smyslu § 2 písm. f) zákona č. 111/2009 Sb., o základních registrech, ve znění pozdějších předpisů. Žalovaná byla při zadržení průkazu o povolení k pobytu stěžovatelky oprávněna využít údaje o jeho platnosti právě z tohoto informačního systému"

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

#### F. Kazuistika

**1. Modelová situace.** Profesní komora (např. komora vykonávající kárnou pravomoc nad svými členy) chce přistupovat k údajům v ROB pro účely kárného řízení a tvrdí, že je „soukromoprávním uživatelem údajů" podle § 2 písm. d), protože jde o samosprávnou korporaci. Současně advokát zastupující klienta tvrdí totéž o sobě. Účastníci: komora, advokát, DIA (posouzení titulu přístupu). Důkazy: zákon zakládající kárnou pravomoc komory, vymezení působnosti.

**2. Právní otázka.** Je subjekt, který vykonává svěřenou veřejnou moc, „orgánem veřejné moci" podle § 2 písm. c), nebo „soukromoprávním uživatelem údajů" podle § 2 písm. d)?

**3. Použitelné právo.**
- *Komentované ustanovení:* § 2 písm. c) (orgán veřejné moci — zahrnuje FO/PO se svěřenou působností v oblasti veřejné správy, notáře, exekutory, insolvenční správce, archivy) a písm. d) (soukromoprávní uživatel — působení, které NENÍ působením OVM).
- *Související ustanovení téhož zákona:* § 5 (přístup OVM) vs. § 5a (přístup soukromoprávního uživatele) — odlišný režim titulu (zákon/souhlas).
- *Související předpisy:* § 1 odst. 1 správního řádu (užší pojem správního orgánu); zákony zakládající kárnou/disciplinární pravomoc jednotlivých komor.
- *Judikatura:* nosný závěr Ústavního soudu, že profesní komory při výkonu veřejnoprávní disciplinární pravomoci jednají jako vykonavatelé veřejné moci (veřejnoprávní korporace s delegovanou působností).

**4. Subsumpce.** Rozhodující je povaha činnosti: vykonává-li subjekt svěřenou působnost v oblasti veřejné správy (kárné řízení komory), je „orgánem veřejné moci" podle písm. c) bez ohledu na soukromoprávní formu. Klíčová negativní podmínka písm. d) — „působení, které není působením orgánu veřejné moci" — pak splněna není; komora v kárné věci není soukromoprávním uživatelem. Advokát naopak při zastupování klienta nevykonává veřejnou moc, soukromoprávním uživatelem ovšem také není automaticky — musí mít zvláštní zákonný titul přístupu.

**5. Řešení.** Komora v kárném řízení přistupuje jako OVM (§ 5). Advokát přistupuje jen tehdy, dává-li mu zvláštní zákon postavení soukromoprávního uživatele, jinak nemá přístup do ZR vůbec a údaje získává jinou cestou (od klienta, soudu). Procesně: ověřit, podle jakého titulu subjekt jedná, a tomu přizpůsobit registraci agendy a režim § 5/§ 5a.

**6. Varianty.** (a) Kdyby komora čerpala údaje pro evidenci svých členů jako vnitřní spolkovou agendu bez výkonu veřejné moci, mohla by být soukromoprávním uživatelem podle písm. d) — s nutností zvláštního zákonného titulu. (b) Notář při sepisu veřejné listiny je výslovně OVM podle písm. c), byť jde o privatizovaný výsek veřejné moci.

#### G. Protiargumenty a rizika

- *Protiargument:* „Soukromoprávní forma subjektu (komora, exekutor) určuje, že jde o soukromoprávního uživatele." — Neutralizace: písm. c) výslovně zahrnuje FO/PO se svěřenou působností i notáře a exekutory; rozhodující je funkční (materiální) kritérium výkonu veřejné moci, nikoli forma.
- *Protiargument:* „Editor podle písm. i) je každý, kdo fakticky zapisuje data." — Neutralizace: editorem je jen OVM zákonem k zápisu oprávněný; faktická manipulace s daty bez zákonného zmocnění editorství nezakládá.
- *Slabé místo:* hranice mezi výkonem veřejné moci a soukromým působením téhož subjektu (komora) může být sporná u smíšených agend; nutné posuzovat jednotlivý úkon, ne subjekt jako celek.

#### H. Praktický závěr

§ 2 je výkladový slovník zákona; pojmy zde mají striktně právní význam. V praxi se nejčastěji řeší, zda subjekt je OVM (písm. c) — režim § 5) nebo soukromoprávní uživatel (písm. d) — režim § 5a), protože od toho se odvíjí titul i kanál přístupu.

**Checklist (advokát / soud / správní orgán / adresát normy):**
- [ ] Vykonává subjekt v dané věci veřejnou moc (→ OVM, písm. c) nebo soukromé působení (→ písm. d)?
- [ ] Je-li to editor, má zákonné zmocnění k zápisu (písm. i)?
- [ ] Je „agenda" správně vymezena jako ucelená oblast působení (písm. e)?
- [ ] Probíhá přístup přes AIS (písm. f) napojený na ISZR/ISSS (písm. g, h)?

**Typicky rozhodné důkazy / podklady:** zákon zakládající působnost subjektu, registrace agendy v RPP, doklad o editorství.

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

**Judikatura (z místních zdrojů):**

- *NSS* [4 As 372/2021 - 74](https://vyhledavac.nssoud.cz/DokumentOriginal/Text/701208) — 9. 6. 2022
  > „RÚIAN patří mezi základní registry upravené v § 3 zákona č. 111/2009 Sb., o základních registrech. Jak vyplývá z § 4 odst. 4 téhož zákona, údaje v základních registrech se považují za správné, pokud není prokázán opak. Je současně zřejmé, že aktuálnost základních registrů je klíčová pro chod celého systému. Z tohoto důvodu dochází k řešení nově zjištěných problémů automaticky a z úřední povinnosti"
- *NSS* [43 A 44/2019 - 13](https://vyhledavac.nssoud.cz/DokumentOriginal/Text/437735) — 19. 6. 2019
  > „Registr územní identifikace je základním registrem [§ 3 písm. c) zákona č. 111/2009 Sb., o základních registrech, ve znění pozdějších předpisů (dále jen „zákon o základních registrech“)] a veřejným seznamem (§ 30 odst. 1 zákona o základních registrech). … Zákon o základních registrech nepředpokládá, že by faktickému úkonu spočívajícímu v provedení zápisu určitého údaje v registru územní identifikace, který je ze své povahy pouze informativního charakteru, byť je s ním spojena vyvratitelná domněnka správnosti, mělo předcházet formalizované řízení a mělo se o něm vydávat formalizované rozhodnutí…"

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

#### F. Kazuistika

**1. Modelová situace.** Provozovatel nové centrální evidence (např. evidence sociálních dávek) tvrdí, že jeho systém má povahu „základního registru", a proto by jeho údaje měly požívat domněnky správnosti referenčního údaje a být závazné pro ostatní orgány. Ministerstvo to chce potvrdit vnitřním předpisem. Účastníci: provozovatel evidence, gestor (ministerstvo), DIA. Důkazy: zřizovací akt evidence, popis dat a vazeb.

**2. Právní otázka.** Lze evidenci povýšit na „základní registr" jinak než novelou § 3 — např. podzákonným předpisem nebo výkladem?

**3. Použitelné právo.**
- *Komentované ustanovení:* § 3 — taxativní výčet čtyř základních registrů (ROB, registr osob, RUIAN, RPP).
- *Související ustanovení téhož zákona:* § 2 písm. a) (základní registr = jen registr uvedený v § 3 — čistě odkazová definice), § 4 (vlastnosti referenčních údajů, které má jen ZR).
- *Související předpisy:* zákon č. 365/2000 Sb. (ISVS) — obecná kategorie informačního systému veřejné správy, do níž evidence spadá, aniž by byla ZR.
- *Judikatura:* zásada, že rozsah zákonných institutů nelze rozšiřovat podzákonným předpisem (čl. 79 odst. 3 Ústavy — meze prováděcích předpisů); nosně potvrzeno judikaturou Ústavního soudu k zákazu rozšiřování zákona vyhláškou.

**4. Subsumpce.** Evidence sociálních dávek není uvedena ve výčtu § 3, a podle § 2 písm. a) tedy není „základním registrem". Vlastnosti referenčního údaje podle § 4 (domněnka správnosti, ochrana dobré víry) se na ni nevztahují. Podmínka „základnosti" — uvedení v § 3 — splněna není.

**5. Řešení.** Bez novely § 3 nelze evidenci povýšit na ZR. Vnitřní předpis ani vyhláška to nezvládnou — šlo by o překročení mezí prováděcího předpisu. Evidence zůstává běžným ISVS (typicky AIS) a její údaje nemají závaznost referenčního údaje. Cesta: legislativní iniciativa k novele § 3, nebo využití existujících ZR přes referenční vazby.

**6. Varianty.** (a) Pokud by zákonodárce novelizoval § 3 a doplnil pátý registr, získal by tento status ZR i s režimem § 4. (b) Pokud evidence jen čerpá referenční údaje ze čtyř ZR a vede vlastní agendové údaje, funguje legitimně jako AIS bez nároku na „základnost".

#### G. Protiargumenty a rizika

- *Protiargument:* „Materiálně náš systém splňuje znaky základního registru (je centrální, závazný), takže jím je." — Neutralizace: § 2 písm. a) je formální/odkazová definice — rozhodující je výlučně uvedení v § 3, nikoli materiální podobnost.
- *Protiargument:* „Výčet § 3 lze rozšířit analogií." — Neutralizace: jde o taxativní výčet zakládající zvláštní právní režim; analogické rozšiřování je vyloučeno, šlo by o nepřípustné dotváření práva v neprospěch právní jistoty.
- *Slabé místo:* zkratky RPO vs. RPP se v praxi zaměňují; chyba v identifikaci registru může vést k chybnému určení správce a editora.

#### H. Praktický závěr

§ 3 uzavřeně vyjmenovává čtyři základní registry. Žádný jiný systém není ZR, dokud jej zákonodárce do § 3 nedoplní. V praxi slouží jako kontrolní bod: než někdo přizná údajům závaznost referenčního údaje, musí ověřit, že pocházejí z jednoho ze čtyř registrů § 3.

**Checklist (advokát / soud / správní orgán / adresát normy):**
- [ ] Je dotčený systém uveden ve výčtu § 3 (jen pak je ZR)?
- [ ] Je správně rozlišeno ROS/RPO (registr osob, písm. b) od RPP (registr práv a povinností, písm. d)?
- [ ] Která referenční vazba propojuje dotčené registry (ROB→RUIAN, ROS→ROB apod.)?
- [ ] Nepožaduji závaznost referenčního údaje u systému, který ZR není?

**Typicky rozhodné důkazy / podklady:** znění § 3, zřizovací akt dotčené evidence, dokumentace referenčních vazeb.

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

**Judikatura (z místních zdrojů):**

- *NSS* [29 A 33/2023 - 26](https://vyhledavac.nssoud.cz/DokumentOriginal/Text/769182) — 19. 12. 2025
  > „Referenční údaje z RÚIAN jsou totiž do katastru nemovitostí přebírány automatickou či poloautomatickou cestou, přičemž tyto referenční údaje jsou ve smyslu § 4 odst. 4 zákona o základních registrech považovány za správné, tj. odpovídající skutečnosti. Zákon tedy v tomto případě nepředpokládá bližší posuzování přejímaných změn, což potvrzuje judikatura správních soudů…"
- *NSS* [62 A 51/2023 - 60](https://vyhledavac.nssoud.cz/DokumentOriginal/Text/717238) — 30. 11. 2023
  > „Podle § 32 odst. 1 katastrálního zákona je možné jiné údaje katastru přejímat z jiných informačních systémů, registrů, rejstříků nebo evidencí veřejné správy, pokud … údaje v nich uvedené požívají ochrany dobré víry v jejich pravdivost a úplnost. Základní registry, mezi které patří i RÚIAN, přitom jistě splňují druhou podmínku. V souladu s § 4 odst. 6 zákona o základních registrech ten, kdo vychází z referenčního údaje, je v dobré víře, že stav referenčního údaje v základním registru odpovídá skutečnému stavu věci, ledaže musel vědět o jeho nesprávnosti"
- *NSS* [41 Af 6/2025 - 35](https://vyhledavac.nssoud.cz/DokumentOriginal/Text/744980) — 22. 8. 2025
  > „To, že je tedy v systému RÚIAN jako technickoekonomický atribut nemovitosti žalobců uvedeno připojení na vodovod, ještě neznamená, že se jedná o vodovod podle citovaného zákona, na nějž odkazuje § 10c odst. 1 zákona o místních poplatcích. Současně podle § 4 odst. 4 zákona č. 111/2009 Sb., o základních registrech, ve znění pozdějších předpisů je referenční údaj … zapsaný v RÚIAN považován za správný, pokud není prokázán opak nebo pokud nevznikne oprávněná pochybnost o správnosti referenčního údaje"

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

#### F. Kazuistika

**1. Modelová situace.** Banka poskytla úvěr 2 mil. Kč osobě, která se prokázala občanským průkazem; identifikační údaje (jméno, datum narození, adresa) byly v souladu s referenčními údaji v ROB. Po roce vyjde najevo, že v ROB došlo k záměně dvou osob (osoba A vystupovala s referenčními údaji osoby B v důsledku chyby editora při zápisu). Skutečná osoba B (jejíž údaje byly „obsazeny") nyní popírá smluvní vztah a tvrdí, že úvěr nečerpala. Účastníci: banka (důvěřovala ROB), osoba A (fakticky čerpala úvěr), osoba B (poškozená záměnou), editor (MV/obecní úřad). Důkazy: úvěrová smlouva, výpis z ROB k datu úvěru, doklad totožnosti, audit-trail ISZR, podkladové dokumenty editora.

**2. Právní otázka.** Může osoba B namítat vůči bance, že referenční údaj v ROB neodpovídal skutečnosti, a zprostit se tak právních následků jednání učiněného bankou v důvěře v tento údaj?

**3. Použitelné právo.**
- *Komentované ustanovení:* § 4 odst. 4 (domněnka správnosti referenčního údaje), odst. 6 (domněnka dobré víry toho, kdo z údaje vychází), odst. 7 (zákaz namítat nesprávnost vůči poctivému uživateli — ledaže dotčený prokáže nesprávnost A že ji nezpůsobil).
- *Související ustanovení téhož zákona:* § 4 odst. 2 (odpovědnost editora za soulad se zdrojovým dokumentem), odst. 5 (informativní povaha údaje označeného jako nesprávný), § 5 odst. 2 (OVM neověřuje), § 5a odst. 4 (soukromoprávní uživatel neověřuje), § 14 odst. 6 (reklamace).
- *Související předpisy:* § 980 a násl. občanského zákoníku (materiální publicita veřejných seznamů — obdobná ochrana důvěry, např. u katastru); GDPR čl. 16 (právo na opravu).
- *Judikatura:* nosný závěr civilní judikatury Nejvyššího soudu k ochraně dobré víry nabyvatele důvěřujícího zápisu ve veřejném seznamu — dobrá víra se presumuje a její vyvrácení tíží toho, kdo ji popírá.

**4. Subsumpce.** Banka „vyšla z referenčního údaje" → uplatní se domněnka dobré víry (odst. 6), vyvratitelná jen důkazem, že banka o nesprávnosti vědět musela (nic tomu nenasvědčuje, údaje byly konzistentní). Osoba B chce namítat nesprávnost (odst. 7); k úspěchu musí kumulativně prokázat (i) že údaj byl nesprávný (záměna prokázána) A SOUČASNĚ (ii) že nesprávnost nezpůsobila. Druhá podmínka je zde splněna (chybu způsobil editor, nikoli B). První rovněž. Obě podmínky odst. 7 by tedy mohly být naplněny ve prospěch B.

**5. Řešení.** Klíčové je, že odst. 7 chrání důvěru jen vůči tomu, „jehož se referenční údaj týká". Posoudit nutno, vůči komu banka jednala: jednala-li s osobou A jako se smluvní stranou (a údaje ROB jen ověřovala), pak smlouva váže A, nikoli B — B není smluvní stranou a netřeba odst. 7 k jejímu prospěchu ani neprospěchu. Vede-li však banka pohledávku formálně proti B (na základě záměny), může B prolomit ochranu důvěry podle odst. 7, neboť prokáže nesprávnost i to, že ji nezpůsobila. Banka se pak musí hojit na osobě A (bezdůvodné obohacení, podvod) a případně uplatnit odpovědnost státu za nesprávný úřední postup editora. Procesně: reklamace údaje (§ 14 odst. 6), označení údaje jako nesprávného (§ 4 odst. 4) s účinkem informativní povahy do nápravy.

**6. Varianty.** (a) Kdyby byl údaj v době úvěru již označen jako nesprávný (odst. 5), banka by se nemohla dovolávat dobré víry — údaj měl jen informativní povahu a banka jej měla ověřit. (b) Kdyby chybu v ROB zavinila sama osoba B (např. uvedla nepravdivé doklady), nesplní druhou podmínku odst. 7 a nemohla by nesprávnost namítat — ochrana banky by obstála.

#### G. Protiargumenty a rizika

- *Protiargument:* „Domněnka správnosti činí referenční údaj nevyvratitelným." — Neutralizace: jde o domněnku vyvratitelnou (odst. 4) — padá důkazem opaku nebo oprávněnou pochybností; tehdy editor údaj označí jako nesprávný a ten má jen informativní povahu.
- *Protiargument:* „Editor odpovídá za pravdivost údaje, takže za škodu vždy ručí stát." — Neutralizace: editor odpovídá jen za soulad zápisu se zdrojovým dokumentem (odst. 2), nikoli za pravdivost samotného dokumentu; odpovědnost státu je dána jen při nesprávném úředním postupu, ne při věrném přepisu vadného podkladu.
- *Slabé místo:* odst. 7 chrání jen vztah mezi poctivým uživatelem a „tím, jehož se údaj týká"; v třístranných situacích (záměna identit) je nutné pečlivě určit, kdo je smluvní stranou — jinak hrozí chybná aplikace ochrany důvěry.

#### H. Praktický závěr

§ 4 je jádrem zákona: zakládá domněnku správnosti referenčního údaje, povinnosti editora, lhůtu 3 pracovních dnů a trojstupňovou ochranu důvěry (odst. 4, 6, 7). V praxi znamená, že kdo jedná v důvěře v referenční údaj, je chráněn; prolomit ochranu lze jen splněním přísných podmínek odst. 7.

**Checklist (advokát / soud / správní orgán / adresát normy):**
- [ ] Byl údaj v rozhodné době referenčním a nebyl označen jako nesprávný (jinak jen informativní povaha — odst. 5)?
- [ ] Vyšel uživatel skutečně z referenčního údaje (presumpce dobré víry — odst. 6)?
- [ ] Chce-li dotčený namítat nesprávnost: prokáže kumulativně nesprávnost I to, že ji nezpůsobil (odst. 7)?
- [ ] Odpovídá editor jen za soulad se zdrojovým dokumentem (odst. 2), nebo jde o nesprávný úřední postup?
- [ ] Byla podána reklamace podle § 14 odst. 6 a dodržena lhůta 3 prac. dnů (odst. 3)?

**Typicky rozhodné důkazy / podklady:** výpis z ROB k rozhodnému datu, podkladové dokumenty editora (matriční doklad, listina o pobytu), audit-trail ISZR, doklad totožnosti, smluvní dokumentace.

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

#### F. Kazuistika

**1. Modelová situace.** Občan v dubnu nahlásí na úřadě změnu rodinného stavu (sňatek). Editor agendy ji do svého AIS zapíše až po 9 pracovních dnech. Mezitím jiný úřad čerpá z AIS starý údaj a vydá rozhodnutí na jeho základě. Občan namítá průtahy a tvrdí, že editor porušil lhůtu pro zápis. Účastníci: občan, editor (správce AIS), čerpající úřad. Důkazy: datum, kdy se editor o změně dozvěděl, datum zápisu, log AIS.

**2. Právní otázka.** Jaká je nejzazší lhůta pro zápis údaje do agendového informačního systému a kdy její běh počíná?

**3. Použitelné právo.**
- *Komentované ustanovení:* § 4a odst. 3 — zápis do AIS bez zbytečného odkladu, nejpozději do 10 pracovních dnů ode dne, kdy se editor o vzniku/změně skutečnosti dozví.
- *Související ustanovení téhož zákona:* § 4 odst. 3 (kratší lhůta 3 prac. dnů pro referenční údaj v ZR), § 4a odst. 2 (zápis editorem nebo využití z jiného ZR/AIS), § 5 odst. 4 (notifikace editora).
- *Související předpisy:* zákon č. 12/2020 Sb., o právu na digitální služby (vložil § 4a); ZISVS jako lex generalis pro AIS.
- *Judikatura:* obecné zásady ochrany před nečinností a průtahy ve veřejné správě (§ 80 správního řádu) — analogicky k vymáhání včasného zápisu.

**4. Subsumpce.** Lhůta pro AIS je 10 pracovních dnů (odst. 3); primárně však „bez zbytečného odkladu". Editor zapsal 9. pracovní den — formálně v limitu 10 dnů. Otázka je, zda neporušil pravidlo „bez zbytečného odkladu", pokud zápis mohl provést dříve. Podmínka maximální lhůty splněna; podmínka „bez zbytečného odkladu" sporná podle okolností.

**5. Řešení.** Zápis 9. den je v zákonné toleranci 10 prac. dnů, ale „bez zbytečného odkladu" je primární pravidlo — jsou-li podklady úplné a nic nebrání rychlejšímu zápisu, prodlení může být vadou. Pro občana je podstatné, že jde o AIS (10 dnů), nikoli o referenční údaj v ZR (3 dny). Procesně: stížnost na průtahy, popř. opatření proti nečinnosti; čerpající úřad nese riziko, že čerpal neaktuální údaj z AIS — měl zvážit § 5 odst. 3 (referenční údaj se z AIS bere jen v historické verzi).

**6. Varianty.** (a) Šlo-li by o referenční údaj zapisovaný do ZR, platila by lhůta 3 prac. dnů (§ 4 odst. 3) a zápis 9. den by byl opožděný. (b) Vznikne-li údaj automatickým převzetím z jiného ZR/AIS (odst. 2), neběží samostatná desetidenní lhůta editora, neboť údaj se „využije", nikoli vytváří.

#### G. Protiargumenty a rizika

- *Protiargument:* „Deset pracovních dnů je vždy v pořádku." — Neutralizace: jde o maximum; nadřazené pravidlo je „bez zbytečného odkladu" — bezdůvodné vyčkávání do konce lhůty může být vadou postupu.
- *Protiargument:* „AIS má stejný režim správnosti jako ZR." — Neutralizace: AIS nevede referenční údaje s domněnkou správnosti; jeho aktuální údaj nemá závaznost referenčního údaje (srov. § 5 odst. 3).
- *Slabé místo:* určení okamžiku „kdy se editor dozvěděl" je skutkové; bez logu/podání nelze počátek lhůty spolehlivě prokázat.

#### H. Praktický závěr

§ 4a sjednocuje pravidla zápisu do AIS: údaje vznikají při výkonu agendy nebo se přebírají z jiného systému, lhůta zápisu je 10 pracovních dnů (oproti 3 dnům u ZR). AIS nevede referenční údaje.

**Checklist (advokát / soud / správní orgán / adresát normy):**
- [ ] Jde o údaj v AIS (lhůta 10 prac. dnů) nebo referenční údaj v ZR (3 prac. dny)?
- [ ] Byl zápis proveden „bez zbytečného odkladu", nejen v rámci maxima?
- [ ] Vznikl údaj zápisem editora, nebo převzetím z jiného ZR/AIS (odst. 2)?
- [ ] Nebere čerpající orgán z AIS údaj, který má brát jen v historické verzi (§ 5 odst. 3)?

**Typicky rozhodné důkazy / podklady:** podání/oznámení zakládající skutečnost, log zápisu v AIS, doklad o datu vědomosti editora.

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

**Judikatura (z místních zdrojů):**

- *NSS* [51 A 1/2022 - 100](https://vyhledavac.nssoud.cz/DokumentOriginal/Text/705205) — 31. 8. 2022
  > „Zmocnění, které žalovaný dovozoval z § 32 odst. 1 katastrálního zákona ve spojení s § 5 odst. 1 zákona č. 111/2009 Sb., o základních registrech, jej neopravňovalo k učiněnému postupu. … žalovaný zaměnil postup spočívající v přebírání jiných údajů ze základních registrů s postupem, v jehož důsledku došlo k výmazu nemovitostí z LV žalobců…"

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

#### F. Kazuistika

**1. Modelová situace.** Stavební úřad zahájí řízení o odstranění stavby. V rámci podání vyzve účastníka, aby doložil výpisem z evidence obyvatel své trvalé bydliště a výpisem z katastru/RUIAN adresu stavby — přestože obě data jsou referenčními údaji dostupnými úřadu přes ROB a RUIAN. Účastník namítá, že je úřad nesmí požadovat. Účastníci: stavební úřad (OVM), účastník řízení, editoři údajů. Důkazy: výzva úřadu, registrace agendy stavebního úřadu v RPP a výčet zpřístupněných údajů, log přístupu.

**2. Právní otázka.** Smí orgán veřejné moci požadovat po osobě doložení údaje, který je veden jako referenční údaj a je úřadu zpřístupněn pro výkon jeho agendy?

**3. Použitelné právo.**
- *Komentované ustanovení:* § 5 odst. 1 (využití jen v rozsahu potřebném a v rámci výčtu zpřístupněných údajů pro registrovanou agendu), odst. 2 (zákaz požadovat doložení referenčních údajů — s výjimkami a) až d), odst. 5 (přístup výhradně přes AIS a ISZR/ISSS).
- *Související ustanovení téhož zákona:* § 4 odst. 4–6 (domněnka správnosti a dobrá víra — proto netřeba ověřovat), § 5 odst. 4 (notifikace editora při nesouladu), § 51 odst. 6 písm. l) (výčet zpřístupněných údajů v registraci agendy), § 55 (registrace pro výkon agendy).
- *Související předpisy:* zákon č. 12/2020 Sb., o právu na digitální služby (vymahatelné právo na neopakované dokládání); GDPR čl. 5 odst. 1 písm. c) (minimalizace) a čl. 6 (zákonnost).
- *Judikatura:* zásada „neptej se občana na to, co stát ví" jako projev dobré správy; nosně podpořeno judikaturou správních soudů k zákazu zatěžovat účastníka opatřováním podkladů, jež má úřad k dispozici.

**4. Subsumpce.** Adresa pobytu (ROB) i adresa stavby (RUIAN) jsou referenční údaje. Je-li agenda stavebního úřadu registrována a tyto údaje jsou ve výčtu zpřístupněných (typicky ano), pak podle odst. 2 úřad nesmí jejich doložení požadovat. Žádná z výjimek a)–d) není dána (údaj je zpřístupněn, není označen jako nesprávný, není pochybnost, nejde o bezpečnostní řízení). Zákonná podmínka pro výzvu k doložení tedy splněna není; výzva je protizákonná.

**5. Řešení.** Úřad si oba údaje opatří sám čerpáním z ROB a RUIAN přes svůj AIS a ISZR (odst. 5), bez ověřování správnosti (§ 4). Výzva k doložení je vadná; účastník se může bránit námitkou, stížností, případně v odvolání. Procesně: úřad doplní spis výpisem ze ZR vlastním úkonem; zjistí-li nesoulad, neopravuje sám, ale notifikuje editora (odst. 4). Riziko pro úřad: požadováním nadbytečných podkladů zatěžuje účastníka a porušuje § 5 odst. 2 i právo na digitální služby.

**6. Varianty.** (a) Pokud daný údaj NENÍ ve výčtu zpřístupněných údajů pro agendu stavebního úřadu (výjimka a), úřad jej zpřístupněn nemá a smí jej po účastníkovi požadovat. (b) Vznikne-li u úřadu oprávněná pochybnost o správnosti adresy (výjimka c), např. zjevný rozpor s místním šetřením, smí doložení požadovat a současně notifikuje editora.

#### G. Protiargumenty a rizika

- *Protiargument:* „Pro jistotu si vyžádáme doklad od občana, ať máme ověřeno." — Neutralizace: § 5 odst. 2 ověřování výslovně vylučuje (mimo výjimky a–d); referenční údaj se nesmí ověřovat, redundantní vyžádání je nezákonné.
- *Protiargument:* „Úřad může k registru přistoupit i přímo, mimo AIS." — Neutralizace: odst. 5 stanoví přístup výhradně přes AIS a ISZR/ISSS; přímý přístup je možný jen v režimu § 5b (bezpečnost).
- *Slabé místo:* hranice „oprávněné pochybnosti" (výjimka c) je neostrá; orgán musí pochybnost umět odůvodnit, jinak se výjimka stává záminkou k obcházení zákazu doložení.

#### H. Praktický závěr

§ 5 je v praxi nejfrekventovanější: zakazuje požadovat po osobě doložení referenčních údajů, které úřad má zpřístupněny (princip „write once / neptej se občana"), a nařizuje přístup výhradně přes AIS a ISZR/ISSS. Výjimky jsou jen čtyři (a–d).

**Checklist (advokát / soud / správní orgán / adresát normy):**
- [ ] Je požadovaný údaj referenčním a ve výčtu zpřístupněných údajů pro agendu (§ 51 odst. 6 písm. l)?
- [ ] Není dána některá z výjimek § 5 odst. 2 písm. a)–d)?
- [ ] Čerpá orgán údaj přes vlastní AIS a ISZR/ISSS (odst. 5), nikoli mimo rozhraní?
- [ ] Při zjištěném nesouladu — notifikoval orgán editora (odst. 4) místo vlastní opravy?
- [ ] Nepožaduje orgán po účastníkovi nadbytečné podklady v rozporu s právem na digitální služby?

**Typicky rozhodné důkazy / podklady:** registrace agendy a výčet zpřístupněných údajů v RPP, log přístupu přes ISZR, znění výzvy úřadu, doklad o případné oprávněné pochybnosti.

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

#### F. Kazuistika

**1. Modelová situace.** Banka v rámci uzavírání úvěru ověřuje klienta a chce z ROB čerpat nejen údaje nutné pro identifikaci podle AML zákona, ale i údaj o rodinném stavu a omezení svéprávnosti, který by se jí hodil pro scoring. Klient současně podepsal obecný „souhlas se zpracováním osobních údajů" v marketingových podmínkách. Účastníci: banka (soukromoprávní uživatel), klient (subjekt údajů), DIA. Důkazy: registrace agendy AML s výčtem zpřístupněných údajů, text souhlasu, log SPSVU.

**2. Právní otázka.** V jakém rozsahu smí soukromoprávní uživatel čerpat referenční údaje — a postačí k rozšíření rozsahu obecný souhlas subjektu, nebo je rozhodující výčet údajů zpřístupněných v rámci agendy?

**3. Použitelné právo.**
- *Komentované ustanovení:* § 5a odst. 1 (zákonný titul — účel a rozsah dle zvláštního zákona, jen výčet zpřístupněných údajů v agendě), odst. 2 (titul souhlasu — účel a rozsah dle souhlasu), odst. 3 (kanál — AIS určený ohlašovatelem nebo SPSVU napojený na ISZR/ISSS), odst. 4 (neověřování správnosti).
- *Související ustanovení téhož zákona:* § 5 odst. 3 a 4 (použijí se obdobně — odst. 5), § 2 písm. d) (soukromoprávní uživatel), § 8a (povinnosti SPSVU).
- *Související předpisy:* zákon č. 253/2008 Sb. (AML) — titul a rozsah identifikace klienta; GDPR čl. 6 odst. 1 písm. a) a c), čl. 7 (podmínky souhlasu — svobodný, konkrétní, informovaný); zákon č. 21/1992 Sb., o bankách (§ 38a).
- *Judikatura:* nosný závěr k tomu, že souhlas se zpracováním osobních údajů musí být konkrétní a informovaný ve vztahu k danému účelu; paušální souhlas „pro všechno" je neúčinný (konstantní výklad ÚOOÚ a soudů k GDPR).

**4. Subsumpce.** Pro AML identifikaci jedná banka podle zákonného titulu (odst. 1) — smí čerpat jen údaje ve výčtu zpřístupněných pro agendu AML a v rozsahu potřebném k úkonu. Rodinný stav a omezení svéprávnosti pro scoring do účelu AML nespadají; rozsah podle odst. 1 splněn není. Obecný marketingový souhlas (odst. 2) není konkrétní a informovaný ve vztahu k čerpání těchto referenčních údajů, a neúčinně rozšiřuje rozsah; podmínka odst. 2 rovněž splněna není.

**5. Řešení.** Banka smí čerpat jen údaje zpřístupněné pro agendu AML v rozsahu potřebném k identifikaci klienta. Pro scoring nemá ani zákonný titul (odst. 1), ani účinný souhlas (odst. 2) — paušální souhlas nestačí. Čerpání rodinného stavu/svéprávnosti by bylo nezákonným zpracováním. Procesně: čerpání přes SPSVU napojený na ISZR (odst. 3) s kódem agendy; neověřovat správnost (odst. 4); při nesouladu notifikovat editora (odst. 5 → § 5 odst. 4).

**6. Varianty.** (a) Pokud by zvláštní zákon (např. úvěrový) bance výslovně přiznal právo čerpat údaj o svéprávnosti, jednala by podle odst. 1 v rozšířeném rozsahu. (b) Pokud by klient udělil konkrétní, informovaný souhlas přesně k čerpání rodinného stavu pro daný účel, mohla by banka postupovat podle odst. 2 v rozsahu souhlasu.

#### G. Protiargumenty a rizika

- *Protiargument:* „Klient podepsal souhlas, takže můžeme čerpat cokoli." — Neutralizace: odst. 2 váže rozsah na účel stanovený v souhlasu; paušální souhlas není konkrétní ani informovaný (čl. 7 GDPR) a rozsah čerpání nerozšiřuje.
- *Protiargument:* „Soukromý subjekt může referenční údaj sám ověřit u zdroje." — Neutralizace: odst. 4 stanoví, že soukromoprávní uživatel neověřuje; požívá ochrany dobré víry podle § 4 odst. 6, ověřování je nadbytečné a může být zásahem.
- *Slabé místo:* hranice mezi „zákonným titulem" a „souhlasem" se může překrývat; je nutné jasně určit právní základ čerpání, jinak hrozí záměna rozsahu zpracování.

#### H. Praktický závěr

§ 5a otevírá soukromé sféře (banky, pojišťovny, poskytovatelé eID) přístup k referenčním údajům ve dvou režimech — zákonný titul (rozsah dle zákona) a souhlas (rozsah dle souhlasu) — vždy jen v rozsahu potřebném a v rámci výčtu zpřístupněných údajů, přes SPSVU/AIS napojený na ISZR/ISSS, bez ověřování správnosti.

**Checklist (advokát / soud / správní orgán / adresát normy):**
- [ ] Jaký je titul čerpání — zákon (odst. 1) nebo souhlas (odst. 2)?
- [ ] Je rozsah čerpání v mezích účelu a výčtu zpřístupněných údajů?
- [ ] Je souhlas konkrétní a informovaný k danému účelu (ne paušální)?
- [ ] Probíhá čerpání přes AIS/SPSVU napojený na ISZR/ISSS s kódem agendy (odst. 3)?
- [ ] Neověřuje uživatel zbytečně správnost (odst. 4) a notifikuje editora při nesouladu (odst. 5)?

**Typicky rozhodné důkazy / podklady:** registrace agendy a výčet zpřístupněných údajů, text souhlasu subjektu, zvláštní zákon zakládající titul, log SPSVU, kód agendy.

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

#### F. Kazuistika

**1. Modelová situace.** Útvar policie při vyšetřování série loupeží potřebuje rychle ztotožnit pachatele popsaného jen znaky (přibližný věk, bydliště v určité oblasti) a vyžádá si přímý přístup do AIS evidence obyvatel mimo ISZR, s argumentem, že integrovaný přístup je pomalý a zanechává auditní stopu, kterou nelze v utajeném řízení připustit. Finanční úřad téhož dne žádá o stejný přímý přístup pro účely vymáhání daňového nedoplatku. Účastníci: policie, finanční úřad, správce AIS, DIA. Důkazy: spisový materiál o účelu, právní kvalifikace úkonu.

**2. Právní otázka.** Pro které účely lze využít přímý přístup do AIS mimo referenční rozhraní a vztahuje se výjimka i na vymáhání daní?

**3. Použitelné právo.**
- *Komentované ustanovení:* § 5b odst. 1 — taxativní výčet účelů (a) bezpečnost ČR, b) obrana, c) veřejná bezpečnost a ochrana života/zdraví, d) předcházení/odhalování/stíhání trestné činnosti, e) významný hospodářský/finanční zájem ČR/EU, f) ochrana práv osob v řízení před soudem), odst. 2 (nepoužití pravidel o ISZR/ISSS).
- *Související ustanovení téhož zákona:* § 5 odst. 5 (obecné pravidlo — vše přes AIS a ISZR/ISSS), § 60 (blokace zpřístupnění záznamů), § 60a (přístup MV, PČR, zpravodajských služeb k záznamům).
- *Související předpisy:* zákon č. 273/2008 Sb., o Policii ČR; zákon č. 412/2005 Sb., o ochraně utajovaných informací; GDPR / zákon č. 110/2019 Sb. (zpracování pro účely předcházení a vyšetřování trestných činů).
- *Judikatura:* nosný požadavek judikatury ÚS a ESLP, že zásahy do informačního sebeurčení musí mít zákonný podklad, sledovat legitimní cíl a být proporcionální; výjimky z ochrany se vykládají restriktivně.

**4. Subsumpce.** Vyšetřování loupeží spadá pod písm. d) (odhalování a stíhání trestné činnosti) a přípustné je i ztotožnění osoby, která není jednoznačně určena (popis znaky) — podmínky § 5b odst. 1 splněny, přímý přístup policie je legální. Vymáhání běžného daňového nedoplatku finančním úřadem nesplňuje žádné z písm. a)–f): nejde o „významný hospodářský/finanční zájem ČR/EU" ve smyslu odst. 1 písm. e) (to míří na systémové/měnové/rozpočtové zájmy, ne na individuální exekuci). Podmínka taxativního účelu pro finanční úřad splněna není.

**5. Řešení.** Policie smí přímý přístup využít (písm. d) — i u neurčené osoby; pravidla o ISZR/ISSS se nepoužijí (odst. 2). Finanční úřad přímý přístup využít nesmí — musí postupovat standardně přes AIS a ISZR/ISSS (§ 5 odst. 5). Procesně: u policie zdokumentovat účel podřaditelný písm. a)–f); zvážit blokaci zpřístupnění záznamů (§ 60). Riziko: extenzivní výklad písm. e) by otevřel přímý přístup plošně — nutný restriktivní výklad.

**6. Varianty.** (a) Šlo-li by o ochranu finančního zájmu EU při rozsáhlém daňovém podvodu (karuselové podvody), mohla by být naplněna písm. e). (b) Při běžném správním řízení bez vazby na účely a)–f) je přímý přístup vyloučen a jakékoli jeho využití by bylo nezákonné.

#### G. Protiargumenty a rizika

- *Protiargument:* „Každý finanční zájem státu spadá pod písm. e)." — Neutralizace: písm. e) míří na významný systémový zájem (měnový, rozpočtový, daňový v makro rovině), nikoli na individuální vymáhání; výjimky se vykládají restriktivně.
- *Protiargument:* „Přímý přístup ruší veškerou ochranu auditní stopy." — Neutralizace: ZZR riziko vyvažuje úpravou § 60 a § 60a; absence záznamu v ISZR neznamená absenci jakékoli kontroly.
- *Slabé místo:* taxativní výčet účelů je formulován široce (zejména písm. e a f); hrozí účelové podřazování běžných úkonů pod bezpečnostní výjimku — slabina v dohledatelnosti zneužití.

#### H. Praktický závěr

§ 5b je úzká výjimka z architektonického zákazu přímého přístupu: jen pro taxativně vyjmenované účely (bezpečnost, obrana, veřejná bezpečnost, trestní řízení, významný hospodářský/finanční zájem, ochrana práv v řízení před soudem) lze přistupovat do AIS přímo, mimo ISZR/ISSS, a to i u osoby neurčené.

**Checklist (advokát / soud / správní orgán / adresát normy):**
- [ ] Spadá účel přístupu pod některé z písm. a)–f) odst. 1 (taxativní)?
- [ ] Je výjimka vykládána restriktivně (zejm. písm. e a f)?
- [ ] Jde-li o neurčenou osobu, je to potřebné pro daný úkol v působnosti orgánu?
- [ ] Byla zvážena ochrana/blokace záznamů podle § 60 a § 60a?
- [ ] Nepoužívá běžný správní orgán přímý přístup tam, kde má jít přes ISZR/ISSS (§ 5 odst. 5)?

**Typicky rozhodné důkazy / podklady:** spisová dokumentace účelu, právní kvalifikace úkonu (trestní/bezpečnostní), evidence přístupu, podklady k blokaci podle § 60.

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

#### F. Kazuistika

**1. Modelová situace.** Občan má podezření, že k jeho údajům někdo neoprávněně nahlížel. Požádá DIA o záznam o využívání svých údajů vedených v agendových informačních systémech. DIA část záznamů odmítne vydat s tím, že jsou starší 2 let, a u jednoho přístupu zjistí podezřelé čerpání bez zjevného účelu. Účastníci: občan (subjekt údajů), DIA (správce ISSS), ÚOOÚ, dotčený orgán/uživatel. Důkazy: žádost občana, logy ISSS, registrace agendy čerpajícího subjektu.

**2. Právní otázka.** V jakém rozsahu a po jakou dobu je DIA povinna vést a vydat subjektu záznam o využívání jeho údajů a jak má reagovat na podezření z neoprávněného přístupu?

**3. Použitelné právo.**
- *Komentované ustanovení:* § 7 odst. 4 (DIA vede záznam o využívání údajů z AIS, uchovává 2 roky; obsah záznamu), odst. 5 (vydání záznamu na žádost osoby, i jako ověřený výstup), odst. 7 (při pochybnosti o neoprávněném využívání DIA neprodleně informuje ÚOOÚ).
- *Související ustanovení téhož zákona:* § 7 odst. 2 písm. h) (vedení záznamů o událostech), odst. 6 (DIA sama nesmí čerpat mimo vlastní agendu), § 14 (záznamy ze ZR), § 60a (přístup ÚOOÚ a dalších k záznamům).
- *Související předpisy:* GDPR čl. 15 (právo na přístup), čl. 12 odst. 5 (bezplatnost); zákon č. 471/2022 Sb., o DIA.
- *Judikatura:* nosný závěr k právu subjektu údajů na informaci o příjemcích a o tom, komu byly údaje zpřístupněny (výklad čl. 15 GDPR — právo znát konkrétní příjemce).

**4. Subsumpce.** DIA vede záznam o využívání údajů z AIS po dobu 2 let (odst. 4) — záznamy starší 2 let oprávněně nevydá, neboť je již neuchovává. Záznamy v rámci 2 let je povinna vydat na žádost (odst. 5), i jako ověřený výstup. U podezřelého čerpání bez doloženého důvodu/účelu (odst. 4 písm. e) vzniká „důvodná pochybnost o neoprávněném využívání" → aktivuje se povinnost odst. 7. Podmínky pro vydání záznamu i pro notifikaci ÚOOÚ jsou splněny.

**5. Řešení.** DIA vydá záznam za poslední 2 roky (bezplatně, i jako ověřený výstup); u staršího období vydání odmítne pro uplynutí retenční doby. Při zjištěné pochybnosti o neoprávněném přístupu informuje neprodleně ÚOOÚ (odst. 7), který provede dozor. Procesně: občan podá žádost; DIA prověří log; podezřelý přístup eskaluje na ÚOOÚ. Riziko: kratší retence (2 roky) může bránit doložení starších zneoprávněných přístupů.

**6. Varianty.** (a) Jde-li o veřejně přístupné údaje, DIA záznam o jejich využívání nevede (odst. 4 in fine) a nevydá jej. (b) Pochází-li sporný přístup z činnosti samotné DIA mimo její registrovanou agendu, jde o porušení odst. 6 a věc řeší ÚOOÚ vůči DIA.

#### G. Protiargumenty a rizika

- *Protiargument:* „DIA jako provozovatel může data využívat libovolně." — Neutralizace: odst. 6 výslovně zakazuje DIA využívat údaje mimo vlastní registrovanou agendu; provozovatel infrastruktury není uživatelem dat.
- *Protiargument:* „Záznamy se vedou trvale, takže lze doložit i staré přístupy." — Neutralizace: odst. 4 stanoví retenci 2 roky; po jejím uplynutí záznam neexistuje a nelze jej vydat.
- *Slabé místo:* hranice „důvodné pochybnosti" o neoprávněném využívání (odst. 7) je vágní; bez jasných kritérií hrozí, že podezřelé přístupy nebudou eskalovány na ÚOOÚ.

#### H. Praktický závěr

§ 7 činí DIA správcem ISZR/ISSS (a navíc ROB a RPP) a ukládá jí vést auditní záznamy o využívání údajů (2 roky), vydávat je subjektu na žádost (i jako ověřený výstup) a notifikovat ÚOOÚ při pochybnosti o neoprávněném využívání. DIA sama nesmí čerpat mimo vlastní agendu.

**Checklist (advokát / soud / správní orgán / adresát normy):**
- [ ] Spadá požadovaný záznam do retenční doby 2 let (odst. 4)?
- [ ] Obsahuje záznam zákonné náležitosti (kód agendy, role, výčet údajů, datum/čas, důvod a účel — odst. 4)?
- [ ] Byl záznam vydán bezplatně, případně jako ověřený výstup (odst. 5)?
- [ ] Vznikla pochybnost o neoprávněném využívání → informována ÚOOÚ (odst. 7)?
- [ ] Nečerpá DIA údaje mimo vlastní registrovanou agendu (odst. 6)?

**Typicky rozhodné důkazy / podklady:** žádost subjektu, logy ISZR/ISSS, registrace agendy čerpajícího subjektu, doklad o účelu přístupu, podání vůči ÚOOÚ.

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

#### F. Kazuistika

**1. Modelová situace.** Ministerstvo jako správce AIS daňové správy zpřístupní jinému úřadu (cizí agenda) prostřednictvím své služby širší okruh údajů, než kolik má cizí úřad ve výčtu zpřístupněných údajů pro svou agendu. Současně při komunikaci s ISZR neuvede u některých dotazů kód agendy. Účastníci: ministerstvo (správce AIS), čerpající úřad, správce RPP (DIA), subjekt údajů. Důkazy: registrace agend obou úřadů, technické logy komunikace AIS–ISZR, přidělený kód agendy.

**2. Právní otázka.** Smí správce AIS zpřístupnit údaje v širším rozsahu, než je čerpajícímu orgánu zpřístupněno pro jeho agendu, a jaké jsou následky komunikace bez kódu agendy?

**3. Použitelné právo.**
- *Komentované ustanovení:* § 8 odst. 3 (správce AIS umožní využití údajů jen v rozsahu zpřístupněném pro výkon agendy daného OVM, resp. v rozsahu oprávnění soukromoprávního uživatele), odst. 4 (povinné používání kódu agendy přiděleného RPP), odst. 5 (dvojí identifikátory — vlastní uvnitř, AIFO/IČO navenek), odst. 6 (mechanismus opravy), odst. 7 (notifikace o změně).
- *Související ustanovení téhož zákona:* § 5 odst. 1 (čerpání jen v rámci výčtu zpřístupněných údajů), § 13 (kód agendy), § 9–11 (AIFO), § 7 odst. 2 písm. k) (centrální notifikační služba).
- *Související předpisy:* GDPR čl. 5 odst. 1 písm. b), c) (účelové omezení, minimalizace), čl. 32 (zabezpečení).
- *Judikatura:* obecná zásada vázanosti zpracování osobních údajů účelem a rozsahem; zpřístupnění nad rámec oprávnění je nezákonné zpracování (konstantní výklad k GDPR).

**4. Subsumpce.** Podle odst. 3 správce AIS zpřístupní údaje jen v rozsahu, v jakém jsou čerpajícímu OVM zpřístupněny pro jeho agendu. Zpřístupnění širšího okruhu překračuje toto oprávnění — podmínka odst. 3 splněna není. Komunikace bez kódu agendy porušuje odst. 4; ISZR/ISSS má takový dotaz odmítnout, takže přístup buď neproběhne, nebo je vadný. Obě jednání jsou v rozporu s § 8.

**5. Řešení.** Správce AIS musí omezit zpřístupnění na rozsah zpřístupněný čerpajícímu úřadu pro jeho agendu (odst. 3) a každý dotaz označit kódem agendy (odst. 4), navenek používat AIFO/IČO (odst. 5). Širší zpřístupnění je nezákonné zpracování; věc spadá do dozoru ÚOOÚ. Procesně: revize konfigurace zpřístupnění proti výčtu v RPP, technické vynucení kódu agendy. Riziko: bez kontroly rozsahu hrozí plošný únik nad rámec oprávnění.

**6. Varianty.** (a) Pokud by čerpajícím byl soukromoprávní uživatel, rozsah by se řídil jeho oprávněním podle zákona/souhlasu (odst. 3 druhá část). (b) Pokud by AIS uvnitř používal navenek vlastní interní ID místo AIFO (porušení odst. 5), umožnil by nepřípustné propojování údajů napříč agendami mimo ORG.

#### G. Protiargumenty a rizika

- *Protiargument:* „Správce AIS je pánem svých dat a může je zpřístupnit, komu uzná." — Neutralizace: odst. 3 váže zpřístupnění na rozsah zpřístupněný čerpajícímu pro jeho agendu; nad rámec oprávnění jde o nezákonné zpracování.
- *Protiargument:* „Kód agendy je formalita." — Neutralizace: odst. 4 jej činí podmínkou komunikace; bez něj ISZR/ISSS dotaz odmítne a chybí auditní přiřaditelnost.
- *Slabé místo:* dvojí identifikátor (odst. 5) je technicky náročný; chyba v mapování vlastní ID ↔ AIFO může vést buď k záměně osob, nebo k obcházení ochrany proti profilování.

#### H. Praktický závěr

§ 8 ukládá správci AIS sedm povinností: napojení na ISZR (zápis i čtení), propustnost na jiné AIS přes ISZR/ISSS, zpřístupnění údajů jen v rozsahu oprávnění, povinné používání kódu agendy, dvojí identifikátor (vlastní uvnitř, AIFO/IČO navenek), mechanismus opravy a notifikaci o změnách.

**Checklist (advokát / soud / správní orgán / adresát normy):**
- [ ] Zpřístupňuje správce AIS údaje jen v rozsahu oprávnění čerpajícího pro jeho agendu (odst. 3)?
- [ ] Je u každé komunikace s ISZR/ISSS použit kód agendy přidělený RPP (odst. 4)?
- [ ] Používá AIS navenek AIFO/IČO, nikoli vlastní interní ID (odst. 5)?
- [ ] Má AIS zaveden mechanismus opravy nesprávných údajů (odst. 6)?
- [ ] Zajišťuje správce vyrozumění o změně údajů (odst. 7, § 7 odst. 2 písm. k)?

**Typicky rozhodné důkazy / podklady:** registrace agend a výčty zpřístupněných údajů v RPP, technické logy komunikace AIS–ISZR/ISSS, přidělený kód agendy, mapování identifikátorů.

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

#### F. Kazuistika

**1. Modelová situace.** Banka provozující SPSVU pro AML kontrolu chce při komunikaci s ISZR identifikovat klienty svým interním číslem klienta (CIF), aby si zjednodušila párování s vnitřními systémy, a kód agendy uvádět jen občas. Účastníci: banka (soukromoprávní uživatel), DIA (ISZR), klient. Důkazy: konfigurace SPSVU, logy komunikace, přidělený kód agendy a identifikátor soukromoprávního uživatele.

**2. Právní otázka.** Jaké identifikátory musí soukromoprávní uživatel používat při komunikaci v referenčním rozhraní a smí místo nich použít vlastní interní identifikátor?

**3. Použitelné právo.**
- *Komentované ustanovení:* § 8a odst. 3 (povinné používání kódu agendy), odst. 4 (vlastní identifikátory uvnitř, AIFO/IČO navenek vůči ISZR/ISSS).
- *Související ustanovení téhož zákona:* § 9 odst. 3 (komunikace ZR/AIS/SPSVU jen přes kód agendy + AIFO), § 9 odst. 1 (AIFO odvozen i z identifikátoru soukromoprávního uživatele), § 13 (kód agendy), § 5a (titul přístupu).
- *Související předpisy:* zákon č. 253/2008 Sb. (AML); GDPR čl. 5 (minimalizace, účelové omezení), čl. 25 (záměrná ochrana — privacy by design).
- *Judikatura:* nosný požadavek minimalizace propojitelnosti identifikátorů jako prvek ochrany soukromí; zákaz jednotného sémantického identifikátoru (kritika rodného čísla ÚS).

**4. Subsumpce.** Navenek vůči ISZR musí SPSVU používat AIFO (pro FO) a IČO (pro PO) a kód agendy (odst. 3, 4 ve spojení s § 9 odst. 3). Interní CIF je „vlastní identifikátor", který smí být použit jen uvnitř SPSVU. Jeho použití navenek a vynechávání kódu agendy podmínky § 8a odst. 3, 4 nesplňují; dotaz bez kódu agendy ISZR odmítne.

**5. Řešení.** Banka uvnitř SPSVU smí používat CIF, ale navenek musí komunikovat výhradně AIFO/IČO + kód agendy. Mapování CIF ↔ AIFO je interní věcí banky. Použití CIF navenek by narušilo architekturu ORG a umožnilo nepřípustné propojování. Procesně: úprava SPSVU tak, aby každý dotaz nesl kód agendy a navenek jen AIFO/IČO. Riziko: bez toho ISZR komunikaci odmítne a banka nesplní AML povinnost.

**6. Varianty.** (a) Téže osobě banka pro jinou agendu obdrží jiné AIFO — identifikátory nejsou převoditelné mimo ÚOOÚ (§ 11). (b) Pro různé SPSVU téže soukromoprávní agendy může mít osoba různá AIFO (§ 10 odst. 1) — banka to musí zohlednit v párování.

#### G. Protiargumenty a rizika

- *Protiargument:* „AIFO je jen technické číslo, lze ho nahradit vlastním ID." — Neutralizace: § 8a odst. 4 a § 9 odst. 3 stanoví AIFO/IČO + kód agendy jako jediný přípustný způsob vnější komunikace; vlastní ID je přípustné jen uvnitř.
- *Protiargument:* „Z AIFO si lze dohledat totožnost, takže je rizikové." — Neutralizace: § 9 odst. 1, 2 — z AIFO nelze odvodit ZIFO ani osobní údaje; jde o bezsémantický identifikátor, bezpečnější než rodné číslo.
- *Slabé místo:* správné mapování interních ID na AIFO je technicky náročné; chyba vede buď k záměně osob, nebo k obejití ochrany proti profilování.

#### H. Praktický závěr

§ 9 zavádí dvouvrstvou identifikaci fyzických osob: neveřejné ZIFO (jen ÚOOÚ) a z něj jednosměrně odvozené, agendově vázané AIFO (neveřejné, bez sémantiky). Komunikace v referenčním rozhraní probíhá výhradně přes kód agendy + AIFO; z AIFO nelze odvodit ZIFO ani osobní údaje.

**Checklist (advokát / soud / správní orgán / adresát normy):**
- [ ] Probíhá vnější komunikace jen přes kód agendy + AIFO (resp. IČO u PO)?
- [ ] Není navenek používán vlastní/interní identifikátor (přípustný jen uvnitř)?
- [ ] Je respektováno, že z AIFO nelze odvodit ZIFO ani osobní údaje (odst. 1, 2)?
- [ ] Je pro propojení napříč agendami využit výhradně převod přes ÚOOÚ (§ 11)?

**Typicky rozhodné důkazy / podklady:** konfigurace AIS/SPSVU, logy komunikace s ISZR, přidělený kód agendy a identifikátor soukromoprávního uživatele, mapování identifikátorů.

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

#### F. Kazuistika

**1. Modelová situace.** IT firma získá v rámci úniku dat „dumpy" tří různých agendových informačních systémů (evidence obyvatel, zdravotní pojištění, daně) a pokusí se sestavit kompletní profil konkrétní osoby propojením podle identifikátorů. Zjistí, že tatáž osoba má v každém systému jiný identifikátor a nelze je spárovat. Účastníci: IT firma (útočník), tři správci AIS, ÚOOÚ. Důkazy: struktura uniklých dat, identifikátory v jednotlivých AIS.

**2. Právní otázka.** Lze osobní údaje téže osoby propojit napříč agendami na základě agendových identifikátorů bez součinnosti ÚOOÚ?

**3. Použitelné právo.**
- *Komentované ustanovení:* § 9 odst. 1 (AIFO odvozen ze ZIFO + kódu agendy, vázaný na agendu; z AIFO nelze odvodit ZIFO ani osobní údaje), odst. 2 (ze ZIFO nelze dovodit osobní údaje), odst. 3 (komunikace jen přes kód agendy + AIFO).
- *Související ustanovení téhož zákona:* § 11 (převod AIFO mezi agendami výhradně ÚOOÚ na zákonný požadavek), § 10 (jeden člověk – jedna agenda – jeden AIFO), § 8 odst. 5 a § 8a odst. 4 (dvojí identifikátor).
- *Související předpisy:* GDPR čl. 5, čl. 25, čl. 32 (zabezpečení); zákon č. 110/2019 Sb. (sankce za neoprávněné zpracování).
- *Judikatura:* nosný závěr ÚS o protiústavnosti univerzálního identifikátoru (rodného čísla) umožňujícího plošné propojování osobních údajů — architektura AIFO je přímou reakcí na tuto kritiku.

**4. Subsumpce.** AIFO je v každé agendě jiné a z něj nelze odvodit ZIFO (odst. 1) — bez ZIFO a bez převodu přes ÚOOÚ (§ 11) jsou agendová ID vzájemně nepropojitelná. Podmínka odvoditelnosti, na níž útok stojí, není splněna; propojení napříč agendami je technicky vyloučeno.

**5. Řešení.** Útok na propojení selže — to je přesně cíl architektury § 9: agendové identifikátory technicky znemožňují masové propojení. Legitimní propojení je možné jen přes ÚOOÚ na zákonný požadavek (§ 11) s auditní stopou. Procesně: únik dat se řeší jako bezpečnostní incident (GDPR čl. 33–34), nikoli jako možnost legálního propojení. Riziko zůstává jen u dat získaných pro jednu agendu — uvnitř ní jsou údaje propojené.

**6. Varianty.** (a) Kdyby útočník získal i ZIFO (kompromitace ÚOOÚ), stále z něj nemůže odvodit osobní údaje (odst. 2), získá jen prostředek k odvození AIFO. (b) Pro legitimní agendovou potřebu propojit ROB a zdravotní AIS by orgán požádal ÚOOÚ o převod AIFO (§ 11), což je jediná zákonná cesta.

#### G. Protiargumenty a rizika

- *Protiargument:* „Stačí dost dat a osobu lze deanonymizovat i bez převodu." — Neutralizace: deanonymizace přes kvazi-identifikátory (jméno, datum narození) je jiná rovina než propojení přes AIFO; ZZR cílí na zákaz systémového identifikátoru, plný profil přes nepřímé znaky neřeší, ale výrazně ztěžuje.
- *Protiargument:* „Z AIFO lze zpětně odvodit ZIFO/údaje." — Neutralizace: odst. 1 a 2 výslovně vylučují odvoditelnost; jednosměrnost odvození je vlastností konstrukce.
- *Slabé místo:* ochrana závisí na faktické jednosměrnosti odvozovací funkce a na bezpečnosti ÚOOÚ; technické selhání by oslabilo celý systém.

#### H. Praktický závěr

§ 9 představuje bezpečnostní jádro zákona: agendové identifikátory jsou vázané na jednu agendu, bez sémantiky a vzájemně nepropojitelné; propojení napříč agendami je možné jen přes ÚOOÚ. Architektura cílí proti masovému profilování a je reakcí na protiústavnost rodného čísla.

**Checklist (advokát / soud / správní orgán / adresát normy):**
- [ ] Je propojení údajů napříč agendami prováděno výhradně přes ÚOOÚ (§ 11)?
- [ ] Není mimo agendu používán identifikátor umožňující propojení (jen kód agendy + AIFO)?
- [ ] Je respektována neodvoditelnost ZIFO a osobních údajů z AIFO (odst. 1, 2)?
- [ ] Při úniku dat — řešeno jako bezpečnostní incident, nikoli jako legální propojení?

**Typicky rozhodné důkazy / podklady:** struktura identifikátorů v jednotlivých AIS, logy převodů přes ÚOOÚ, dokumentace odvozovací funkce, incidentní dokumentace.

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

#### F. Kazuistika

**1. Modelová situace.** Při migraci dat v agendě zdravotního pojištění se zjistí, že dvěma různým pojištěncům (manželům se stejným příjmením) byl omylem přiřazen tentýž agendový identifikátor fyzické osoby; rozhodnutí a platby se začaly mísit. Správce AIS to ohlásí. Účastníci: dva pojištěnci, správce AIS zdravotní pojišťovny, správce ROB (DIA). Důkazy: záznamy o přidělení AIFO, migrace, mylně spárované úkony.

**2. Právní otázka.** Jak se postupuje, byl-li týž AIFO v jedné agendě přidělen dvěma osobám, a kdo kolizi řeší?

**3. Použitelné právo.**
- *Komentované ustanovení:* § 10 odst. 2 (jeden AIFO z jednoho ZIFO nesmí být přidělen více osobám), odst. 4 (kolize → oběma záznamům nový AIFO), odst. 1 (v agendě jeden AIFO na osobu), odst. 3 (neměnnost AIFO, ledaže zákon stanoví jinak), odst. 6, 7 (eskalační mechanismus opravy: zjistitel → správce AIS/SPSVU → správce ROB).
- *Související ustanovení téhož zákona:* § 9 (povaha AIFO), § 11 (ÚOOÚ jako tvůrce AIFO a převodník), § 23 (nové pořízení AIFO).
- *Související předpisy:* GDPR čl. 5 odst. 1 písm. d) (přesnost údajů), čl. 16 (oprava).
- *Judikatura:* obecná zásada povinnosti správce zajistit přesnost a integritu identifikace; chybné spárování identit zakládá vadu zpracování.

**4. Subsumpce.** Nastala situace odst. 4 — týž AIFO přidělen dvěma osobám. Pravidlo odst. 2 (jeden AIFO ≠ více osob) bylo porušeno. Aktivuje se odst. 4: oběma záznamům se přidělí nový AIFO. Současně běží eskalace odst. 6–7: zjistitel ohlásí správci AIS; nelze-li opravit v AIS, věc jde na správce ROB. Podmínky pro přidělení nových AIFO jsou splněny.

**5. Řešení.** Správce AIS se pokusí nedostatek odstranit ve svém systému (odst. 6); nelze-li, ohlásí správci ROB (odst. 7), který ve spolupráci řeší kolizi, a nelze-li jinak, postupuje podle odst. 4, 5 (nové AIFO oběma). Neměnnost AIFO (odst. 3) zde ustupuje výjimce „stanoví-li zákon jinak". Procesně: zablokovat mylně spárované úkony, opravit přiřazení, přidělit nová AIFO, narovnat platby. Riziko: než dojde k opravě, hrozí pokračující mísení úkonů a škody.

**6. Varianty.** (a) Opačná vada — jedné osobě přiděleny dva AIFO v jedné agendě (odst. 5) — se řeší konsolidací obdobně podle odst. 4. (b) Lze-li nedostatek odstranit již v AIS (odst. 6), není třeba eskalace na ROB ani nové AIFO.

#### G. Protiargumenty a rizika

- *Protiargument:* „AIFO je neměnné, takže kolizi nelze opravit změnou identifikátoru." — Neutralizace: odst. 3 připouští výjimku „stanoví-li tento zákon jinak"; odst. 4 a 5 takovou výjimku zakládají právě pro kolizní situace.
- *Protiargument:* „Opravu provede sám zjistitel chyby." — Neutralizace: zjistitel jen ohlašuje (odst. 6); opravu provádí správce AIS/SPSVU, eskalačně správce ROB — centralizace zajišťuje integritu.
- *Slabé místo:* dokud kolize trvá, mísí se úkony dvou osob; mechanismus je reaktivní (po zjištění), nikoli preventivní — slabina v detekci.

#### H. Praktický závěr

§ 10 zaručuje integritu přidělování AIFO podle pravidla „jeden člověk – jedna agenda – jeden AIFO". Kolize (týž AIFO dvěma osobám) i multiplicita (dvě AIFO jedné osobě) se řeší přidělením nových AIFO; opravy probíhají eskalačně přes správce AIS až ke správci ROB.

**Checklist (advokát / soud / správní orgán / adresát normy):**
- [ ] Jde o kolizi (odst. 4) nebo multiplicitu (odst. 5) AIFO?
- [ ] Byla chyba ohlášena správci AIS/SPSVU (odst. 6) a případně eskalována na správce ROB (odst. 7)?
- [ ] Lze nedostatek odstranit v AIS, nebo je nutné nové AIFO (odst. 4, 5)?
- [ ] Byly zablokovány a narovnány úkony provedené pod chybným AIFO?

**Typicky rozhodné důkazy / podklady:** záznamy o přidělení AIFO, migrační logy, doklady o mylně spárovaných úkonech, komunikace se správcem ROB.

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

#### F. Kazuistika

**1. Modelová situace.** Orgán sociálního zabezpečení potřebuje pro řízení o dávce propojit údaje o téže osobě vedené pod různými AIFO ve dvou agendách (evidence obyvatel a důchodové pojištění). Sám si je propojit nedokáže. Žádá proto o převod AIFO. Souběžně soukromá detektivní kancelář žádá ÚOOÚ o převod AIFO konkrétní osoby, aby pro klienta zjistila její údaje napříč agendami. Účastníci: orgán sociálního zabezpečení, detektivní kancelář, ÚOOÚ. Důkazy: registrace agendy a její oprávnění, právní podklad žádosti o převod.

**2. Právní otázka.** Za jakých podmínek a komu ÚOOÚ provede převod AIFO mezi agendami a co je „zákonný požadavek"?

**3. Použitelné právo.**
- *Komentované ustanovení:* § 11 odst. 1 písm. a) (ÚOOÚ vytváří ZIFO a AIFO a vede jejich seznamy), písm. b) (převod AIFO mezi agendami na základě zákonného požadavku), odst. 2 (ZIFO užívá výhradně ÚOOÚ a jen k tvorbě/převodu AIFO).
- *Související ustanovení téhož zákona:* § 9 (povaha identifikátorů), § 10 (pravidla AIFO), § 5 odst. 1 (vázanost čerpání na registrovanou agendu a výčet údajů).
- *Související předpisy:* zákon č. 110/2019 Sb. a postavení ÚOOÚ jako nezávislého dozorového úřadu; GDPR čl. 6 (zákonnost).
- *Judikatura:* nosný požadavek, že každý zásah do informačního sebeurčení musí mít zákonný podklad a sledovat legitimní účel; svěření převodníku nezávislému dozorovému orgánu posiluje záruky.

**4. Subsumpce.** Orgán sociálního zabezpečení má agendovou potřebu propojení v rámci registrované agendy — to je „zákonný požadavek" podle písm. b); převod je přípustný a probíhá s auditní stopou. Detektivní kancelář nemá registrovanou agendu ani zákonný titul; její žádost není „zákonným požadavkem" — podmínka písm. b) splněna není a převod je nepřípustný.

**5. Řešení.** ÚOOÚ provede převod pro orgán sociálního zabezpečení (zákonný požadavek z registrace agendy), nikoli pro detektivní kancelář (chybí zákonný titul). ZIFO přitom neopouští ÚOOÚ (odst. 2). Procesně: orgán doloží agendovou potřebu/oprávnění; ÚOOÚ převod zaznamená (audit). Riziko: extenzivní výklad „zákonného požadavku" by mohl otevřít převody bez dostatečného titulu — nutný restriktivní přístup.

**6. Varianty.** (a) Soudní/policejní požadavek v trestním řízení je rovněž „zákonným požadavkem" → převod přípustný. (b) Žádost orgánu o převod nad rámec jeho registrované agendy (např. pro účel, který nemá zaregistrován) by zákonným požadavkem nebyla a ÚOOÚ by ji odmítl.

#### G. Protiargumenty a rizika

- *Protiargument:* „Převodník by lépe provozovalo MV/DIA, které mají eGovernment v gesci." — Neutralizace: svěření ÚOOÚ je záměrné — dozorový orgán bez vlastního agendového zájmu eliminuje konflikt zájmů a působí jako operační strážce ochrany dat.
- *Protiargument:* „Zákonný požadavek je každá žádost orgánu." — Neutralizace: musí jít o požadavek mající oporu v zákoně/registrované agendě; pouhá žádost bez titulu nestačí.
- *Slabé místo:* „zákonný požadavek" není v § 11 definován výčtem; jeho posouzení leží na ÚOOÚ a může být sporné v hraničních případech.

#### H. Praktický závěr

§ 11 svěřuje ÚOOÚ provoz převodníku identifikátorů (ORG): jako jediný tvoří ZIFO i AIFO a jako jediný převádí AIFO mezi agendami, a to jen na zákonný požadavek. ZIFO neopouští ÚOOÚ. Jde o institucionální brzdu profilování.

**Checklist (advokát / soud / správní orgán / adresát normy):**
- [ ] Má žadatel o převod zákonný titul / registrovanou agendu (zákonný požadavek)?
- [ ] Je převod prováděn výhradně ÚOOÚ a zaznamenán (auditní stopa)?
- [ ] Zůstává ZIFO výhradně u ÚOOÚ a jen k tvorbě/převodu AIFO (odst. 2)?
- [ ] Není převod žádán nad rámec registrované agendy žadatele?

**Typicky rozhodné důkazy / podklady:** registrace agendy a její oprávnění v RPP, právní podklad žádosti o převod (soudní/policejní akt, agendová potřeba), log převodu u ÚOOÚ.

---

### § 12 — Identifikátor subjektů vedených v registru osob

> **§ 12**
>
> *Identifikátorem subjektu vedeného v registru osob je identifikační číslo osoby.*

**Výklad:**

§ 12 stanoví, že identifikátorem subjektu v ROS je **identifikační číslo osoby (IČO)** — osmimístné číslo, které se přiděluje právnickým osobám, OSVČ, organizačním složkám státu, OVM a dalším subjektům podle § 25.

**Judikatura (z místních zdrojů):**

- *NSS* [10 A 32/2017 - 44](https://vyhledavac.nssoud.cz/DokumentOriginal/Text/437932) — 31. 5. 2019
  > „z dikce § 18 odst. 2 s. ř., na který odkazuje § 68 odst. 2 s. ř., sice vyplývá, že údaji, umožňujícími identifikaci fyzické osoby se rozumějí jméno, příjmení a datum narození a místo trvalého pobytu, nicméně takovým údajem může být popřípadě jiný údaj podle zvláštního zákona. Takovým případem zvláštního zákona je zákon č. 111/2009 Sb. o základních registrech, který uvádí, že identifikátorem subjektu vedeného v registru osob je identifikační číslo osoby (§ 12 zákona č. 111/2009 Sb.)"

#### IČO — kontrast s AIFO

Zásadní rozdíl proti identifikátorům fyzických osob:

| | Fyzické osoby | Právnické osoby a OSVČ |
|---|---|---|
| Identifikátor | AIFO (různý v každé agendě) | IČO (jediné, sdílené napříč agendami) |
| Veřejnost | Neveřejný | Veřejné |
| Ochrana profilování | Ano (přes ORG) | Žádná |

Proč rozdíl? Právnické osoby a podnikatelé **nemají ústavní právo na soukromí** v takovém rozsahu jako fyzické osoby. Naopak veřejnost obchodního styku vyžaduje **jednoznačnou a veřejnou identifikaci** podnikatelských subjektů. IČO proto plní opačnou funkci — má usnadnit propojování údajů o subjektu napříč evidencemi.

OSVČ jsou v této struktuře zvláštním případem — jako fyzické osoby mají AIFO (pro osobní záležitosti), jako podnikatelé mají IČO (pro podnikatelské záležitosti). Tato dvojakost je zachycena v § 26 odst. 2 písm. b) — pro OSVČ se vede odkaz na ROB i IČO v ROS.

#### F. Kazuistika

**1. Modelová situace.** Podnikatel vede spor o totožnost dvou obchodních partnerů, kteří mají podobné názvy. Chce mít jistotu, kterým subjektem jedná, a navrhuje identifikovat partnera v evidenci podle jména jednatele a adresy. Protistrana namítá, že jediným spolehlivým identifikátorem je IČO. Účastníci: podnikatel, dva obchodní partneři (PO/OSVČ), rejstříkový/registrační orgán. Důkazy: výpisy z ROS/veřejných rejstříků, IČO subjektů.

**2. Právní otázka.** Co je identifikátorem subjektu vedeného v registru osob a lze jej spolehlivě nahradit jinými údaji (jméno, adresa)?

**3. Použitelné právo.**
- *Komentované ustanovení:* § 12 — identifikátorem subjektu v ROS je identifikační číslo osoby (IČO).
- *Související ustanovení téhož zákona:* § 26 odst. 2 písm. b) (pro OSVČ odkaz na ROB i IČO v ROS), § 25 (přidělování IČO), § 9 (kontrast s neveřejným AIFO u FO).
- *Související předpisy:* zákon č. 304/2013 Sb. (veřejné rejstříky) — IČO jako veřejný identifikátor; zákon č. 455/1991 Sb. (živnostenský zákon) pro OSVČ.
- *Judikatura:* obecná zásada určitosti označení účastníka právního vztahu; IČO jako jednoznačný a veřejný identifikátor podnikatele.

**4. Subsumpce.** Identifikátorem subjektu v ROS je IČO (§ 12) — veřejné a jednoznačné. Jméno jednatele a adresa nejsou identifikátorem subjektu a mohou být u podobných firem shodné či zaměnitelné; spolehlivá identifikace přes ně podmínku jednoznačnosti nesplňuje. Pro určení subjektu je rozhodné IČO.

**5. Řešení.** Partnera nutno identifikovat IČO (§ 12), nikoli jménem/adresou. Na rozdíl od FO (neveřejné AIFO) je IČO veřejné a sdílené napříč agendami — slouží naopak k usnadnění propojení údajů o podnikateli. Procesně: ve smlouvách a podáních uvádět IČO; ověřit subjekt ve veřejném rejstříku/ROS. Riziko záměny při spoléhání na jméno odpadá použitím IČO.

**6. Varianty.** (a) Jde-li o OSVČ, má jako FO neveřejné AIFO (osobní záležitosti) a jako podnikatel IČO (§ 26 odst. 2 písm. b) — pro podnikatelský styk je rozhodné IČO. (b) U zahraničního subjektu bez IČO je nutné identifikovat jej jiným úředním identifikátorem dle příslušné evidence.

#### G. Protiargumenty a rizika

- *Protiargument:* „Identifikace podle názvu a sídla je dostatečná." — Neutralizace: § 12 určuje IČO jako identifikátor; názvy a sídla mohou být zaměnitelné, IČO je jednoznačné a veřejné.
- *Protiargument:* „IČO má stejnou ochranu jako AIFO." — Neutralizace: IČO je naopak veřejné a sdílené napříč agendami; právnické osoby nepožívají ochrany soukromí v rozsahu jako FO.
- *Slabé místo:* u OSVČ se prolíná osobní (AIFO) a podnikatelská (IČO) identita; v hraničních věcech je nutné určit, ve které roli osoba vystupuje.

#### H. Praktický závěr

§ 12 určuje IČO jako identifikátor subjektu v registru osob. Na rozdíl od neveřejného, agendově vázaného AIFO u fyzických osob je IČO veřejné a jediné napříč agendami — jeho funkcí je usnadnit, nikoli ztížit, propojování údajů o podnikatelských subjektech.

**Checklist (advokát / soud / správní orgán / adresát normy):**
- [ ] Je subjekt v ROS identifikován IČO (nikoli jen názvem/adresou)?
- [ ] Jde o OSVČ, kde se liší osobní (AIFO) a podnikatelská (IČO) identita?
- [ ] Je IČO ověřeno ve veřejném rejstříku / ROS?

**Typicky rozhodné důkazy / podklady:** výpis z ROS / veřejného rejstříku, IČO subjektu, doklad o přidělení IČO (§ 25).

---

### § 13 — Kód agendy

> **§ 13**
>
> *Kód agendy je veřejným identifikátorem, který je jednoznačně přiřazen záznamu o agendě v číselníku agend v registru práv a povinností.*

**Výklad:**

**Kód agendy** je veřejný identifikátor agendy v RPP. Číselník agend vede Agentura (DIA) a je veřejně přístupný — každý si může ověřit, jaké agendy jsou v ČR registrovány a kdo je vykonává.

Kód agendy je **klíčovým prvkem každé komunikace v referenčním rozhraní** (§ 9 odst. 3 písm. a)) — bez něj je požadavek na údaje z ZR nepřípustný.

> **Praktický význam:** Kód agendy umožňuje detailní auditní trail. Když DIA loguje přístup k ROB, vždy je u záznamu uveden kód agendy. Lze tak zpětně rekonstruovat, kdo k údaji přistoupil a v jaké agendě.

#### F. Kazuistika

**1. Modelová situace.** Úřad provozující AIS odešle do ISZR dotaz na referenční údaje občana, aniž v dotazu uvede kód agendy (chyba konfigurace). ISZR dotaz odmítne. Občan později reklamuje, že u záznamu o přístupu k jeho údajům není dohledatelné, v jaké agendě k němu mělo dojít. Účastníci: úřad (správce AIS), DIA (správce ISZR), občan. Důkazy: log odmítnutého dotazu, číselník agend v RPP, přidělený kód agendy.

**2. Právní otázka.** Jakou roli hraje kód agendy v komunikaci s referenčním rozhraním a jaké jsou důsledky jeho neuvedení?

**3. Použitelné právo.**
- *Komentované ustanovení:* § 13 — kód agendy je veřejný identifikátor jednoznačně přiřazený záznamu o agendě v číselníku agend v RPP.
- *Související ustanovení téhož zákona:* § 9 odst. 3 písm. a) (kód agendy jako povinný identifikátor komunikace), § 8 odst. 4 a § 8a odst. 3 (povinnost používat kód agendy), § 51 odst. 6 (registrace agendy v RPP).
- *Související předpisy:* GDPR čl. 5 odst. 2 (odpovědnost a doložitelnost — accountability).
- *Judikatura:* obecný požadavek auditní dohledatelnosti zpracování osobních údajů jako podmínky kontrolovatelnosti.

**4. Subsumpce.** Kód agendy je povinným identifikátorem komunikace (§ 9 odst. 3 písm. a) ve spojení s § 13). Dotaz bez kódu agendy nesplňuje podmínku § 8 odst. 4 / § 9 odst. 3 — ISZR jej oprávněně odmítne. Bez kódu agendy by chyběla auditní přiřaditelnost přístupu k agendě.

**5. Řešení.** Úřad musí opravit konfiguraci AIS tak, aby každý dotaz nesl přidělený kód agendy (veřejně dohledatelný v číselníku agend v RPP). Odmítnutí dotazu je správné; chrání auditní stopu. Procesně: zjistit kód agendy v RPP, doplnit jej do volání služby. Riziko: bez kódu agendy úřad údaje vůbec nezíská a porušuje pravidla komunikace.

**6. Varianty.** (a) Uvedl-li by úřad cizí kód agendy (jiné, než pro kterou je registrován), šlo by o neoprávněné využití v rozporu s § 5 odst. 1. (b) U veřejně přístupných údajů je auditní režim mírnější, ale kód agendy zůstává nástrojem identifikace agendy.

#### G. Protiargumenty a rizika

- *Protiargument:* „Kód agendy je interní technikálie bez právního významu." — Neutralizace: § 9 odst. 3 jej činí povinným prvkem komunikace; bez něj je dotaz nepřípustný a chybí auditní přiřaditelnost.
- *Protiargument:* „Číselník agend je neveřejný." — Neutralizace: § 13 výslovně stanoví, že kód agendy je veřejný identifikátor — každý si může ověřit registrované agendy a jejich vykonavatele.
- *Slabé místo:* správnost přiřazení kódu agendy závisí na konfiguraci AIS; chyba vede k odmítnutí dotazů nebo k riziku použití nesprávné agendy.

#### H. Praktický závěr

§ 13 definuje kód agendy jako veřejný identifikátor agendy v RPP. Je povinným prvkem každé komunikace v referenčním rozhraní a základem auditní stopy — bez něj je dotaz na údaje ze ZR nepřípustný.

**Checklist (advokát / soud / správní orgán / adresát normy):**
- [ ] Nese každý dotaz do ISZR/ISSS přidělený kód agendy (§ 9 odst. 3 písm. a)?
- [ ] Odpovídá použitý kód agendy agendě, pro kterou je subjekt registrován (§ 5 odst. 1)?
- [ ] Je kód ověřitelný ve veřejném číselníku agend v RPP?

**Typicky rozhodné důkazy / podklady:** číselník agend v RPP, přidělený kód agendy, logy komunikace s ISZR/ISSS.

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

#### F. Kazuistika

**1. Modelová situace.** Občanka zjistí, že v ROB je u ní vedena nesprávná adresa místa pobytu (důsledek chybného přepisu při změně bydliště). Hrozí, že jí kvůli tomu nebudou doručovány úřední písemnosti. Chce (i) zjistit, kdo k jejím údajům přistupoval, (ii) bezplatně dosáhnout opravy. Editor adresy nereaguje. Účastníci: občanka (subjekt údajů), editor (obecní úřad obce s rozšířenou působností), správce ROB (DIA), kontaktní místo veřejné správy (CzechPOINT). Důkazy: výpis z ROB, doklad o skutečném pobytu, žádost o opravu, datum jejího podání.

**2. Právní otázka.** Jaká práva má osoba vůči svým údajům v ZR — zejména na transparentnost přístupů a na bezplatnou opravu — a v jaké lhůtě je editor povinen opravu provést?

**3. Použitelné právo.**
- *Komentované ustanovení:* § 14 odst. 3 (záznam o využívání jen subjektu údajů), odst. 4 (bezplatné obstarání záznamu, i jako ověřený výstup, do datové schránky), odst. 5 (proaktivní zaslání výpisu při změně údaje do datové schránky), odst. 6 (bezplatná reklamace u editora, i přes CzechPOINT; editor postupuje podle § 4 odst. 3).
- *Související ustanovení téhož zákona:* § 4 odst. 3 (lhůta 3 prac. dnů na zápis/změnu), odst. 4 (označení údaje jako nesprávného), § 5 odst. 4 (notifikace editora), § 58 (poskytování údajů).
- *Související předpisy:* GDPR čl. 15 (právo na přístup), čl. 16 (právo na opravu), čl. 12 odst. 5 (bezplatnost); nařízení EU 2016/1191 (vícejazyčný formulář).
- *Judikatura:* nosný závěr k bezodkladné povinnosti správce opravit nepřesný osobní údaj (výklad čl. 16 GDPR) a k právu subjektu znát příjemce údajů (čl. 15).

**4. Subsumpce.** Občanka je „osobou, o které jsou údaje vedeny" (odst. 3) → má právo na záznam o využívání svých údajů, bezplatně a i jako ověřený výstup (odst. 4). Nesoulad adresy se skutečností zakládá právo na bezplatnou reklamaci (odst. 6); žádost lze podat přímo u editora nebo přes CzechPOINT, který ji editorovi předá. Editor pak postupuje podle § 4 odst. 3 — lhůta 3 pracovních dnů. Podmínky pro obě práva jsou splněny.

**5. Řešení.** Občanka podá bezplatnou žádost o opravu (i přes CzechPOINT) a obstará si bezplatně záznam o využívání údajů. Editor je povinen opravit do 3 pracovních dnů ode dne, kdy se o správné skutečnosti dozví (§ 4 odst. 3); do nápravy lze údaj označit jako nesprávný (§ 4 odst. 4) s informativní povahou. Při nečinnosti editora se občanka brání stížností/opatřením proti nečinnosti. Procesně: doložit skutečný pobyt; CzechPOINT předá žádost editorovi; kontrolovat dodržení lhůty. Riziko nedoručení písemností trvá do opravy.

**6. Varianty.** (a) Má-li občanka zřízenou a zpřístupněnou datovou schránku, dostává při každé změně referenčního údaje proaktivně výpis (odst. 5) a může okamžitě reagovat. (b) Žádá-li o záznam o přístupech jiná osoba než subjekt, vydá se jen na základě zvláštního zákona (odst. 3) — běžně se odepře.

#### G. Protiargumenty a rizika

- *Protiargument:* „Lhůta na opravu je obecná podle GDPR (měsíc)." — Neutralizace: § 14 odst. 6 odkazuje na § 4 odst. 3 — zvláštní, kratší lhůta 3 pracovních dnů má přednost před obecnou měsíční lhůtou GDPR.
- *Protiargument:* „Záznam o přístupech či výpis lze zpoplatnit." — Neutralizace: odst. 4 stanoví bezplatnost (i ověřeného výstupu a zaslání do datové schránky), v souladu s čl. 12 odst. 5 GDPR.
- *Slabé místo:* lhůta 3 dnů běží ode dne, kdy se editor o skutečnosti „dozví"; sporný může být okamžik doložení skutečného stavu — bez prokázané změny editor zapíše poslední známý stav.

#### H. Praktický závěr

§ 14 zakládá subjektivní práva osoby vůči jejím údajům v ZR: ověřené výstupy (CzechPOINT), právo na záznam o přístupech (transparentnost), proaktivní notifikaci při změně do datové schránky a bezplatnou reklamaci s opravou v krátké lhůtě 3 pracovních dnů.

**Checklist (advokát / soud / správní orgán / adresát normy):**
- [ ] Žádá o záznam o přístupech subjekt údajů (odst. 3), nebo jiná osoba se zvláštním zákonným titulem?
- [ ] Je záznam/výpis poskytnut bezplatně, případně jako ověřený výstup (odst. 4)?
- [ ] Byla reklamace podána (i přes CzechPOINT) a předána editorovi (odst. 6)?
- [ ] Dodržel editor lhůtu 3 pracovních dnů podle § 4 odst. 3?
- [ ] Má subjekt zpřístupněnou datovou schránku pro proaktivní notifikaci (odst. 5)?

**Typicky rozhodné důkazy / podklady:** výpis z ROB, doklad o skutečném stavu (pobyt, matriční doklad), žádost o opravu s datem, potvrzení CzechPOINT, záznam o využívání údajů.

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

#### F. Kazuistika

**1. Modelová situace.** Soukromá společnost stáhne podstatnou část dat z RUIAN (databáze adresních míst) a komerčně ji nabízí jako vlastní produkt bez souhlasu správce. Správce RUIAN (ČÚZK) se brání. Současně vzniká spor, který orgán je oprávněn rozhodovat o podmínkách poskytnutí dat třetím stranám. Účastníci: soukromá společnost, správce příslušného ZR (ČÚZK pro RUIAN), stát jako vlastník. Důkazy: rozsah staženého obsahu, doklad o správcovství databáze, podmínky poskytování dat.

**2. Právní otázka.** Kdo vlastní základní registry a jejich infrastrukturu a kdo vykonává zvláštní právo pořizovatele databáze, jež je základem ochrany před neoprávněným užitím?

**3. Použitelné právo.**
- *Komentované ustanovení:* § 15 — ZR, ISZR a ISSS jsou majetkem státu; zvláštní právo pořizovatele databáze vykonává správce příslušného ZR.
- *Související ustanovení téhož zákona:* § 7 odst. 1 (DIA správce ISZR/ISSS), § 20 (DIA správce ROB), správcovství RUIAN (ČÚZK) a ROS (Agentura), § 58–58a (poskytování údajů).
- *Související předpisy:* § 88 a násl. autorského zákona (zvláštní právo pořizovatele databáze — ochrana podstatné části obsahu).
- *Judikatura:* nosný výklad pojmu „podstatná část databáze" a podmínek zásahu do zvláštního práva pořizovatele (judikatura Soudního dvora EU k databázové směrnici).

**4. Subsumpce.** RUIAN je majetkem státu a zvláštní právo pořizovatele databáze vykonává jeho správce — ČÚZK (§ 15). Stažení a komerční nabízení „podstatné části" obsahu bez souhlasu správce zasahuje do tohoto zvláštního práva. Podmínka neoprávněného užití podstatné části je naplněna; oprávněným k ochraně je správce (ČÚZK), nikoli stát obecně.

**5. Řešení.** Správce RUIAN (ČÚZK) uplatní zvláštní právo pořizovatele databáze a brání se proti neoprávněnému užití podstatné části (zdržení se, náhrada škody). O podmínkách poskytování dat třetím stranám rozhoduje správce příslušného ZR. Procesně: doložit rozsah užití (podstatnost části), správcovství databáze, neexistenci souhlasu. Riziko: u nepodstatné části nebo při zákonné výjimce může ochrana selhat.

**6. Varianty.** (a) Šlo-li by jen o nepodstatnou část obsahu, zásah do zvláštního práva by nemusel být dán. (b) U jiného registru (ROB, RPP) by zvláštní právo vykonávala DIA, u ROS Agentura — určení správce mění aktivně legitimovaný subjekt.

#### G. Protiargumenty a rizika

- *Protiargument:* „Veřejná data jsou volně použitelná, ochrana databáze se neuplatní." — Neutralizace: veřejná přístupnost údaje neznamená vzdání se zvláštního práva pořizovatele k databázi jako celku; podstatná část je chráněna podle autorského zákona.
- *Protiargument:* „Vlastníkem je konkrétní úřad, který může s daty nakládat libovolně." — Neutralizace: § 15 určuje vlastníkem stát; správce jen vykonává zvláštní právo pořizovatele — nakládání je vázáno zákonem.
- *Slabé místo:* hranice „podstatné části" databáze je výkladově náročná; bez doložení rozsahu užití je ochrana obtížně vymahatelná.

#### H. Praktický závěr

§ 15 určuje, že základní registry, ISZR a ISSS jsou majetkem státu, přičemž zvláštní právo pořizovatele databáze vykonává správce příslušného registru. Toto právo je nástrojem ochrany před neoprávněným kopírováním a základem pro podmínky poskytování dat třetím stranám.

**Checklist (advokát / soud / správní orgán / adresát normy):**
- [ ] Který subjekt je správcem dotčeného ZR (DIA/ČÚZK/Agentura) a vykonává zvláštní právo pořizovatele?
- [ ] Jde o užití „podstatné části" obsahu databáze (§ 88 a násl. autorského zákona)?
- [ ] Existuje souhlas správce / zákonná výjimka pro užití?
- [ ] O podmínkách poskytnutí dat třetí straně rozhoduje správce příslušného ZR?

**Typicky rozhodné důkazy / podklady:** doklad o správcovství databáze, rozsah a způsob užití obsahu, podmínky poskytování dat, neexistence souhlasu.

---

## HLAVA II — Registr obyvatel

### § 16 — Předmět ROB

> **§ 16**
>
> *V registru obyvatel jsou o fyzických osobách uvedených v § 17 vedeny referenční údaje a další údaje, o nichž tak stanoví tento zákon.*

**Výklad:**

§ 16 stanoví **funkci ROB** — vést referenční a další údaje o fyzických osobách v zákonem vymezeném okruhu (§ 17). ROB tedy **není evidencí všech lidí žijících v ČR**, nýbrž jen těch, kteří splňují podmínky § 17 (občané ČR, cizinci s pobytem, azylanti a další zákonem stanovené osoby).

ROB tvoří **referenční datovou základnu** pro identifikaci fyzických osob ve veřejné správě. Všechny ostatní AIS, které potřebují identifikovat osobu, vedou referenční vazby do ROB a samy údaje neuchovávají duplicitně.

#### F. Kazuistika

**1. Modelová situace.** Úřad chce ověřit identitu krátkodobého turisty z třetí země (pobyt 14 dnů), a předpokládá, že jeho údaje najde v ROB. V ROB ho nenajde a uvažuje, zda jde o chybu registru. Účastníci: úřad (čerpající OVM), cizinec-turista, správce ROB. Důkazy: pobytový status osoby, dotaz do ROB, evidence v AIS cizinců.

**2. Právní otázka.** Vede ROB údaje o všech fyzických osobách nacházejících se v ČR, nebo jen o zákonem vymezeném okruhu osob?

**3. Použitelné právo.**
- *Komentované ustanovení:* § 16 — v ROB se vedou referenční a další údaje o fyzických osobách uvedených v § 17, o nichž tak stanoví zákon.
- *Související ustanovení téhož zákona:* § 17 (taxativní okruh subjektů ROB), § 18 (katalog vedených údajů), § 4 (vlastnosti referenčních údajů).
- *Související předpisy:* zákon č. 326/1999 Sb. (pobyt cizinců) — AIS cizinců; zákon č. 133/2000 Sb. (evidence obyvatel).
- *Judikatura:* obecná zásada, že rozsah evidence je dán zákonným vymezením okruhu evidovaných osob; mimo něj evidence neexistuje.

**4. Subsumpce.** ROB vede údaje jen o osobách podle § 17 (§ 16). Krátkodobý turista (pobyt do 90 dnů, bez trvalého/dlouhodobého pobytu) do okruhu § 17 nespadá. Absence jeho údaje v ROB tedy není chybou — podmínka „subjekt podle § 17" splněna není.

**5. Řešení.** Úřad nemůže turistu v ROB najít, protože tam být nemá; jeho údaje jsou vedeny v AIS cizinců, nikoli jako referenční údaj v ROB. Identitu ověří jinou cestou (doklad totožnosti, AIS cizinců, je-li k němu oprávněn). Procesně: nehledat v nesprávném zdroji; využít správnou evidenci podle pobytového statusu. Riziko mylného závěru o „chybě ROB" odpadá znalostí okruhu § 17.

**6. Varianty.** (a) Získá-li cizinec dlouhodobý pobyt nad 90 dnů, stane se subjektem ROB (§ 17 písm. b) a jeho údaje tam budou vedeny. (b) U občana ČR žijícího trvale v zahraničí je v ROB veden vždy (§ 17 písm. a), byť fakticky v ČR nepobývá.

#### G. Protiargumenty a rizika

- *Protiargument:* „ROB je evidence všech lidí v ČR." — Neutralizace: § 16 ve spojení s § 17 omezuje okruh na zákonem vymezené osoby; mnohé osoby v ČR (turisté) v ROB nejsou.
- *Protiargument:* „Chybí-li osoba v ROB, jde o vadu registru." — Neutralizace: absence osoby mimo okruh § 17 je souladná se zákonem, nikoli vada.
- *Slabé místo:* hranice okruhu § 17 (zejm. přechodný pobyt, doplňková ochrana) je proměnlivá v čase; status osoby je nutné ověřit k rozhodnému datu.

#### H. Praktický závěr

§ 16 vymezuje funkci ROB jako referenční datové základny o fyzických osobách, avšak jen o těch v okruhu § 17. ROB není evidencí všech osob v ČR; ostatní jsou vedeni v agendových systémech a v ROB nejsou referenčním údajem.

**Checklist (advokát / soud / správní orgán / adresát normy):**
- [ ] Spadá osoba do okruhu subjektů ROB podle § 17?
- [ ] Hledá orgán údaj ve správném zdroji (ROB vs. AIS cizinců)?
- [ ] Je absence osoby v ROB souladná se zákonem (mimo okruh § 17), nebo skutečná vada?

**Typicky rozhodné důkazy / podklady:** doklad o pobytovém statusu osoby, dotaz do ROB, evidence v AIS cizinců.

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

#### F. Kazuistika

**1. Modelová situace.** Žadatel o azyl (před vydáním rozhodnutí) se domáhá zápisu do ROB s argumentem, že na území ČR pobývá. Souběžně občan EU, který má v ČR přechodný pobyt v délce 2 měsíců, žádá o zápis do ROB. Účastníci: žadatel o azyl, občan EU s přechodným pobytem, editor (MV/Policie ČR), správce ROB. Důkazy: doklad o pobytovém statusu, délka a typ pobytu, rozhodnutí o (ne)udělení ochrany.

**2. Právní otázka.** Které kategorie cizinců a osob jsou subjekty údajů vedených v ROB a od jakého okamžiku/statusu?

**3. Použitelné právo.**
- *Komentované ustanovení:* § 17 — taxativní výčet: a) občané ČR, b) cizinci s trvalým/dlouhodobým pobytem nebo dlouhodobým vízem, c) občané EU/EHP a rodinní příslušníci s trvalým nebo přechodným pobytem nad 3 měsíce, d) osoby s mezinárodní ochranou (azyl/doplňková), e) jiné osoby podle zvláštního zákona.
- *Související ustanovení téhož zákona:* § 16 (funkce ROB), § 18 (vedené údaje), § 19 (editoři podle kategorie subjektu).
- *Související předpisy:* zákon č. 325/1999 Sb., o azylu; zákon č. 326/1999 Sb., o pobytu cizinců; zákon č. 186/2013 Sb., o státním občanství.
- *Judikatura:* obecná zásada vázanosti statusu na splnění zákonných podmínek pobytu/ochrany; status žadatele se liší od statusu osoby s udělenou ochranou.

**4. Subsumpce.** Žadatel o azyl (před rozhodnutím) nemá udělenu mezinárodní ochranu podle písm. d) — je veden v AIS cizinců, nikoli v ROB; podmínka písm. d) splněna není. Občan EU s přechodným pobytem 2 měsíce nesplňuje práh „nad 3 měsíce" podle písm. c) — do okruhu ROB nespadá; podmínka písm. c) splněna není.

**5. Řešení.** Ani žadatel o azyl, ani občan EU s pobytem do 3 měsíců nejsou subjekty ROB — jejich údaje se vedou v příslušných AIS. Po udělení ochrany (azyl/doplňková) se žadatel stane subjektem ROB (písm. d); po překročení 3 měsíců přechodného pobytu se subjektem stane občan EU (písm. c). Procesně: ověřit status k rozhodnému datu a vést osobu ve správné evidenci. Riziko mylného zápisu/nenalezení odpadá znalostí prahů.

**6. Varianty.** (a) Udělením doplňkové ochrany se osoba zařadí pod písm. d) a stane subjektem ROB. (b) „Jiná osoba" se stane subjektem ROB jen tehdy, stanoví-li to zvláštní zákon (písm. e) — bez něj nikoli.

#### G. Protiargumenty a rizika

- *Protiargument:* „Každý cizinec dlouhodobě v ČR je v ROB." — Neutralizace: rozhoduje typ a délka pobytu / status ochrany podle písm. b)–d); samotná přítomnost nestačí.
- *Protiargument:* „Žadatel o azyl má stejný status jako azylant." — Neutralizace: písm. d) míří na osoby s udělenou ochranou; žadatel před rozhodnutím tam nespadá.
- *Slabé místo:* prahové podmínky (3 měsíce u EU, druh víza u třetích zemí) jsou citlivé na časový okamžik; status je nutné posuzovat ke konkrétnímu datu.

#### H. Praktický závěr

§ 17 taxativně vymezuje subjekty ROB podle občanství a pobytového statusu. Klíčové prahy: u občanů EU přechodný pobyt nad 3 měsíce, u osob s ochranou až po jejím udělení. Mimo tyto kategorie je osoba vedena jen v agendových systémech.

**Checklist (advokát / soud / správní orgán / adresát normy):**
- [ ] Do které kategorie § 17 písm. a)–e) osoba spadá k rozhodnému datu?
- [ ] Je splněn prahový požadavek (typ/délka pobytu, udělení ochrany)?
- [ ] Jde o žadatele o ochranu (AIS cizinců) nebo o osobu s udělenou ochranou (ROB, písm. d)?
- [ ] U „jiných osob" existuje zvláštní zákon zakládající zápis (písm. e)?

**Typicky rozhodné důkazy / podklady:** doklad o pobytovém statusu, rozhodnutí o udělení ochrany, doklad o občanství, doklad o délce přechodného pobytu.

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

**Judikatura (z místních zdrojů):**

- *NSS* [10 Af 7/2023 - 50](https://vyhledavac.nssoud.cz/DokumentOriginal/Text/717012) — 16. 11. 2023
  > „V registru obyvatel či osob (včetně právnických a podnikajících fyzických osob) jsou vedeny údaje jmenované v § 18 a § 26 zákona č. 111/2009 Sb., o základních registrech, v platném a účinném znění. Mezi těmito údaji nejsou údaje o tom, zda jsou osoby vedeny jako osoby účastnící se důchodového nebo nemocenského pojištění (srov. citovaná ustanovení § 18 a § 26 zákona o základních registrech). Z citovaných ustanovení tedy vyplývá, že účast na nemocenském pojištění (či důchodovém pojištění) není údajem vedeným v registru osob"
- *NSS* [31 A 14/2023 - 38](https://vyhledavac.nssoud.cz/DokumentOriginal/Text/716091) — 26. 9. 2023
  > „Daňový řád vychází z formálních předpokladů místa pobytu či sídla (z jejich zapsání v příslušných registrech) a není rozhodné, zda se adresát v místě doručení zdržuje. … V základním registru obyvatel [srovnej § 3 odst. 1 písm. a) a § 18 odst. 1 písm. d) zákona č. 111/2009 Sb., o základních registrech, ve znění pozdějších předpisů] je uvedena adresa místa pobytu fyzické osoby, případně též adresa, na kterou jí mají být doručovány písemnosti podle jiného právního předpisu"

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

#### F. Kazuistika

**1. Modelová situace.** Orgán veřejné moci je pro svou agendu oprávněn čerpat z ROB jméno a adresu místa pobytu osoby. Potřebuje jí doručit písemnost a chce využít i adresu pro doručování a údaj o datové schránce, aniž by je měl výslovně ve výčtu zpřístupněných údajů. Současně dceřin úřad chce z ROB čerpat telefonní číslo osoby pro „efektivnější komunikaci". Účastníci: čerpající OVM, subjekt údajů, správce ROB. Důkazy: registrace agendy a výčet zpřístupněných údajů, povaha jednotlivých údajů (referenční vs. neferenční).

**2. Právní otázka.** Které údaje v ROB jsou referenčními (závaznými) a může orgán čerpající některé referenční údaje automaticky využít i údaje pro doručování, doklady a datovou schránku, případně telefon?

**3. Použitelné právo.**
- *Komentované ustanovení:* § 18 odst. 2 (referenčními údaji jsou údaje písm. a)–k)), odst. 6 (rozšířené oprávnění čerpat adresu pro doručování, údaje písm. j)–m) a datum poslední změny — bez výslovného uvedení ve výčtu), odst. 1 písm. l) (telefon/e-mail — neferenční), odst. 3 (autentizační údaje v jednosměrně šifrované podobě).
- *Související ustanovení téhož zákona:* § 4 (vlastnosti referenčního údaje), § 5 odst. 1 (čerpání v rámci výčtu zpřístupněných údajů), § 19 (editoři a zápis).
- *Související předpisy:* GDPR čl. 5 (minimalizace); zákon č. 300/2008 Sb. (datové schránky) pro písm. k).
- *Judikatura:* obecná zásada účelového omezení a zákazu nadbytečného zpracování; rozšířené oprávnění je výjimkou, kterou nelze vykládat extenzivně nad rámec textu.

**4. Subsumpce.** Adresa pro doručování (písm. d), čísla dokladů (písm. j), datová schránka (písm. k) a certifikát (písm. m) spadají do rozšířeného oprávnění odst. 6 — orgán čerpající některé referenční údaje je smí využít i bez výslovného uvedení ve výčtu; podmínka odst. 6 splněna. Telefon/e-mail (písm. l) je neferenční a do výčtu odst. 6 nepatří — jeho čerpání „pro efektivitu" zákonný základ nemá; podmínka splněna není.

**5. Řešení.** Orgán smí na základě odst. 6 využít adresu pro doručování, čísla dokladů, datovou schránku a certifikát, aniž je má výslovně ve výčtu — „balíčková" logika usnadňuje doručení. Telefon/e-mail (písm. l) však čerpat nesmí, není-li k tomu titul; je to neferenční údaj sloužící jen pro zasílání zvolených informací. Procesně: doručovat přes datovou schránku / adresu pro doručování; telefon nečerpat bez titulu. Riziko: čerpání písm. l) bez titulu je nezákonné zpracování.

**6. Varianty.** (a) Má-li osoba zpřístupněnou datovou schránku (písm. k), je to přednostní kanál doručení a využití je kryto odst. 6. (b) Autentizační údaje (písm. n) nelze „přečíst" — jsou v jednosměrně šifrované podobě (odst. 3), takže ani správce nezíská jejich hodnotu.

#### G. Protiargumenty a rizika

- *Protiargument:* „Kdo má přístup ke jménu a adrese, má přístup ke všem údajům v ROB." — Neutralizace: odst. 6 rozšiřuje oprávnění jen na taxativně vyjmenované údaje (adresa pro doručování, písm. j–m, datum změny); ostatní vyžadují vlastní titul.
- *Protiargument:* „Telefon v ROB je referenční, takže ho lze čerpat." — Neutralizace: odst. 2 činí referenčními jen písm. a)–k); telefon/e-mail (písm. l) referenční není a do rozšíření odst. 6 nespadá.
- *Slabé místo:* hranice mezi referenčními (a)–k) a neferenčními (l)–o) údaji se v praxi přehlíží; chybné zacházení s neferenčním údajem jako se závazným je vada.

#### H. Praktický závěr

§ 18 je katalogem údajů ROB ve třech vrstvách: referenční (písm. a)–k), neferenční (písm. l)–o), provozní (odst. 5). Údaje, které jsou referenční v jiném ZR, se vedou jen jako referenční vazba (kód). Rozšířené oprávnění (odst. 6) umožňuje čerpat vybrané kontaktní a dokladové údaje i bez jejich výslovného uvedení ve výčtu.

**Checklist (advokát / soud / správní orgán / adresát normy):**
- [ ] Je čerpaný údaj referenční (písm. a)–k) nebo neferenční (písm. l)–o)?
- [ ] Spadá do rozšířeného oprávnění odst. 6 (adresa pro doručování, písm. j)–m), datum změny)?
- [ ] Není čerpán neferenční údaj (telefon/e-mail) bez vlastního titulu?
- [ ] Je adresa/místo narození/úmrtí brána jako referenční vazba (kód) na RUIAN, nikoli textově?

**Typicky rozhodné důkazy / podklady:** registrace agendy a výčet zpřístupněných údajů, povaha jednotlivých údajů (referenční/neferenční), logy čerpání z ROB.

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

#### F. Kazuistika

**1. Modelová situace.** Občan ČR si na portálu veřejné správy chce doplnit do ROB telefonní číslo a e-mail pro zasílání informací a aktivovat data pro elektronickou identifikaci. Současně cizinec s dlouhodobým pobytem reklamuje, že jeho jméno je v ROB zapsáno v jiném přepisu než v matričním dokladu. Účastníci: občan ČR, cizinec, Agentura (DIA), MV/Policie ČR jako editoři. Důkazy: žádost přes portál, matriční/cestovní doklad cizince, log zápisu.

**2. Právní otázka.** Kdo je editorem jednotlivých údajů v ROB a podle jaké předlohy se zapisuje jméno cizince?

**3. Použitelné právo.**
- *Komentované ustanovení:* § 19 odst. 1 (MV editor pro občany ČR; rozdělení mezi IS evidence obyvatel a IS OP/cestovních dokladů), odst. 2, 3 (Policie ČR/MV editor pro cizince přes AIS cizinců), odst. 4 (jméno cizince podle matričního dokladu, jinak latinkou z cestovního dokladu), odst. 5 (provozní údaje zapisuje Agentura automatizovaně), odst. 6 (datová schránka — správce ISDS), odst. 7 (telefon/e-mail/EID — Agentura na žádost subjektu přes portál).
- *Související ustanovení téhož zákona:* § 18 (katalog údajů), § 4 odst. 2, 3 (odpovědnost a lhůta editora), § 20 (správce ROB).
- *Související předpisy:* zákon č. 133/2000 Sb. (evidence obyvatel); zákon č. 326/1999 Sb. (pobyt cizinců); zákon č. 301/2000 Sb. (matriky).
- *Judikatura:* obecná zásada, že zápis údaje provádí zákonem určený editor; transliterace jména se řídí úředním dokladem.

**4. Subsumpce.** Telefon, e-mail a požadavek na EID (písm. l, m, n) zapisuje podle odst. 7 Agentura na žádost subjektu přes portál — občan je tedy oprávněn si je sám doplnit; podmínka odst. 7 splněna. Jméno cizince se zpracovává podle matričního dokladu, a nebyl-li vydán, latinkou z cestovního dokladu (odst. 4) — reklamace přepisu se posoudí proti matričnímu/cestovnímu dokladu; editorem je MV/Policie ČR (odst. 2, 3).

**5. Řešení.** Občan ČR si přes portál veřejné správy doplní telefon/e-mail a aktivuje EID — zápis provede Agentura (odst. 7). Cizincovo jméno editor (MV/Policie ČR) opraví tak, aby odpovídalo matričnímu dokladu, případně latinkové podobě z cestovního dokladu (odst. 4), ve lhůtě § 4 odst. 3. Procesně: žádost přes portál vs. reklamace u editora; doložit doklad pro správný přepis. Riziko: bez správného dokladu nelze přepis jména jednoznačně určit.

**6. Varianty.** (a) Údaj o datové schránce (písm. k) zapisuje správce ISDS (odst. 6), nikoli MV — reklamace tohoto údaje směřuje jinam. (b) Provozní údaje (§ 18 odst. 5) píše Agentura automatizovaně (odst. 5) — nelze je „opravit" jako věcný údaj, jde o audit-trail.

#### G. Protiargumenty a rizika

- *Protiargument:* „Všechny údaje v ROB zapisuje jeden editor (MV)." — Neutralizace: editorství je rozděleno podle subjektu a druhu údaje (MV, Policie ČR, správce ISDS, Agentura); reklamaci je nutné směřovat správnému editorovi.
- *Protiargument:* „Občan si nemůže sám měnit údaje v ROB." — Neutralizace: odst. 7 výslovně umožňuje, aby telefon, e-mail a EID požadavek zapsala Agentura na žádost subjektu přes portál.
- *Slabé místo:* správný přepis jména cizince závisí na existenci matričního/cestovního dokladu; při jejich absenci nebo rozporu je zápis sporný.

#### H. Praktický závěr

§ 19 zavádí distribuované editorství ROB: MV pro občany ČR (rozděleno mezi IS evidence obyvatel a IS dokladů), Policie ČR/MV pro cizince, správce ISDS pro datovou schránku, Agentura pro provozní údaje a pro telefon/e-mail/EID na žádost občana. Jméno cizince se zapisuje podle matričního, jinak cestovního dokladu (latinkou).

**Checklist (advokát / soud / správní orgán / adresát normy):**
- [ ] Který editor je příslušný pro daný údaj (MV / Policie ČR / správce ISDS / Agentura)?
- [ ] Jde o údaj, který si subjekt doplňuje sám přes portál (telefon, e-mail, EID — odst. 7)?
- [ ] U cizince — odpovídá jméno matričnímu dokladu, jinak latinkové podobě z cestovního dokladu (odst. 4)?
- [ ] Jsou provozní údaje (odst. 5) chápány jako automatizovaný audit-trail, nikoli věcný údaj?

**Typicky rozhodné důkazy / podklady:** žádost přes portál veřejné správy, matriční/cestovní doklad cizince, log zápisu, určení příslušného editora.

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

#### F. Kazuistika

**1. Modelová situace.** Obecní úřad obce s rozšířenou působností (matriční úřad) chybně zapíše údaj v ROB. Občan se domáhá nápravy a chce vědět, kdo za pochybení odpovídá a kdo dohlíží na výkon přenesené působnosti obce v oblasti ROB. Zároveň vzniká otázka, kdo odpovídá za samotný výpadek databáze ROB. Účastníci: občan, obecní úřad ORP (editor v přenesené působnosti), DIA (správce ROB), krajský úřad. Důkazy: doklad o chybném zápisu, vymezení rolí editor/správce, podklady kontroly přenesené působnosti.

**2. Právní otázka.** Kdo je správcem ROB, jak se liší jeho odpovědnost od odpovědnosti editora a kdo kontroluje výkon přenesené působnosti obcí v oblasti ROB?

**3. Použitelné právo.**
- *Komentované ustanovení:* § 20 odst. 1 (správcem ROB je Agentura/DIA), odst. 2 (poskytování údajů podle § 58, 58a), odst. 3 (DIA kontroluje výkon přenesené působnosti ÚSC; tím není dotčena kontrola krajskými úřady podle zákona o obcích), odst. 4 (zpracování údajů v rozsahu § 18).
- *Související ustanovení téhož zákona:* § 19 (editoři — MV/Policie ČR), § 4 odst. 2 (odpovědnost editora za soulad se zdrojem), § 7 (DIA jako správce ISZR/ISSS).
- *Související předpisy:* zákon č. 128/2000 Sb., o obcích (kontrola přenesené působnosti krajskými úřady); zákon č. 471/2022 Sb., o DIA; zákon č. 82/1998 Sb. (odpovědnost za nesprávný úřední postup).
- *Judikatura:* nosné rozlišení odpovědnosti za obsah zápisu (editor) a za provoz/bezpečnost systému (správce); odpovědnost státu za nesprávný úřední postup.

**4. Subsumpce.** Za správnost zápisu odpovídá editor (§ 4 odst. 2, § 19), nikoli správce; za provoz a bezpečnost ROB odpovídá DIA jako správce (§ 20 odst. 1). Výkon přenesené působnosti obce v oblasti ROB kontroluje DIA (odst. 3), aniž je dotčena kontrola krajskými úřady podle zákona o obcích. Chybný zápis tedy spadá na editora; výpadek databáze na správce (DIA).

**5. Řešení.** Nápravu chybného zápisu řeší editor (reklamace, § 14 odst. 6, lhůta § 4 odst. 3); za provozní výpadek odpovídá DIA. Dohled nad přenesenou působností obce vykonává DIA (odst. 3) souběžně s kontrolou krajského úřadu. Procesně: směřovat reklamaci editorovi; provozní stížnost správci; doložit povahu pochybení. Riziko záměny odpovědných subjektů odpadá rozlišením rolí editor/správce.

**6. Varianty.** (a) Jde-li o poskytování údajů třetím osobám, řídí se § 58 a 58a a zajišťuje je Agentura (odst. 2). (b) Selhání obce v přenesené působnosti řeší jak DIA (odst. 3), tak krajský úřad podle zákona o obcích — kontroly se nevylučují.

#### G. Protiargumenty a rizika

- *Protiargument:* „Za vše v ROB odpovídá jeho správce DIA." — Neutralizace: § 20 odst. 1 svěřuje DIA provoz a bezpečnost; za správnost obsahu zápisu odpovídá editor (§ 4 odst. 2) — role jsou oddělené.
- *Protiargument:* „Kontrolu obce vykonává jen DIA, nikoli kraj." — Neutralizace: odst. 3 výslovně zachovává kontrolu krajskými úřady podle zákona o obcích — obě kontroly koexistují.
- *Slabé místo:* hranice mezi pochybením editora a provozní vadou správce může být v konkrétním incidentu nejasná; nutné skutkové rozlišení příčiny.

#### H. Praktický závěr

§ 20 určuje DIA správcem ROB s odpovědností za provoz, bezpečnost a poskytování údajů. Odpovědnost za správnost zápisu nese editor (MV/Policie ČR). Výkon přenesené působnosti obcí v oblasti ROB kontroluje DIA souběžně s kontrolou krajských úřadů.

**Checklist (advokát / soud / správní orgán / adresát normy):**
- [ ] Jde o vadu obsahu zápisu (editor) nebo o provozní/bezpečnostní vadu (správce DIA)?
- [ ] Je reklamace směřována správnému subjektu (editor vs. správce)?
- [ ] Probíhá kontrola přenesené působnosti obce přes DIA i krajský úřad (odst. 3)?
- [ ] Řídí se poskytování údajů třetím osobám § 58 a 58a (odst. 2)?

**Typicky rozhodné důkazy / podklady:** doklad o povaze pochybení (zápis vs. provoz), vymezení rolí editor/správce, podklady kontroly přenesené působnosti.

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

#### F. Kazuistika

**1. Modelová situace.** Osoba byla před 48 lety prohlášena soudem za mrtvou (nezvěstná v zahraničí). Údaje jsou stále v ROB, neboť 50letá lhůta dosud neuplynula. Dědicové se domáhají, aby byly údaje již zlikvidovány. Souběžně badatel-genealog žádá o přístup k údajům jiné osoby, která zemřela před 55 lety a jejíž záznam již byl zlikvidován. Účastníci: dědicové, badatel, správce ROB (DIA). Důkazy: rozhodnutí o prohlášení za mrtvého a jeho právní moc, datum úmrtí, stav záznamu v ROB.

**2. Právní otázka.** Po jakou dobu se údaje subjektu uchovávají v ROB a kdy se likvidují, včetně provozních záznamů?

**3. Použitelné právo.**
- *Komentované ustanovení:* § 22 odst. 1 (uchovávání 50 let od smrti nebo právní moci rozhodnutí o prohlášení za mrtvého), odst. 2 (není-li údaj o úmrtí, 50 let od poslední aktualizace), odst. 3 (po uplynutí likvidace, kromě provozních údajů podle § 18 odst. 5, jež se vedou dalších 10 let).
- *Související ustanovení téhož zákona:* § 18 odst. 1 písm. f) (údaj o úmrtí), § 18 odst. 5 (provozní údaje), § 23 (nové pořízení po likvidaci).
- *Související předpisy:* § 71 a násl. občanského zákoníku (prohlášení za mrtvého); § 27 autorského zákona (lhůty); zákon č. 110/2019 Sb. (zásada omezeného uložení).
- *Judikatura:* obecná zásada omezeného uchovávání osobních údajů (čl. 5 odst. 1 písm. e) GDPR); konstitutivní účinky rozhodnutí o prohlášení za mrtvého.

**4. Subsumpce.** U osoby prohlášené za mrtvou běží 50letá lhůta od právní moci rozhodnutí (odst. 1); uplynulo 48 let — lhůta dosud neuplynula, údaje se nelikvidují. Požadavek dědiců na předčasnou likvidaci podmínku odst. 1 nesplňuje. U osoby zemřelé před 55 lety lhůta uplynula a věcné údaje byly zlikvidovány (odst. 3); badatel je již v ROB nenajde, byť provozní záznamy mohou existovat ještě 10 let.

**5. Řešení.** Údaje prohlášené za mrtvou osoby zůstávají v ROB do uplynutí 50 let od právní moci rozhodnutí; předčasná likvidace na žádost dědiců není možná. U osoby po uplynutí 50 let jsou věcné údaje zlikvidovány a genealogická rešerše přes ROB není možná (provozní údaje se vedou ještě 10 let, ale neslouží badatelskému přístupu). Procesně: ověřit počátek a běh lhůty (právní moc/úmrtí/poslední aktualizace). Riziko: záměna počátku lhůty (smrt vs. právní moc) vede k chybnému určení data likvidace.

**6. Varianty.** (a) Není-li veden údaj o úmrtí (osoba „administrativně zmizela"), běží 50 let od poslední aktualizace alespoň jednoho údaje (odst. 2). (b) Po likvidaci a opětovném zjištění, že osoba žije, se postupuje podle § 23 (nové pořízení AIFO a údajů).

#### G. Protiargumenty a rizika

- *Protiargument:* „Dědicové mohou žádat o okamžitou likvidaci údajů zemřelého." — Neutralizace: § 22 stanoví pevnou 50letou lhůtu; předčasná likvidace na žádost není upravena.
- *Protiargument:* „Po smrti se vše ihned maže." — Neutralizace: lhůta je 50 let (od smrti/právní moci/poslední aktualizace) a provozní údaje přetrvávají dalších 10 let (odst. 3).
- *Slabé místo:* určení počátku lhůty se liší podle situace (odst. 1 vs. odst. 2); u prohlášení za mrtvého je rozhodná právní moc, nikoli den uvedený jako den smrti — záměna je častou chybou.

#### H. Praktický závěr

§ 22 stanoví uchovávání údajů v ROB po dobu 50 let (od smrti, právní moci rozhodnutí o prohlášení za mrtvého, nebo poslední aktualizace), poté likvidaci — s výjimkou provozních údajů vedených ještě 10 let. Předčasná likvidace na žádost není upravena.

**Checklist (advokát / soud / správní orgán / adresát normy):**
- [ ] Jaký je počátek 50leté lhůty (smrt / právní moc rozhodnutí / poslední aktualizace)?
- [ ] Je veden údaj o úmrtí (odst. 1), nebo se uplatní odst. 2 (poslední aktualizace)?
- [ ] Byly po uplynutí lhůty zlikvidovány věcné údaje a vedou se provozní údaje ještě 10 let (odst. 3)?
- [ ] Není požadována předčasná likvidace, kterou zákon neumožňuje?

**Typicky rozhodné důkazy / podklady:** rozhodnutí o prohlášení za mrtvého a doklad o právní moci, údaj o datu úmrtí, doklad o poslední aktualizaci, stav záznamu v ROB.

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

#### F. Kazuistika

**1. Modelová situace.** Osoba byla v minulosti prohlášena za mrtvou, její údaje v ROB byly po uplynutí lhůty zlikvidovány. Po návratu ze zahraničí se prokáže, že žije, a žádá o obnovení záznamu v ROB. Současně se obává, že obnovou „ožijí" i historická propojení (např. dávné záznamy navázané na její původní identifikátor). Účastníci: subjekt údajů, správní orgán vedoucí agendu evidence obyvatel (podnět), Agentura (DIA), editor ROB. Důkazy: doklad o tom, že osoba žije, podnět podaný přes příslušný správní orgán, poslední stav vedený v IS evidence obyvatel.

**2. Právní otázka.** Jak se po likvidaci údajů obnoví záznam osoby v ROB, obnoví se původní identifikátor, a podle jakého stavu se zapisují ostatní údaje?

**3. Použitelné právo.**
- *Komentované ustanovení:* § 23 odst. 1 (na podnět subjektu přes správní orgán evidence obyvatel/cizinců zajistí Agentura nové pořízení AIFO), odst. 2 (ostatní zlikvidované údaje se nově pořídí opakovanou editací z IS evidence obyvatel/AIS cizinců na podnět subjektu), odst. 3 (editor zapisuje podle posledního stavu vedeného v AIS, neprokáže-li subjekt změnu).
- *Související ustanovení téhož zákona:* § 22 (likvidace po 50 letech), § 9, § 10 (povaha a pravidla AIFO), § 11 (ÚOOÚ jako tvůrce AIFO), § 19 (editoři ROB).
- *Související předpisy:* § 71 a násl. občanského zákoníku (prohlášení za mrtvého, jeho zrušení); zákon č. 133/2000 Sb. (evidence obyvatel).
- *Judikatura:* obecná zásada ochrany před „digitálním stigmatem" a před trvalým propojením historických záznamů s aktuální identitou; právo na omezení uchovávání (čl. 5 odst. 1 písm. e) GDPR).

**4. Subsumpce.** Po likvidaci se na podnět subjektu pořizuje NOVÉ AIFO (odst. 1) — nikoli obnova původního; tím historické záznamy navázané na původní identifikátor nezůstanou propojeny. Ostatní údaje se obnoví opakovanou editací z IS evidence obyvatel (odst. 2), je-li tam jejich poslední stav zachován. Editor zapíše poslední stav, neprokáže-li subjekt změnu (odst. 3). Podmínky pro nové pořízení AIFO i obnovu údajů jsou splněny.

**5. Řešení.** Agentura na podnět (podaný přes správní orgán evidence obyvatel) zajistí nové AIFO; ostatní údaje se obnoví z IS evidence obyvatel podle posledního stavu, ledaže subjekt prokáže změnu (pak se zapíše změněný stav). Obava z „oživení" historických propojení je lichá — nové AIFO je právě zárukou proti tomu (odst. 1). Procesně: podat podnět přes příslušný správní orgán; doložit aktuální stav, liší-li se od posledního. Riziko: nezachoval-li agendový systém údaje, obnova není možná a osoba se zapíše „od nuly".

**6. Varianty.** (a) Prokáže-li subjekt změnu některého údaje (např. novou adresu), editor zapíše aktuální stav, nikoli historický (odst. 3). (b) Nebyl-li v AIS poslední stav zachován, ostatní údaje nelze obnovit editací (odst. 2) a osoba je pořízena nově, jen s novým AIFO.

#### G. Protiargumenty a rizika

- *Protiargument:* „Po obnově se vrátí původní identifikátor a s ním všechna historická propojení." — Neutralizace: odst. 1 zakládá nové AIFO, nikoli obnovu starého — historická propojení se neobnoví; jde o záměrnou ochranu před digitálním stigmatem.
- *Protiargument:* „Údaje se obnoví automaticky bez podnětu subjektu." — Neutralizace: odst. 1 i 2 vyžadují podnět subjektu (podaný přes příslušný správní orgán); bez něj se neobnovuje.
- *Slabé místo:* obnova ostatních údajů závisí na tom, zda je AIS zachoval; při jejich absenci je obnova fakticky vyloučena a chybí zdroj pro „poslední stav".

#### H. Praktický závěr

§ 23 řeší opětovné pořízení záznamu po likvidaci: na podnět subjektu Agentura zajistí NOVÉ AIFO (ne obnovu původního — ochrana před propojením historických záznamů) a ostatní údaje se obnoví editací z IS evidence obyvatel podle posledního stavu, neprokáže-li subjekt změnu.

**Checklist (advokát / soud / správní orgán / adresát normy):**
- [ ] Byl podán podnět subjektu přes příslušný správní orgán (evidence obyvatel/cizinců)?
- [ ] Pořizuje se NOVÉ AIFO, nikoli obnova původního (odst. 1)?
- [ ] Jsou ostatní údaje obnovitelné editací z IS evidence obyvatel (odst. 2) — zachoval je AIS?
- [ ] Zapisuje editor poslední stav, nebo subjekt prokázal změnu (odst. 3)?

**Typicky rozhodné důkazy / podklady:** podnět subjektu, doklad o tom, že osoba žije / o novém pobytu, poslední stav vedený v IS evidence obyvatel, doklad o případné změně údajů.
