Verbeteringen

Inhoudelijk
- Contactgegevens gemeente en Verkiezingswebsite gemeente lijken me generiek.
- stembureau nummer: iets zeggen over EML nummer
- tijden velden: date time velden html 
- locatie via PDOK locatie service?

 
Algemeen
- Nederlands en Engels wordt doorelkaar gebruikt in naming van variabelen.
- Uitzonderingen specfieke verkiezingen in code in kaart brengen.
- Generiek maken verkiezings datum (en verwijdingen naar vorige verkiezingen?)
- Google tag maanager eruit?



Bestanden structuur
- Docker container start directory nu zelfde als root repository, daardoor loopt eea door elkaar.
- templates -> gemeente login in eigen subdirectory? bv `gemeente/`
- gemeente paginas eigen base.html
- include bestanden eigen directory
- naamgeving bestanden: alles nederlands.


Productie/Docker
- Apps niet opstarten als root in docker containers
- Scripts e.d. niet meer inladen via een cdn, alles zelf hosten.


Grote wijzigngen:
- CBS data eruit en dynamisch ophalen via PDOK locatie server: https://api.pdok.nl/bzk/locatieserver/search/v3_1/ui/#/Locatieserver/free


CSS:
- Vervang $color e.d. uit _variables.scss voor echte css variable var(--color)
- split css nodig voor main site van css nodig voor invoer gegevens.

Variabelen:
- naam verkiezing
- datum verkiezing
- naam vorige verkiezingen
- uiterste aanlever datum stembureaus
