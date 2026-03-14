# Data Science Tech Stack Magyarországon (AI Kísérlet) 🤖📊

Egy interaktív, egyoldalas webalkalmazás (SPA), amely bemutatja a hazai Data Science munkaerőpiac technológiai elvárásait **junior, medior és senior** szintekre bontva egy véletlenszerű pillanatban vizsgálva 2026-os álláshirdetések alapján.

👉 **[Élő demó megtekintése itt](https://csabatatrai.hu/hu-data-science-tech-stack-by-seniority/)**

> [!IMPORTANT]
> Akár ennek mintájára más szakmákra is érdemes lehet hasonlót elkészíttetni, amihez a fenti kód jó kiindulási alap csak oszd meg Geminivel, miközben a Deep Reasearch be van pipálva és írd meg neki, melyik szakma érdekel ennek mintájára!

## 💡 A projekt háttere

Ez a projekt egy **LLM (Large Language Model) kísérlet** eredménye. A cél az volt, hogy felmérjem, képes-e a Google Gemini Deep Research funkció segítségével egyetlen egy prompt alapján:
1. Aggregálni a magyarországi adatos álláspiac pillanatnyi elvárásait (NoFluffJobs, Profession.hu, LinkedIn adatok alapján).
2. Szintetizálni az információkat szenioritási szintek szerint.
3. Megtervezni és lekódolni egy komplett, interaktív frontend dashboardot az adatok vizualizálására.

A repoban található HTML kód **egy az egyben a nyelvi modell outputja**, manuális kódolási beavatkozás nélkül.

## ✨ Funkciók

* **Interaktív szenioritás-választó:** Váltás a Junior, Medior és Senior szintek között.
* **Képességprofil (Radar Chart):** Vizuálisan ábrázolja, hol vannak a fókuszok az adott szinten (pl. Programozás vs. MLOps).
* **Technológiai részletezés:** Konkrét eszközök (Python, SQL, K8s, Docker stb.) listája, iparági indoklással és referencialinkekkel.
* **Készség-evolúció (Stacked Bar Chart):** Egy összehasonlító ábra, amely megmutatja, hogyan tolódik el a hangsúly a tiszta programozástól az architektúra tervezés és az MLOps felé a karrierút során.

## 🛠️ Tech Stack

A projekt szándékosan "Zero-build" megközelítéssel készült, hogy egyetlen fájlban futtatható legyen:
* **HTML5** (Szemantikus felépítés)
* **Tailwind CSS** (CDN-en keresztül, a gyors és reszponzív designért)
* **Chart.js** (CDN-en keresztül, a Canvas-alapú interaktív diagramokért)
* **Vanilla JavaScript** (Állapotkezelés, DOM manipuláció és interakciók)

> [!CAUTION]
> Ez egy vibe-kódolt weblap, ilyen összetettségű vizualizációt már rábízhatsz egy LLM-re!

## 🚀 Futtatás lokálisan

Mivel a projekt egyetlen statikus HTML fájlból áll, semmilyen szerver vagy build folyamat nem szükséges:
1. Klónozd a repót: `git clone https://github.com/FELHASZNALONEVED/REPO_NEVE.git`
2. Nyisd meg a letöltött mappát.
3. Kattints duplán a `index.html` (vagy ahogy elnevezted) fájlra, és már meg is nyílik a böngésződben.

## ⚠️ Limitációk és Értelmezés

Fontos kiemelni, hogy ez a vizualizáció egy **pillanatfelvétel**, ami a generáláskori álláshirdetések kulcsszavait tükrözi.
* **Radar diagram értelmezése:** Ha egy seniornál az adatvizualizáció alacsony értéket kap, az nem azt jelenti, hogy azt nem várják el. A diagram a **piaci differenciáló fókuszokat** mutatja. A senior kiírásokban ezt már "alaphigiéniának" veszik, és inkább a szűk keresztmetszetet jelentő technológiákat (pl. Cloud, MLOps, LLM) hangsúlyozzák.
* **Soft skillek:** A projekt szigorúan a "hard" technológiai stackre fókuszál, a domaintudás és a soft skillek nem szerepelnek benne.
* **Nem validált, hosszútávú, reprezentatív adatok, csak egy pillanatkép, nincs mögötte se backend, se pipeline ami valós időben frissítené!!!**

## 🤝 Kapcsolat & Visszajelzés
Kíváncsi vagyok a véleményedre!

Ha észrevételed van a hazai elvárt tech stackkel kapcsolatban, esetleg van hasonló témájú projekted amit megosztanál, keress meg a személyes oldalamon található formon:
**[csabatatrai.hu](https://csabatatrai.hu/)**

Vagy vegyük fel a kapcsolatot LinkedIn-en:
**[Csaba A. Tátrai](https://www.linkedin.com/in/csabatatrai-datascientist/)**

