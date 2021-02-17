# CSS to the Rescue Process
**@cmda-minor-web** 2020 - 2021

# Opdracht
Bij dit vak ga ik alle hoeken van CSS bekijken. Met pure CSS ga ik een menukaart visualiseren en een print stylesheet in elkaar zetten. Door dit vak hoop ik beter te worden met CSS, met bijvoorbeeld selectoren clip-paths en animaties etc. [Beoordelingsformulier](https://rickgroot.github.io/css-to-the-rescue-2021/docs/beoordeling/beoordelingsformulier.html) van deze course.

## Live link
[Check hier de site](https://rickgroot.github.io/css-to-the-rescue-2021/menu.html)

# Week 2
## Interaction
In deze week ben ik aan de gang gegaan met interaction. Hiervoor heb ik veel gebruik gemaakt van de **:target** selector. Wanneer je via een link naar een bepaalde id in je HTML gaat, kan je het gelinkte blok stijlenn met de :target. Op deze mannier is het mogelijk om een bepaald stuk tekst te highlighten wanneer je daar naartoe navigeert. In mijn geval gebruik ik deze selector om alles wat niet getarget wordt weg te halen. Op deze manier kan ik een werkende navigatie maken met pure CSS.

## Layout
De layout doe ik met behulp van **display: flex** en **display: grid**. Alle artiklen met gerechten zet ik door middel van flex naast elkaar en laat ik wrappen naar een volgende kolom. Ik heb dit met flex gedaan omdat je op die manier makkelijker een responsive layout kan maken zonder media queries. Vervolgens heb ik in de articles een grid toegepast. Deze hoeven minder responsive te zijn omdat de articles van zichzelf al klein zijn. Op deze manier kan ik een simpel grid toepassen waarmee alles op een nette manier uitgelijnd kan worden.

## Banners
Ook ben ik banners gaan maken voor de categorieën. Door de banners heeft de menukaart wat meer kleur en ziet het er minder saai uit. De banners heb ik gemaakt door middel van **::before** en **::after**. Ik heb de pseudo elementen absoluut gepositioneerd, en net buiten het blok met een z-index van -1. Op deze manier staan de blokken naast en onder de container. Daarna ben ik doorm middel van **clip-path** een vorm gaan maken. Omdat shadows niet goed werken op clip-paths heb ik het hoofd element een border gegeven. Op die manier is er toch nog een diepte effect.

# Week 1
## Kennismaking
Deze week ben ik begonnen met een kennismaking opdracht. Hierbij moest het team onderzoek doen naar een specifieke techniek/onderwerp. Mijn team had als onderwerp *effecten*. Hieronder vallen bijvoorbeeld blend-modes, clip-paths en filters. Binnen deze onderwerpen ben ik vooral gaan kijken naar de blend-modes en filters.

[Live preview van kennismaking](https://rickgroot.github.io/css-to-the-rescue-2021/docs/kennismaking/test.html)


### Blend-Modes
Blend modes zijn ook in andere programma's te vinden en zijn handig om verschillende afbeeldingen met elkaar te blenden. Photoshop heeft ook blend-modes, en deze zijn vergelijkbaar met de CSS blend-modes. Zo is het mogelijk om verschillen in afbeeldingen te highlighten of om een bepaald patroon of kleur in een afbeelding door te drukken. De CSS attributen voor blend-modes zijn **background-blend-mode:** (voor background images en kleuren)**;** en **mix-blend-mode:** (voor 2 elementen)**;**. Dit is een lijst van de CSS blend-Modes die beschikbaar zijn:
* color
* color-burn
* color-dodge
* darken
* lighten
* overlay
* screen
* multiply
* difference
* exclusion
* soft-light
* hard-light
* hue
* saturation
* luminosity
* normal

### Filters
Filers zijn handig toe te passen op afbeeldingen. Normaal pas je wel eens wat instellingen aan als je een afbeelding op instagram zet. Dan maak je de foto bijvoorbeeld iets lichter of pas je de temeratuur iets aan. Deze instellingen heb je ook in CSS met het **filter: ;** attribuut. Dit is een lijst van de filters die te gebruiken zijn:
* blur()
* brightness()
* contrast()
* drop-shadow()
* grayscale()
* hue-rotate()
* invert()
* opacity()
* saturate()
* sepia()

Filters zijn opvolgbaar, en je kan ze dus achter elkaar neerzetten. Dit scheelt ruimte in je code en ziet er als volgt uit: **filter: contrast(120%) hue-rotate(15deg) brightness(0.9);**

#### Clip-Paths
Ook heb je in CSS clip paths. Hier zijn handige generators voor te vinden online, zodat je zelf niet alle punten hoeft neer te zetten. In een clip path kan een afbeelding geplaatst worden. Deze afbeelding krijgt vervolgens de vorm van de clip-path, dit kan een leuk effect zijn voor bijvoorbeeld parallax scrolling of een wondow effect. De documentatio is als volgende:
```css
.container {
    clip-path: polygon(
		20% 0%,
		0% 20%,
		30% 50%,
		0% 80%,
		20% 100%,
		50% 70%,
		80% 100%,
		100% 80%,
		70% 50%,
		100% 20%,
		80% 0%,
		50% 30%
	); /* clip path of a cross */
}
```

## Start aan eindopdracht
### Contexten en restricties
na de kennismaking ben ik gaan brainstormen over mijn concept. Al snel wist ik dat ik de menu kaart ga vormgeven, en dat ik dit ga doen met **2 kleuren**, **responsive zonder media-queries** en een **print- stylesheet**. De twee kleuren vind ik zelf een leuke uitdaging, en zie ik veel kansen in het gebruiken van blend-modes en filters. Responsive zonder media-queries is een uitdaging waarbij ik veel ga leren, omdat er veel mogelijkheden zijn voor responsive design waar ik niet vanaf weet. De print stylesheet heb ik gekozen omdat ik dit een interessant element vind om meer over te weten te komen, en daarbij past het ook goed bij het onderwerp.

### Concept
Mijn vormgeving ga ik baseren op de stijl van een krijtbord. Hiervoor heb ik gekozen omdat je vaak bij restaurants buiten een krijtbord ziet staan, en het dus goed bij een restaurant style past. Daarbij geeft het ook heel veel uitdaging om het met css te maken, omdat het niet allemaal rechttoe rechtaan is in de stijl van  een krijtbord. Alles is net even anders en dit geeft mij mogelijkheden om te experimenteren met verschillende technieken. Daarnaast lijkt het mij leuk om mezelf uit te dagen om een origineel statisch voorwerp dynamischer te maken en interactief te maken door de mogelijkheden die CSS te bieden heeft.