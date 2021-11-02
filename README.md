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

{Samenvatting van testresultaten, bv. deze website {voldoet/ voldoet niet/ is dichtbij aan voldoen} aan de WCAG 2.1, op niveau A, AA of AAA.}

### Sterke punten
{Samenvatting van de de sterke punten ...}

### Ontoegankelijke punten
{Samenvatting van ontoegankelijke punten ...}

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
De koppen en bodytekst heeft Beyco in de css center aligned. Alleen de tekst in de footer en in de menu is standaard left-aligned.

##### Global code
- Valideer uw HTML.\
De website had alleen maar een waarschuwing.\
Dit wat de waarschuwing kan je hier zien:\

Warning: Consider adding a lang attribute to the html start tag to declare the language of this document.\
From line 1, column 16; to line 1, column 21\
type html><html><head>

##### Keyboard

##### Images

##### Headings

##### Lists

##### Controls

##### Tables

##### Forms

##### Media

##### Video

##### Audio

##### Appearance

##### Animation

##### Color contrast

##### Mobile and touch

Remove horizontal scrolling.
Op kleinere telefoons zoals Iphone 5 is er aan de rechterkant witruimte die zich over de hele lengte van de site verspreid.

Ensure sufficient space between interactive items in order to provide a scroll area.
Bij de sectie van "Search your coffees" is er niet genoeg ruimte voor de gebruiker om te scrollen. Het zou zo maar kunnen dat je perongeluk 1 van de bedrijven aanklikt waardor je weer terug moet gaan naar de vorige pagina.

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
