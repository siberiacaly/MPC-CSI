# Projekt do předmětu MPC-CSI

## Zadání projektu

Cílem bylo vytvořit funkční skript pro **statistickou analýzu reálných dat**.  
Použit je **dataset statistik hráčů NBA** (National Basketball Association) – tato data jsou dále zpracována a analyzována.  
Jednotlivé parametry (např. body, výška, váha) jsou zkoumány z pohledu **náhodných procesů**.  
Součástí je také **vizualizace dat a odhad funkcí hustoty pravděpodobnosti (PDF)**.

---

## 1. Načtení a statistické zpracování dat

Prvním krokem bylo zajištění importu databáze a výběr relevantních veličin.  
Z datového souboru jsou extrahovány klíčové parametry hráčů pro další zpracování.

- Zpracování probíhá v prostředí **MATLAB** (Live Script).
- Výpočet základních charakteristik: **střední hodnota**, **rozptyl** a **směrodatná odchylka**.
- Analýza vybraných sloupců (např. průměrný počet bodů na zápas).

### Ukázka statistické analýzy:

![Ukázka výpočtu statistik](ukazka_vypoctu.png)

---

## 2. Vizualizace a odhad rozdělení pravděpodobnosti

Po získání popisných statistik skript provádí **grafickou vizualizaci**.  
Generují se histogramy pro ověření typu rozdělení dat a jejich četnosti.

**Skript provádí:**

- vykreslení **normovaného histogramu** vybrané veličiny
- proložení dat teoretickou křivkou (**odhad PDF**)
- porovnání teoretického modelu s reálnými daty

> Analýza slouží k ověření, zda data odpovídají normálnímu (Gaussovu) rozdělení nebo vykazují jiné statistické vlastnosti.

Výstupní grafy obsahují jak experimentální data (sloupce histogramu), tak proloženou teoretickou hustotu pravděpodobnosti.

## Odkaz na kódy

- [💾 Hlavní skript (Live Script)](./StatistikaCalabek237881.mlx)

## Shrnutí funkcionality

- ✅ Import a parsování datasetu NBA statistik
- ✅ Výpočet střední hodnoty, rozptylu a směrodatné odchylky
- ✅ Tvorba histogramů četností
- ✅ Odhad a vykreslení funkce hustoty pravděpodobnosti (PDF)
- ✅ Interaktivní prezentace výsledků v MATLAB Live Editoru

---

## Použité platformy a technologie

- Prostředí: **MATLAB (verze s podporou .mlx)**
- Jazyk: **MATLAB Script**
- Knihovny: **Statistics and Machine Learning Toolbox**
- Formát dat: **Strukturovaná data (NBA dataset)**
- Výstup: **Live Script, Grafy**

---

> Projekt byl vypracován Bc. Tomášem Calábkem (ID: 237881) jako semestrální úloha pro kurz **MPC-CSI** (Číslicové signály a systémy) na VUT FEKT.
