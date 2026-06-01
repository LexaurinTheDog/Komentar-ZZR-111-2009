# Úvod — Zákon č. 111/2009 Sb., o základních registrech (ZZR)

## Postavení zákona v právním řádu

Zákon č. 111/2009 Sb., o základních registrech (dále „**ZZR**"), je **klíčovým pilířem českého eGovernmentu** a představuje jeden z nejvýznamnějších legislativních počinů v oblasti veřejné správy po roce 2000. Cílem zákona je vybudovat **jednotnou, spolehlivou a sdílenou datovou infrastrukturu státu**, na jejímž základě mohou orgány veřejné moci i soukromoprávní uživatelé bez duplicit a redundancí pracovat s **referenčními údaji** — tedy údaji, které jsou v České republice **jediné platné, závazné a sdílené**.

ZZR opouští paradigma vícekrát opakovaného sběru týchž údajů různými úřady („**princip vícenásobné evidence**") a nahrazuje jej **principem jednoho zápisu — mnoha využití** (write-once-use-many). Občan, podnikatel ani právnická osoba již nemají povinnost prokazovat úřadu skutečnosti, které jsou již vedeny v některém ze základních registrů — orgán veřejné moci si je musí získat sám prostřednictvím **referenčního rozhraní**.

## Vazba na předcházející a navazující předpisy

ZZR navazuje na dva klíčové předpisy budující informační infrastrukturu veřejné správy:

1. **Zákon č. 365/2000 Sb., o informačních systémech veřejné správy (ZISVS)** — obecný rámec pro správu, provoz a sdílení informačních systémů veřejné správy. ZISVS definuje pojem **referenčního rozhraní** (§ 2 písm. i)), jehož součástí jsou Informační systém základních registrů (**ISZR**) a Informační systém sdílené služby (**ISSS**) zakotvené v ZZR.
2. **Zákon č. 300/2008 Sb., o elektronických úkonech a autorizované konverzi dokumentů (ZDS)** — zákon o datových schránkách. Identifikátor datové schránky je referenčním údajem vedeným v ROB a RPO (§ 18 odst. 1 písm. k), § 26 odst. 2 písm. h)) a slouží jako primární komunikační kanál mezi orgány veřejné moci a osobami zapsanými v základních registrech.

Po nabytí účinnosti GDPR a zákona č. 110/2019 Sb., o zpracování osobních údajů se ZZR stal nedílnou součástí systému ochrany osobních údajů ve veřejné správě. Mimořádný význam má rovněž **zákon č. 12/2020 Sb., o právu na digitální služby**, který občanům přiznává **vymahatelné subjektivní právo** vyžadovat digitální komunikaci s úřady — toto právo je technicky realizovatelné jen díky existenci základních registrů.

## Čtyři základní registry — pilíř datové architektury

Zákon zřizuje čtveřici základních registrů, které se vzájemně doplňují a tvoří **propojený, ale technicky oddělený celek**:

| Registr | Zkratka | Předmět | Správce | Editor |
|---|---|---|---|---|
| Registr obyvatel | **ROB** | Fyzické osoby (občané ČR, cizinci s pobytem, azylanti) | Digitální a informační agentura | MV, Policie ČR |
| Registr osob | **RPO** (registr osob) | Právnické osoby, OSVČ, OVM, svěřenské fondy | Digitální a informační agentura | Agendová místa (rejstříkové soudy, ŽÚ, FÚ aj.) |
| Registr územní identifikace, adres a nemovitostí | **RUIAN** | Územní prvky (obce, kat. území, ulice, adresní místa, stavební objekty, parcely) | Český úřad zeměměřický a katastrální | Katastrální úřady, stavební úřady, obce, ČSÚ |
| Registr práv a povinností | **RPP** | Agendy, orgány veřejné moci, soukromoprávní uživatelé, oprávnění k rolím | Digitální a informační agentura | Ohlašovatelé agend (ústřední správní úřady) |

> **Pozor na zkratku „RPO"** — ZZR sám v textu používá termín **„registr osob"** (legislativní zkratka v § 3 písm. b)). V praxi se však pro něj často užívá zkratka „**RPO**" (Registr Právnických Osob), zatímco zkratka „**RPP**" (Registr Práv a Povinností) označuje registr podle § 3 písm. d). V tomto komentáři pracuji s legislativní zkratkou „registr osob" pro ROS/RPO a „registr práv a povinností" pro RPP.

## Pomocné systémy referenčního rozhraní

K základním registrům se váží další informační systémy, bez nichž by ZZR nemohl fungovat:

1. **ISZR — Informační systém základních registrů** (§ 7) — provozovaný Digitální a informační agenturou. Jediná „dálnice" pro přístup k referenčním údajům. Bez ISZR nelze do registrů zapisovat ani z nich číst.
2. **ISSS — Informační systém sdílené služby** (§ 2 písm. h)) — pro sdílení údajů mezi agendovými informačními systémy, které **nezapisují** do základních registrů.
3. **ORG — Převodník identifikátorů** (zakotvený v § 9–11 a vykonávaný Úřadem pro ochranu osobních údajů) — anonymizovaný převod mezi **agendovými identifikátory fyzických osob (AIFO)** napříč agendami. Klíčový bezpečnostní prvek: znemožňuje propojování osobních údajů napříč ISVS bez zákonného oprávnění.
4. **Autentizační informační systém** (§ 56a) — eviduje fyzické osoby, které jsou nositeli rolí (úředníky), a provádí jejich autentizaci při přístupu k registrům.
5. **Informační systém oprávnění k zastupování** (§ 52e) — eviduje plné moci a oprávnění zástupce vůči veřejné správě.

## Referenční údaje — jádro celého systému

Pojem **referenční údaj** (§ 4) je nejvýznamnějším právním institutem zavedeným ZZR. Referenční údaj je údaj vedený v základním registru, který je označen jako referenční — a má tyto vlastnosti:

1. **Platnost erga omnes** — je platným a závazným údajem pro celou veřejnou správu. Žádný úřad nemůže od osoby požadovat doložení skutečnosti, kterou již referenční údaj zachycuje (§ 5 odst. 2).
2. **Domněnka správnosti** — referenční údaj se považuje za správný, pokud není prokázán opak nebo nevznikla oprávněná pochybnost (§ 4 odst. 4).
3. **Důvěra v zápis** — kdo z referenčního údaje vychází, je v dobré víře (§ 4 odst. 6); proti tomu, kdo jednal v důvěře, nelze namítat nesprávnost údaje (§ 4 odst. 7).
4. **Editor odpovídá za zápis** — referenční údaj zapisuje výhradně **editor** (§ 4 odst. 2), který je za jeho správnost odpovědný. Editorství je formálně přiděleno zákonem ke konkrétnímu orgánu veřejné moci.

## Agendový princip — AIS, agendy, role

ZZR opustil model „přímého přístupu úředníka do databáze" a zavedl tzv. **agendový princip**: každý orgán veřejné moci přistupuje k referenčním údajům **prostřednictvím agendového informačního systému (AIS)** a v rámci konkrétní **agendy**. Agenda je „ucelená oblast působení orgánu veřejné moci" (§ 2 písm. e)) — typicky odpovídá jednomu zákonu nebo jeho části (např. agenda evidence obyvatel, agenda živnostenského podnikání).

Pro výkon agendy musí:

1. **Ústřední správní úřad agendu ohlásit** Digitální a informační agentuře (§ 53). Ohlášení obsahuje výčet referenčních údajů, které pro výkon agendy úřad potřebuje, a jejich odůvodnění (princip nezbytnosti dle čl. 5 odst. 1 písm. c) GDPR).
2. **DIA agendu zaregistrovat** a přidělit jí kód agendy (§ 54).
3. **Orgány veřejné moci se zaregistrovat pro výkon agendy** (§ 55) — teprve poté získávají oprávnění k přístupu k referenčním údajům v rozsahu rolí podle § 51 odst. 6 písm. c).

Tento mechanismus umožňuje **granulární kontrolu přístupu**: úřad nemůže přistupovat ke všem údajům v základním registru, nýbrž jen k těm, které pro výkon své agendy a v rámci své role potřebuje.

## ORG a problematika propojování osobních údajů

Architektura ZZR řeší jeden z klíčových konfliktů eGovernmentu — **propojitelnost údajů versus ochrana před profilováním občanů státem**. Řešením je princip **agendových identifikátorů fyzické osoby (AIFO)**: každá agenda má svůj vlastní AIFO pro téhož občana, přičemž tyto identifikátory jsou navzájem neodvoditelné. Převod mezi AIFO v jedné a druhé agendě může provést **výhradně Úřad pro ochranu osobních údajů** (§ 11), a to jen na základě zákonného požadavku.

Tím se zabraňuje vytvoření jediného „supervedoucího" identifikátoru, jakým je rodné číslo, a fakticky se znemožňuje propojování osobních údajů napříč ISVS bez zákonné opory — i pro stát samotný.

## Reklamace nesprávných údajů

ZZR poskytuje subjektu údajů jednoduchý mechanismus opravy nesprávného referenčního údaje — § 14 odst. 6 zakotvuje právo bezplatně požádat editora o opravu, a to i prostřednictvím **kontaktního místa veřejné správy (CzechPOINT)**. Editor je povinen rozhodnout o opravě nebo zápisu změny do **3 pracovních dnů** (§ 4 odst. 3).

## Dohled — ÚOOÚ a DIA

ZZR rozděluje dohledové pravomoci mezi dva orgány:

1. **Úřad pro ochranu osobních údajů (ÚOOÚ)** — dohled nad zpracováním osobních údajů (§ 7 odst. 7, § 60a). Spravuje ORG a zdrojový identifikátor fyzické osoby (§ 11).
2. **Digitální a informační agentura (DIA)** — dohled nad dodržováním povinností podle ZZR samotného (§ 62d), kontrola výkonu přenesené působnosti (§ 20 odst. 3), a faktický provoz ISZR, ISSS, ROB a RPP.

## Klíčové novely

Zákon byl od svého přijetí (9. března 2009) novelizován vícekrát. Z nejvýznamnějších uvádím:

- **Zákon č. 100/2010 Sb.** — drobné úpravy před nabytím účinnosti.
- **Zákon č. 167/2012 Sb.** — rozšíření okruhu subjektů ROB o cizince s krátkodobým pobytem; rozšíření kategorií ROS.
- **Zákon č. 192/2016 Sb.** — zpřesnění zapisování údajů, posílení kontrolních mechanismů.
- **Zákon č. 12/2020 Sb., o právu na digitální služby** — návazná úprava: zavedl § 4a (údaje v AIS), § 5a (využití údajů soukromoprávními uživateli), § 52c–52e (rejstříky informačních systémů a oprávnění k zastupování) a další; přenastavil pravidla využití referenčních údajů soukromoprávními subjekty.
- **Zákon č. 471/2022 Sb.** — zřízení **Digitální a informační agentury (DIA)**, na kterou s účinností od **1. dubna 2023** přešly kompetence Ministerstva vnitra a Správy základních registrů (SZR). Od této novely je správcem ISZR, ISSS, ROB a RPP **DIA** (dříve Ministerstvo vnitra prostřednictvím SZR).
- **Zákon č. 277/2019 Sb.** — terminologické úpravy a uvedení do souladu se zákonem č. 110/2019 Sb., o zpracování osobních údajů (adaptační zákon ke GDPR).

## Účinnost

ZZR nabyl **plné účinnosti 1. července 2010** (§ 70); některá ustanovení (§ 6, § 7, § 63 odst. 2 a 3) nabyla účinnosti již **1. ledna 2010** kvůli přípravným pracím. **Faktický provoz** základních registrů byl spuštěn **1. července 2012**, kdy byla dokončena dvouletá transformační fáze předvídaná v § 64–68.

K dnešnímu dni je verze zákona účinná **od 1. ledna 2026** (kód SB-2009-00111_2026-01-01), reflektující novely související s plnou funkčností DIA a poslední úpravy v oblasti elektronické identifikace a autentizace.
