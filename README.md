# engeto_pbi_project
Power BI project regarding data analysis of Czechia payrolls in industries and GDP comparison of world economies in years 2006 to 2018 


Průvodní listina


Popis projektu:
Analýza mezd v českých odvětvích v letech 2006 až 2008 spolu s porovnáním hrubého domácího produktu a GINI koeficientu mezi světovými ekonomikami.


Použité datové sady

Primární tabulky:
czechia_payroll – Informace o mzdách v různých odvětvích za několikaleté období. Datová sada pochází z Portálu otevřených dat ČR.
czechia_payroll_calculation – Číselník kalkulací v tabulce mezd.
czechia_payroll_industry_branch – Číselník odvětví v tabulce mezd.
czechia_payroll_unit – Číselník jednotek hodnot v tabulce mezd.
czechia_payroll_value_type – Číselník typů hodnot v tabulce mezd.
economies - HDP, GINI, daňová zátěž, atd. pro daný stát a rok.


Výstup projektu


Primární list s názvem 'Mzdy v odvětvích' byl vytvořen seskupením dat z tabulek 'czechia_payroll' a 'economies'. Provázání dat bylo provedeno pomocí sloupců s hodnotami datumů na společné roky. Z tabulky 'czechia_payroll' byly vybrány pouze záznamy s hodnotou 'Průměrná hrubá mzda na zaměstnance'. Pro konkretizaci označení průmyslových odvětví byly ještě připojeny data z tabulky 'czechia_payroll_industry_branch'. Dále byly připojeny data týkající se HDP z tabulky 'economies' Výsledná tabulka obsahuje data shromážděná ve sloupcích s druhy průmyslových odvětví, roky, průměrné mzdy a HDP ČR. 
Primární list přináší grafický přehled průměrných mezd v letech 2006 až 2018 ve srovnání s HDP ČR pro všechna odvětví s možností filtrování na jednotlivá odvětví spolu s tabulkovým přehledem všech výstupních hodnot týkajících se mezd.

Sekundární list s názvem 'Ekonomiky' byl vytvořen z tabulky 'economies'. Byly vybrány pouze záznamy v letech 2006 až 2018 tak, aby se shodovaly s roky primárního přehledu pro ČR. Vyselektovány byly NULL hodnoty ve sloupci GINI koeficientů, které jsou pro větší územní celky, nikoliv samostatné státy. Výsledná tabulka obsahuje data shromážděná ve sloupcích se jmény států, let, HDP, velikostí populace, GINI koeficientů a dopočítané sloupce s rozdělením GINI koeficientů do 7 kategorií a HDP na obyvatele.
Sekundární list přináší grafické porovnání hrubých domácích produktů a hrubých domácích produktů na obyvatele v letech 2006 až 2018 s porovnáním GINI koeficientů a jejich rozdělením do kategorií spolu s možností filtrování na jednotlivé země.

