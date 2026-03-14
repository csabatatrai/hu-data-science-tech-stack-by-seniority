# Prompt Documentation - Munkaerőpiaci Hard Skill Igények Vizsgálata

> Pillanatnyi álláshirdetéseken alapuló, LLM-asszisztált adatgyűjtés és vizualizáció.

---

## Metadata

| Mező              | Érték                          |
|-------------------|-------------------------------|
| Projekt           | Munkaerőpiaci skill-igény elemzés |
| Szerző            | Tátrai Csaba Attila           |
| Utolsó frissítés  | 2026-03-14                       |
| LLM               | Google Gemini 3.1 Pro         |
| Mód               | Deep Research / Paid tier                 |
| Státusz           | `published`                       |

---

## Prompt 1 - Adatgyűjtés és strukturálás

### Cél

Junior, medior és senior szintű data science álláshirdetésekben leggyakrabban elvárt technológiák feltérképezése a magyarországi munkaerőpiacon.

### Konfiguráció

```yaml
mode: Deep Research
grounding: web search enabled
response_language: hu
```

### Prompt szövege

```text
Milyen technológiákat keresnek leginkább junior, medior és senior data science
állásajánlatokban Magyarországon?

Szedd erre a 3 kategóriára és csinálj felsorolást, hivatkozd meg linkekkel az
állításaid!
```

### Elvárt kimenet

- Három kategóriás (junior / medior / senior) strukturált lista
- Technológiánként legalább 1 forráshivatkozás (álláshirdetés-URL vagy aggregátor)

### Megjegyzések

- A Deep Research mód több keresési iterációt végez, ami növeli a lefedettséget, de lassabb.
- Érdemes a kimenetet CSV-be exportálni a downstream analízishez.

---

## Prompt 2 - Interaktív vizualizáció

### Cél

Az összegyűjtött adatok egyoldalas webalkalmazásként (SPA) való megjelenítése, szintenkénti bontással és interaktív elemekkel.

### Konfiguráció

```yaml
mode: Deep Research
input: output of Prompt 1
```

### Prompt szövege

```text
Készíts egy interaktív, egyoldalas webalkalmazást (SPA), amely átfogóan bemutatja
a magyarországi Data Science munkaerőpiac technológiai elvárásait, junior, medior
és senior szintekre bontva, a kért hivatkozásokkal és interaktív vizualizációkkal.
```

### Elvárt kimenet

- Önálló, böngészőben futtatható HTML/JS/CSS fájl
- Szintenként szűrhető nézet
- Forrásokra mutató linkek megjelenítve

### Megjegyzések

- A prompt az 1. prompt kimenetére épít, önállóan nem értelmezhető.
- Ha a generált SPA külső CDN-t használ (pl. Chart.js), az offline nem fog működni.

---

## Changelog

| Verzió | Dátum    | Változás                        |
|--------|----------|---------------------------------|
| 1.0    | 2026-03-14  | Első draft, két alapprompt      |