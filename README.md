# 📊 Projekt Power BI – Analýza mezd a cen potravin v ČR  

## Úvod  
Tento report představuje analýzu vývoje průměrných mezd a cen vybraných potravin v České republice v letech **2006–2018**.  
Cílem je ukázat, jak se vyvíjely mzdy v jednotlivých odvětvích, jak se měnily ceny základních potravin a jak si Česká republika stojí v evropském srovnání.

Report je vytvořen v **Power BI** jako pokračování SQL projektu, kde byla připravena vstupní datová tabulka.  

---

## Použitá data  
- **t_diana_lehka_project_sql_primary_final**  
  Obsahuje sjednocená data o mzdách a cenách potravin v ČR.  
  - Sloupce: `year`, `industry_code`, `industry_name`, `avg_wage_czk`, `food_code`, `food_name`, `avg_price_czk`, `value`, `unit`.  

- **t_diana_lehka_project_sql_secondary_final**  
  Obsahuje data o HDP, GINI koeficientu a populaci vybraných evropských států.  
  - Sloupce: `country`, `year`, `gdp`, `gini`, `population`.  

---

## Struktura reportu  
Report má celkem **4 stránky + úvodní menu**.  

### 1. Úvod & Menu  
- Název projektu, logo a stručný popis.  
- Navigační tlačítka na jednotlivé části reportu.  

### 2. Přehled - ceny, mzdy a HDP
- KPI karty: průměrná mzda, průměrná cena potravin, průměrná HDP.  
- Spojnicový graf - vývoj mezd vs. cen potravin v čase.  
- Slicer: rok, odvětví, potravina.

### 3. Mzdy podle odvětví  
- Skládaný sloupcový graf: průměrná mzda podle odvětví.
- Skládaný sloupcový graf: TOP 5 průměrná mzda podle odvětví.  
- Skládaný plošný graf: vývoj průměrné mzdy v čase.  
- Slicer: rok, odvětví.
- Záložky: odkazující na graf průměrné mzdy nebo graf TOP 5.

### 4. Ceny potravin  
- KPI karty: potravina s minimální a maximální průměrnou cenou.  
- Skládaný pruhový graf: průměrné ceny potravin.  
- Tabulka: jednotlivé ceny potravin.
- Kalkulovaný sloupec: **Price Category (Levná/Drahá)**.
- Slicer: rok, potravina.
- Záložky: nejlevnější a nejdražší potravina.

### 5. Mezinárodní srovnání  
- Donut graf: Porovnání HDP vybraných států.
- Mapa: HDP vybraných evropských zemí.  
- Slicer: rok, země.  

---

## Interaktivní prvky  
- **Navigace mezi stránkami** (menu, logo).  
- **Slicery** (rok, odvětví, potravina, země).  
- **Záložky** – přepínání mezi pohledy.

## Measure
- Average Wage, Average Price, Average GDP

## Kalkulovaný sloupec
- Price Category (Levná/Drahá)

---

## Požadavky projektu  
- Rozsah 2-5 stránek
- Použití minimálně 5 různých typů vizuálů
- Filtrování (primárně) pomocí průřezů/slicerů
- Využití interaktivních prvků jako jsou záložky, navigace po stranách, odkazy na webové stránky, ...
- Propojení několika (2+) datových tabulek, buď přes vazby v rámci Power BI nebo přes propojení v Power Query
- Vytvoření alespoň 1 measure (metrika/míra) a 1 kalkulovaného sloupce/tabulky
- Grafická úprava použitých vizuálů, zvolení správných typů vizuálů a vizuálně přívětivý výsledný report

---

## Shrnutí  
Report ukazuje:  
- Vývoj průměrných mezd v jednotlivých odvětvích v ČR.  
- Změny cen základních potravin.  
- Mezinárodní kontext – HDP a GINI vybraných evropských států.
