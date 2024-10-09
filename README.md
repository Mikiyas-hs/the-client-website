# The Client - Website

Ontwerp en maak een website voor een opdrachtgever en bespreek het resultaat tijdens de Sprint Review.

De instructie van deze leertaak staan in de [INSTRUCTIONS](https://github.com/fdnd-task/the-client-website/blob/main/docs/INSTRUCTIONS.md)



## Inhoudsopgave Readme

  * [Beschrijving](#beschrijving)
  * [Kenmerken](#kenmerken)
  * [Bronnen](#bronnen)
  * [Licentie](#licentie)

## Beschrijving
<!-- In de Beschrijving staat hoe je project er uit ziet, hoe het werkt en wat je er mee kan. -->
<!-- Voeg een mooie poster visual toe 📸 -->
<!-- Voeg een link toe naar Github Pages 🌐-->

## Kenmerken
<!-- Bij Kenmerken staat welke technieken zijn gebruikt en hoe. Wat is de HTML structuur? Wat zijn de belangrijkste dingen in CSS? Wat is er met Javascript gedaan en hoe? Misschien heb je een framwork of library gebruikt? -->



## Licentie

This project is licensed under the terms of the [MIT license](./LICENSE).


Korte uitleg over de opdracht:

Intro 
- Deze sprint ging ik werken aan een webpage voor redpers. de bedoeling van deze opdracht was dat wij een nieuw design opgestuurd kregen en dat we daarmee aan de slag gingen door de website te gaan coderen dmv html/css en javascript. het doel was dat we het nieuwe design gingen waarmaken en dat de website responsive zou zijn voor zowel desktop als telefoon. https://mikiyas-hs.github.io/the-client-website/

Beschrijving 
- mijn project lijkt precies op het design die mij werd opgestuurd alleen. het enige wat mijn project nog niet heeft ten opzichte van de het design is de footer,doneer gedeelte en over de artiest voor de rest is de website identiek aan het design die ons werd opgestuurd 

- wat je met de pagina kunt doen is artikelen van auteurs lezen en uiteindelijk ook meer over hun te weten te komen je kan uiteindelijk ook geld doneren aan redpers en kennis maken met andere artikelen hierdoor maak je automatisch ook kennis met andere auteurs 
<img src="/images/Schermafbeelding 2024-10-10 002929.png">
<img src="/images/Schermafbeelding 2024-10-10 002412.png">
<img src="/images/Schermafbeelding 2024-10-10 002946.png">
<img src="/images/Schermafbeelding 2024-10-10 003139.png">

Kenmerken 
- de html is opgebouwd met semantische elementen zoals header, nav, main en article in de header gebruik ik een input van het type checkbox met het Id menu-toggle om een klikbare toggle te creeeren voor de navigatie. Deze checkbox word gekoppeld zoals je kunt zien met een label dat als een hamburger-menu wordt weergegeven door drie span-elementen die vormen dan die 3 strepen onder elkaar waardoor je een hamburger menu kunt zien en die elementen zitten binnen de menu-button
<label for="menu-toggle" class="menu-button">
                <span></span>
                <span></span>
                <span></span>
            </label>

in het main gedeelte van de HTML plaats ik het belangrijkste artikel, dat een titel heeft in een H1-element en verschillende paragrafen in een p-elementen. Er is ook een afbeelding met de class "bloemetje", die wordt gepositioneerd met css De knoppen onder het artikel (bijv voor het beluisteren van de artikel) zijn html button-elementen:
 <button>Artikel beluisteren</button>
        <button class="opslaan">opsln</button>
        <button class="verzenden">vrzn</button>
        <button class="translate">trnsl</button>


- met css heb ik een aantal custom fonts gebruikt die we opgestuurd kregen zoals tiempos die ik via @font-face in de Css heb ingeladen

@font-face {
    font-family: tiempos;
    font-weight: 700;
    src: url(../fonts/TiemposHeadline-Bold.otf) format('opentype');
}
@font-face {
    font-family: tiempos;
    font-weight: 400;
    src: url(../fonts/TiemposText-Regular.otf) format('opentype');
}
@font-face {
    font-family: tiempos;
    font-weight: 400; 
    font-style: italic;
    src: url(../fonts/TiemposText-RegularItalic.otf) format('opentype');
}

in het header gedeelte gebruikte ik flexbox om de elementen te centreren. Dit wordt gedaan met de display: flex en justify-content: center:

header {
    display: flex;
    justify-content: center;
    padding: 10px;
    background-color: #ffffff;
    max-width: 100%;
    height: 50px;
    border: 1px;
    position: relative;
    z-index: 1;
}

voor het menu is er een checkbox toegepast, waarbij de navigatie wordt weergegeven of verborgen afhankelijk van of de checkbox (#menu-toggle) is aangevinkt. Dit wordt in de Css gedaan

header:has(input:checked) {
    nav.menu {
        display: block;
    }
}

het menu zelf is verborgen met display: none, maar wanneer de checkbox is aangevinkt, wordt dit aangepast naar de display: block 

De knoppen voor acties zoals opslaan, verzenden en translate hebben specifieke klassen zoals .opslaan en .verzenden ze krijgen een eenvoudige styling met een licht transparante achtergrondkleur afgeronde hoeken 
.opslaan{
    display: inline-block;
    background-color: rgba(133, 154, 162, 0.227);
    box-shadow: none;
    border: none;
    color: rgb(124, 114, 114);
    width: 45px;
    padding: 14px 5px;
    font-size: 16px;
    cursor: pointer;
    text-align: center;
    border-radius: 3%;
    margin-top: 30px;
    margin-left: 45px; 
}

 tijdens dit project heb ik me gehouden aan de werkmethode mobile first waardoor ik dus als eerst was begonnen met de site maken voor op de telefoon de volgende stap zou dan zijn om het voor op de desktop toegankelijk te maken 

 ik heb in dit project (nog) geen gebruik gemaakt van javascript wat betekent dat het project puur op html en css gebaseerd is de reden dat ik dit heb gedaan is omdat javascript ervoor kan zorgen dat een site langzamer laad en moeilijker te onderhouden is en wat lastiger toegankelijk kan zijn voor alle gebruikers en apparaten en om dit te voorkomen wilde ik zoveel mogelijk html en css gaan gebruiken in dit project 


de bronnen die ik voor dit project heb gebruikt zijn:
https://stackoverflow.com/questions/48207583/spacing-between-text-with-line-height 
https://developer.mozilla.org/en-US/docs/Web/CSS/box-shadow
https://reintech.io/blog/creating-responsive-hamburger-menu-button-with-css