# Rapportage webtoegankelijkheid-test voor Beyco
*Dit document is een template voor een webtoegankelijkheid-test volgens de Web Content Accessibility Guidelines (WCAG). Een consistente rapportage helpt bij het uitvoeren van een evaluatie en zorgt er voor dat verschilelnde tests kunnen worden vergeleken.*

Datum webtoegankelijkheid-test: 28-10-2021

Webtoegankelijkheid-test uitgevoerd door: Daphne Zwuup

## Inhoudsopgave

  * [Samenvatting](#samenvatting)
  * [Achtergrond bij de evaluatie](#achtergrond-bij-de-evaluatie)
  * [Afbakening](#afbakening)
  * [Beoordelaars](#beoordelaars)
  * [Beoordelingsproces](#beoordelingsproces)
  * [Testresultaten en aanbevelingen](#testresultaten-en-aanbevelingen)
  * [Referenties](#referenties)
  * [Bijlagen](#bijlagen)
  * [Licentie](#licentie)

## Samenvatting

Dit rapport beschrijft in hoeverre de website beyco.nl overeenstemt met de Web Content Accessibility Guidelines (WCAG) van het W3C. Na de achtergrondinformatie en afbakening van de test worden beoordelaars, beoordelingsproces en testresulltaten beschreven.

Conslusie van deze test luidt dat de Beyco website niet voldoet de WCAG 2.1, op niveau AA. Gedetailleerde resultaten en aanbevelingen zijn verderop in dit document beschikbaar en in de referenties vindt u bronnen voor eventuele vervolgstudie. Wij stellen feedback op deze evaluatie zeer op prijs.

## Achtergrond bij de evaluatie

De webtoegankelijkheid-test vereist een combinatie van semi-geautomatiseerde en handmatig uitgevoerde evaluatie tools door een ervaren beoordelaar. De beoordelingsresultaten in dit rapport zijn gebaseerd op een beoordeling welke is uitgevoerd op 28-10-2021. De website kan ondertussen aangepast zijn.

## Afbakening

beyco.nl

Beyco is een platform waarbij je je koffie kan kopen en verkopen.

URLs die mee zijn genomen in de beoordeling:

www.beyco.nl

## Beoordelaars

Daphne Zwuup
Student
daphne.zwuup@hva.nl
Nederlands

## Beoordelingsproces

Deze beoordelings is uitgevoerd op WCAG 2.1 Niveau AA

De tools die zijn gebruikt voor deze beoordeling zijn de volgende:

- [A11Y Checklist](https://www.a11yproject.com/checklist/)
- [WCAG Guidelines Overview](https://www.w3.org/WAI/standards-guidelines/wcag/)

## Testresultaten en aanbevelingen

De huidige website van beyco voldoet niet nivea AA van de WCAG 2.1. Om deze score toch te behalen zijn er een paar aanbevelingen.
- Voeg voor knoppen met zichtbare labels tekstinhoud toe aan het knop element. Maak van het label een duidelijke call-to-action. Bijvoorbeeld: <button>Menu</button>
Gebruik voor knoppen zonder zichtbare labels, zoals pictogram knoppen, het attribuut aria-label om de actie duidelijk te beschrijven voor iedereen die een ondersteunende technologie gebruikt.
- Net als bij knoppen, ontlenen links hun toegankelijke naam voornamelijk aan hun tekstinhoud. Vermijd invulwoorden zoals "Hier" of "Lees meer;" plaats in plaats daarvan de meest betekenisvolle tekst in de link zelf. Gebruik voor links met pictogram knoppen, het attribuut aria-label om de actie duidelijk te beschrijven voor iedereen die een ondersteunende technologie gebruikt. Dus voor de gefaalde elementen kan dus een aria-label gebruikt worden, omdat dat sociale media pictogrammen zijn.
- Verwijder de mogelijkheid om te focussen op elementen die momenteel niet bedoeld zijn om te worden ontdekt. Dit omvat zaken als inactieve vervolg keuzemenu's, navigatie buiten het scherm of modals.
- alt-attributen (alt-tekst) geven een beschrijving van een afbeelding voor mensen die ze mogelijk niet kunnen bekijken. Wanneer een alt-attribuut niet aanwezig is op een afbeelding, kan een schermlezer in plaats daarvan de bestandsnaam en het pad van de afbeelding aankondigen. Hierdoor wordt de inhoud van de afbeelding niet gecommuniceerd. Zorg er daarom altijd voor dat de alt attribuut in jullie afbeeldingen wordt gebruikt.

### Sterke punten
- De lees level in deze pagina is 11.17. Dus de lees level van de website is goed.
- Er is een lang attribuut gebruikt.
- De viewport van de website is niet uitgeschakeld.

### Ontoegankelijke punten
- De inhoud van een button is neit uniek en beschrijvend.
- Social icons hebben geen goede benaming voor de focus.
- Sommige elementen hebben geen zichtbare focusstijl
- Sommige headings hebben geen logische volgorde.

### Checklist 

##### Content
- Schrijf inhoud op lees level 8.\
De lees level in deze pagina is 11.17. Dus de lees level van de website is goed.
- Zorg ervoor dat de inhoud van de button, a en label elementen uniek en beschrijvend is.\
```html
<button type="button" class="menu-icon-container">
```
Daarom is de code die hierboven te zien is gefaald.
- Gebruik links uitgelijnde tekst voor links-naar-rechts (LTR)-talen en rechts uitgelijnde tekst voor rechts-naar-links (RTL)-talen.\
De koppen en bodytekst zijn in de css center aligned. Alleen de tekst in de footer en in de menu is standaard left-aligned.

##### Global code
- Valideer uw HTML.\
De website had alleen maar een waarschuwing.\
De waarschuwing kan je nog een keer zien op deze link in de html validator: https://validator.w3.org/nu/?doc=https%3A%2F%2Ftest.beyco.chippr.dev%2F
- Gebruik een lang attribuut op het html-element.\
Dit is de code van het lang attribuut van Beyco:
```html
<html lang="en-us"></html>
```
De code voor de lang ziet er goed uit.
- Geef elke pagina of weergave een unieke titel.\
De titel van de homepagina is goed vernoemd. De titel van de homepagina is: Worldwide Coffee Trading Platform - Beyco.
- Zorg ervoor dat de viewport zoom niet is uitgeschakeld.\
De viewport van de website is niet uitgeschakeld.\
Hier is de code van de viewport:
```html
<meta name="viewport" content="width=device-width,initial-scale=1">
```
- Gebruik oriëntatiepunten om belangrijke inhoudsgebieden aan te geven.\
De homepagina heeft geen main met sections daarin. Ze hebben in plaats daarvan alleen divs gebruikt. In plaats van de main hebben ze een div gebruikt met de id root en daarin andere divs gezet. 

Ze hebben wel een header met daarin een nav en onderin een footer.
- Zorg voor een lineaire contentstroom.\
De homepagina heeft geen tabindex. Dus dit is niet bij hun van toepassing.
- Vermijd het gebruik van het autofocus attribute.\
Beyco heeft geen autofocus gebruikt. Dus dit is niet bij hun van toepassing.
- Verwijder title attribute tooltips.\
Beyco heeft geen extra titles. Dus dit is niet bij hun van toepassing.

##### Keyboard
- Zorg ervoor dat er een zichtbare focusstijl is voor interactieve elementen waarnaar wordt genavigeerd via toetsenbordinvoer.\
Search for coffees figures/cards zijn onduidelijk voor screenreaders. Het heeft teveel tekst waardoor het moeilijk te begrijpen op een screenreader.

Social icons hebben geen goede benaming voor de focus.\
Hier zijn de gefaalde elementen:
```html
<a class="interactive interactive-link layout layout-row gap-small align-cross-center" href="/">
<a href="https://www.instagram.com/beyco.nl/">
<a href="https://www.linkedin.com/company/beyco-nl/">
```
- Controleer of de focusvolgorde van het toetsenbord overeenkomt met de visuele lay-out.\
Je kan makkelijk de tab toets op het toetsenbord gebruiken om naar interactieve elementen te gaan. Alle elementen zitten in de juiste volgorde.
##### Images
- Zorg ervoor dat alle img elementen een alt attribuut hebben.\
Beyco heeft geen alt in de foto van de map.\
Code van de afbeelding zonder alt:
```html
<img src="/static/media/fake-map.2863d4ee.png" alt="" width="100%">
```

##### Headings
- Gebruik heading elementen om inhoud te introduceren.\
De homepagina heeft headings.
- Gebruik slechts één h1 element per pagina of weergave.\
Er zit alleen maar een h1 element op de homepagina.
- Heading elementen moeten in een logische volgorde worden geschreven.\
De headings hebben geen logische volgorde. De kleine kopjes in de "How does it work?" gedeelte zijn h4 in plaats van h3.

##### Lists
n.v.t.
##### Controls
- Gebruik het a element voor links.\
De links van de homepagina hebben allemaal een a href.
- Zorg ervoor dat links herkenbaar zijn als links.\
De links van Beyco hebben een grijze rand wanneer ze gefocused zijn.
- Zorg ervoor dat besturingselementen :focus states hebben.\
De links hebben allemaal :focus states. Het is alleen dat de figures van het gedeelte Search for coffees geen focus stijl hebben.
- Gebruik het button element voor knoppen.\
De knoppen hebben een button element.
- Zorg voor een skip link en zorg ervoor dat deze zichtbaar is wanneer gefocust.\
De homepagina heeft geen skip content link.
- Identificeer links die openen in een nieuw tabblad of venster.\
De homepagina heeft geen links die naar een nieuw tabblad of venster gaan.

##### Tables
n.v.t.
##### Forms

##### Media

##### Video

##### Audio

##### Appearance

##### Animation

##### Color contrast

##### Mobile and touch

## Referenties

Referenties welke gebruikt zijn bij de webtoegankelijkheid-test. Deze referenties zijn allen in het Engels:

- [Overzicht en introductie van de Web Content Accessibility Guidelines (WCAG)](https://www.w3.org/WAI/intro/wcag)
- [De complete Web Content Accessibility Guidelines 2.1 (WCAG)](https://www.w3.org/TR/WCAG21/)
- [Technieken voor WCAG 2.1](https://www.w3.org/WAI/WCAG21/Techniques/)
- [Bronnen voor beoordeling van webtoegankelijkheidsevaluatie ](http://www.w3.org/WAI/eval/)
- [Tools lijst voor semi-geautomatiseerde beoordeling van webtoegankelijkheid](https://www.w3.org/WAI/ER/tools/)
- [Informatie over het gebruik van gecombineerde expertise voor het evalueren van webtoegankelijkheid](https://www.w3.org/WAI/eval/reviewteams)
- [A11Y Project Checklist](https://www.a11yproject.com/checklist/)

{Vul aan waar nodig, haal weg wat niet relevant is}

## Bijlagen

{Geef een opsomming van de bijlagen, zoals links naar rapportages, screenshots en uitleg in de Wiki}


[Einde van het template]

## Licentie

![GNU GPL V3](https://www.gnu.org/graphics/gplv3-127x51.png)

This work is licensed under [GNU GPLv3](./LICENSE).
