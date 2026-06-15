# Õpimapp: ProjectLibre Kasutusjuhend

**Üliõpilane:** Timur  
**Rühm:** TARpv24  
**Õppeaine:** Projekti juhtimine / Tarkvara arendus  

---

## Sisukord
1. [Projekti eesmärk](#projekti-eesmärk)
2. [Tehtud ülesannete nimekiri (Task List)](#tehtud-ülesannete-nimekiri-task-list)
3. [Muudetud ja loodud failid](#muudetud-ja-loodud-failid)
4. [Lisatud funktsionaalsus](#lisatud-funktsionaalsus)
5. [Koodinäide ja märkused](#koodinäide-ja-märkused)

---

## Projekti eesmärk

Selle iseseisva töö eesmärgiks oli luua veebipõhine kasutusjuhend tarkvara **ProjectLibre** jaoks. Töö käigus õppisin harude (branch) haldamist Git-is, GitHub Issues ja Kanban projektiplaani kasutamist ning veebilehe struktuuri muutmist vastavalt uuele tarkvarale. 

Töö teostati täielikult eraldi arendusharus nimega `projectLibre`.

---

## Tehtud ülesannete nimekiri (Task List)

*   [x] Loodud uus branch nimega `projectLibre` ja lülitutud sellele.
*   [x] Seadistatud GitHub Kanban laud (Project board) ja lisatud 3 issue't.
*   [x] Uuendatud pealeht (`index.html`) ProjectLibre kalendri õpetusega.
*   [x] Loodud uus diagrammide leht (`diagramm.html`) koos Gantt graafikuga.
*   [x] Kustutatud projektist vana fail `valem.html` [^1].
*   [x] Muudetud navigeerimismenüü (navbar) ja kontrollitud linkide toimivust.
*   [x] Tehtud regulaarsed commitid, mis sulgevad automaatselt seotud issues (nt *Fixes #1*).

---

## Muudetud ja loodud failid

| Faili tee | Olek | Selgitus |
| :--- | :--- | :--- |
| `index.html` | Muudetud | Lisatud `MinuOmaKalender` loomise ja seadistamise sammud. |
| `diagramm.html` | Uus fail | Gantt diagrammi ja ressursside vaate kirjeldus. |
| `valem.html` | Kustutatud | Fail eemaldatud, kuna seda ei läinud uues ülesandes vaja. |
| `style.css` | Kontrollitud | Kohandatud menüü ja piltide paigutus (Flexbox, ümarad nurgad). |
| `README.md` | Uus fail | Käesolev aruanne ja dokumentatsioon õpetajale. |

---

## Lisatud funktsionaalsus

### 1. Kalendri haldamine ProjectLibre-s
*   **Uue kalendri loomine:** Menüüst `Tools -> Calendar -> New...` loodi kalender nimega `MinuOmaKalender`.
*   **Tööaja seadistamine:** Muudeti standardsed tööpäevad ja seadistati puhkepäevad.
*   **Projektiga sidumine:** Menüüst `File -> Information` määrati loodud kalender kogu projekti põhiliseks kalendriks.

### 2. Diagrammid ja graafikud
*   Sisestati testiülesanded (*Planeerimine, Disaini väljatöötamine, Testimine jne*).
*   Määrati ülesannete vahelised seosed (eelnevad tegevused) ja lisati ressursid (`Developer`, `Designer`).
*   Genereeriti automaatne Gantt diagramm.

---

## Koodinäide ja märkused

Siin on näide sellest, kuidas HTML struktuuris muudeti navigeerimismenüüd, et eemaldada viide kustutatud failile:

```html
<!-- Uuendatud navbar ilma valem.html lingita -->
<nav class="navbar">
    <a href="index.html" class="active">Uue kalendri loomine</a>
    <a href="diagramm.html">Diagrammide loomine</a>
</nav>
