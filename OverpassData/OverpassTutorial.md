# Získání a zpracování dat o rychlostních kamerách pomocí Overpass Turbo

Tento dokument popisuje postup získání a využití dat o rychlostních kamerách z otevřené databáze **OpenStreetMap (OSM)** pomocí dotazovacího systému **Overpass** a jeho webového rozhraní **Overpass Turbo**. Získaná data jsou použita v rámci ročníkového projektu z oblasti mikropočítačových systémů, kde slouží jako podklad pro práci s GPS polohou.

---

## 1. Overpass a OpenStreetMap

**OpenStreetMap** je otevřený mapový projekt, jehož data jsou vytvářena a udržována komunitou uživatelů po celém světě. Jedná se tedy o **community-based databázi**, kde může docházet k neúplnostem nebo nepřesnostem dat. Z tohoto důvodu není možné zaručit, že všechna uvedená data jsou vždy 100 % aktuální nebo přesná.

**Overpass** je dotazovací systém, který umožňuje číst a filtrovat data z databáze OpenStreetMap podle zadaných kritérií, jako je typ objektu nebo jeho poloha. Je využíván především pro analytické, výukové a vývojové účely.

---

## 2. Overpass QL a Overpass Turbo

Pro vytváření dotazů se používá jazyk **Overpass QL (Query Language)**. Tento jazyk umožňuje přesně definovat, jaká data mají být z databáze získána.

**Overpass Turbo** je webové rozhraní k systému Overpass, které umožňuje:
- psaní a testování Overpass QL dotazů
- okamžité zobrazení výsledků na mapě
- export získaných dat do různých formátů

Webová aplikace je dostupná na adrese:  
https://overpass-turbo.eu

---

## 3. Datový model OpenStreetMap

V databázi OpenStreetMap jsou geografické objekty ukládány jako:
- **node** – bodový objekt
- **way** – liniový nebo plošný objekt
- **relation** – logická vazba mezi objekty

Rychlostní kamery jsou nejčastěji reprezentovány jako **node** s tagem:
[CameraData](CameraData.yaml)


