# Data Science Tech Stack Magyarországon 2026-ban (AI Kísérlet) 
🤖📊

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

## 🤝 Kapcsolat

**[csabatatrai.hu](https://csabatatrai.hu/)**

LinkedIn:
**[Csaba A. Tátrai](https://www.linkedin.com/in/csabatatrai-datascientist/)**

