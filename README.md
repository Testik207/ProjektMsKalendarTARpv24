# Õpimapp: Microsoft Project Kasutusjuhend

**Üliõpilane:** Timur  
**Rühm:** TARpv24  
**Õppeaine:** Projekti juhtimine / Tarkvara arendus  

---

## Sisukord
1. [Projekti eesmärk](#projekti-eesmärk)
2. [Tehtud ülesannete nimekiri (Task List)](#tehtud-ülesannete-nimekiri-task-list)
3. [Veebilehe struktuur](#veebilehe-struktuur)
4. [Käsitletud teemad MS Projectis](#käsitletud-teemad-ms-projectis)
5. [Koodinäide ja disain](#koodinäide-ja-disain)

---

## Projekti eesmärk

Selle praktilise töö eesmärgiks oli luua veebipõhine samm-sammuline kasutusjuhend tarkvara **Microsoft Project** jaoks. Veebileht on koostatud puhtas HTML/CSS keeles ning sisaldab reaalsetest projektidest võetud kuvatõmmiseid ja selgitusi esitatud ülesannete kohta.

---

## Tehtud ülesannete nimekiri (Task List)

*   [x] Loodud veebilehe baasstruktuur ja navigatsioonimenüü.
*   [x] Koostatud juhend uue kalendri loomise ja projektiga sidumise kohta (`index.html`).
*   [x] Lisatud valemite ja arvutusväljade (Custom Fields) kasutamise õpetus (`valem.html`).
*   [x] Visualiseeritud projekti kulude ülevaade ehk diagrammid (`diagramm.html`).
*   [x] Kujundatud kaasaegne ja stiilne välimus, kasutades eraldi stiilifaili (`style.css`).

---

## Veebilehe struktuur

| Faili nimi | Lehe pealkiri | Kirjeldus |
| :--- | :--- | :--- |
| `index.html` | Uue kalendri loomine | Juhend baaskalendri seadistamiseks ja tööaja muutmiseks. |
| `valem.html` | Arvutusvälja lisamine | Õpetus, kuidas lisada kohandatud välju ja matemaatilisi valemeid [[^1]]. |
| `diagramm.html` | Diagrammide loomine | Projekti eelarve ja kulude (Cost Overview) visuaalne raport. |
| `style.css` | - | Fail, mis vastutab lehe kujunduse, fontide ja menüü (Flexbox) eest. |

[^1]: Valemite lisamisel kasutati MS Projecti sisseehitatud kohandatud väljade (Custom Fields) funktsiooni.

---

## Käsitletud teemad MS Projectis

### 1. Kalendri mõju graafikule
*   Õpiti uue 5-päevase töönädala kalendri seadistamist.
*   Määrati riigipühad ja puhkused eranditena (Exceptions).
*   Uuriti, kuidas kalendri muutmine nihutab automaatselt ülesannete lõppkuupäevi [^2].

### 2. Kulude analüüs ja diagrammid
*   Sisestati projekti ressursid ja nende tunnitasud.
*   Genereeriti visuaalne kuluülevaade (Dashboard -> Cost Overview), mis kuvab reaalajas eelarve jääki ja kulutusi graafikutena.

[^2]: Kui märkida tööpäev puhkepäevaks, lükkab MS Project planeeritud tegevused järgmisele tööpäevale.

---

## Koodinäide ja disain

Navigeerimismenüü kood, mis tagab mugava liikumise kõigi kolme MS Projecti teemalehe vahel:

```html
<!-- Esimese etapi navigatsioonimenüü -->
<nav class="navbar">
    <a href="index.html">Uue kalendri loomine</a>
    <a href="valem.html">Arvutusvälja lisamine</a>
    <a href="diagramm.html">Diagrammide loomine</a>
</nav>
