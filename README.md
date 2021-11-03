# Rapportage webtoegankelijkheid-test voor Beyco
![mockup](https://user-images.githubusercontent.com/69635977/140179208-d394447e-218a-4604-b1b9-6f5dc16f93c3.jpg)
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
- De inhoud van een button is niet uniek en beschrijvend.
- Social icons hebben geen goede benaming voor de focus.
- Sommige elementen hebben geen zichtbare focusstijl
- Sla geen heading levels over.

### Checklist 

#### Content
- **Use plain language and avoid figures of speech, idioms, and complicated metaphors.**  
  Het lees level moet level 8 zijn. De lees level in deze pagina is 11.17. Dus de lees level 
  van de website is goed.
- **Make sure that button, a, and label element content is unique and descriptive.**  
  Daarom is de code van deze button is gefaald: `<button type="button" class="menu-icon-container">`. De class is niet duidelijk genoeg.
- **Use left-aligned text for left-to-right (LTR) languages, and right-aligned text for right-to-left (RTL) languages.**  
  De koppen en bodytekst zijn in de css center aligned. Alleen de tekst in de footer en in de menu is standaard left-aligned.

#### Global code
- **Validate your HTML**  
  De website had alleen maar een waarschuwing. De waarschuwing kan je nog een keer zien op deze link in de html validator: https://validator.w3.org/nu/?doc=https%3A%2F%2Ftest.beyco.chippr.dev%2F
- **Use a lang attribute on the html element.**  
  De code voor de lang ziet er goed uit. Dit is de code van het lang attribuut van Beyco: <html lang="en-us"></html>.
- **Provide a unique title for each page or view.**  
  De titel van de homepagina is goed vernoemd. De titel van de homepagina is: Worldwide Coffee Trading Platform - Beyco.
- **Ensure that viewport zoom is not disabled.**  
  De viewport van de website is niet uitgeschakeld.
  Hier is de code van de viewport: <meta name="viewport" content="width=device-width,initial-scale=1">
- **Use landmark elements to indicate important content regions.**  
  De homepagina heeft geen main met sections daarin. Ze hebben in plaats daarvan alleen divs gebruikt. In plaats van de main hebben ze een div gebruikt met de id root en daarin andere divs gezet.

  Ze hebben wel een header met daarin een nav en onderin een footer.
- **Ensure a linear content flow.**  
  De homepagina heeft geen tabindex. Dus dit is niet bij hun van toepassing.
- **Avoid using the autofocus attribute.**  
  Beyco heeft geen autofocus gebruikt. Dus dit is niet bij hun van toepassing.
- **Remove title attribute tooltips.**  
  Beyco heeft geen extra titles. Dus dit is niet bij hun van toepassing.
  
#### Keyboard
- **Make sure there is a visible focus style for interactive elements that are navigated to via keyboard input.**  
  Search for coffees figures/cards zijn onduidelijk voor screenreaders. Het heeft teveel tekst waardoor het moeilijk te begrijpen op een screenreader.

  Social icons hebben geen goede benaming voor de focus.
  Hier zijn de gefaalde elementen:
```html
<a class="interactive interactive-link layout layout-row gap-small align-cross-center" href="/">
<a href="https://www.instagram.com/beyco.nl/">
<a href="https://www.linkedin.com/company/beyco-nl/">
```
- **Check to see that keyboard focus order matches the visual layout.**  
  Je kan makkelijk de tab toets op het toetsenbord gebruiken om naar interactieve elementen te gaan. Alle elementen zitten in de juiste volgorde.
  
#### Images
- **Make sure that all img elements have an alt attribute.**
  BijBeyco heeft geen alt in de foto van de map.
  Code van de afbeelding zonder alt:
```html
<img src="/static/media/fake-map.2863d4ee.png" alt="" width="100%">`
```

#### Headings
- **Use heading elements to introduce content.**
  De homepagina heeft headings.
- **Use only one h1 element per page or view.**
  Er zit alleen maar een h1 element op de homepagina.
- **Don't skip heading levels.**
  De kleine kopjes in de "How does it work?" gedeelte zijn h4 in plaats van h3.

#### Controls
- **Use the a element for links.**
  De links van de homepagina hebben allemaal een a href.
- **Ensure that controls have :focus states.**
  Alleen de social media links in de footer hebben geen focus state.
- **Use the button element for buttons.**
  De knoppen hebben een button element. Maar zijn niet duidelijk beschreven voor de screenreaders.
- **Provide a skip link and make sure that it is visible when focused.**
  De homepagina heeft geen skip content link.
- **De homepagina heeft geen links die naar een nieuw tabblad of venster gaan.**
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
Afbeelding van huidige acessibility
![Schermafbeelding 2021-10-28 214101](https://user-images.githubusercontent.com/69635977/140180222-15d4e284-8988-4897-8641-ecb5d0fda9c1.png)

## Licentie

![GNU GPL V3](https://www.gnu.org/graphics/gplv3-127x51.png)

This work is licensed under [GNU GPLv3](./LICENSE).
