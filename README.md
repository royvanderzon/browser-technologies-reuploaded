# Funda Fork

In de Funda app zaten een aantal onhandige dingen zo is het voor blinden moeilijk om te navigeren. Daarom zijn er een aantal extra functionaliteiten toegevoegd. Deze voor gebruikers die soms in zwaarder weer zitten betreft hun browser.
Bijvoorbeeld de funcionaliteit van het toetsenbord wat nu nog meer wordt benut. Zo kon de gebruiker al veel functionaliteiten benutten met de pijltjestoetsen, letter n, letter m, en spatiebalk. Nu is dat uitgebreid met de esc toets voor het menu. Ook is de site geoptimaliseerd voor telefoon.
Daarnaast zijn kleur contrasten sterker gezet, title en alt teksten toegevoegd, en focus states bij de hover states.
Ook is er een noscript tag toegevoegd zodat mensen zonder javascript weten waarom de webapp niet werkt.

- esc key function
- colors changed
- add titles and alt texts
- no script tags added
- add :focus states

### Funda Progressive Enhancement todo list
- Google maps kaart contrast omdraaien
- Spraak gesproken navigeren met de tiles
- Swipe gestures over de tiles
- Extra toevoegbare controler (externe hardware)

De dingen in de hierbovengenoemde wishlist zijn moeilijk implementeerbare dingen (de meeste dan). Vooral de spraak gesproken navigeren. Hier zou je bijvoorbeeld aan kunnen haken bij een AI achtige API. Hier zal wel eerst onderzoek voor moeten worden gedaan. Wel zouden deze dingen de usabillity sterk vergroten. Zo kunnen (kleuren) blinde en slecht zienden gelijk zonder enige problemen gebruik maken van de functionaliteiten van de webapp. 

## Onderzoek JS

| Website | Bevindingen | Cijfer |
| ------------- |-------------| -----|
| Bol.com      	|  Kan nogsteeds besteld worden, sommige ontbrekende functionaliteiten			|  	6	|
| Mijn hva     	|  Werkt **niet**     	| 1   	|
| CMD moodle 	|     Werkt perfect  	|    10 	|
|    Conrad.nl 	|     Werkt **niet**, maar is aangegeven  	|     2	|
|    Mediamarkt.nl 	|      Werkt **niet** 	|  1   	|
|    Annefrank.org 	|      Werkt bijna goed 	|   7  	|
|    Gmail 	|     Werkt **niet** maar is aangegeven  	|    2 	|
|    fontawesome.io 	|      Werkt bijna goed 	|  7   	|
|    Ah.nl 	|      Werkt **niet** 	|    1 	|

## Onderzoek Internet connectie

| Website 		| 50 kb/s (clean) | No limit (clean) | Size (clean) | Size (cache) | Opmerking | Cijfer|
| ------------- |-------------| -------|-------|-------|-------|-------|
| Bol.com		| 12.09s | 1.13s | 1.1mb  | ~100kb | | 9 |
| Mijn hva		| 7.39s  | 763ms | ~550kb | ~15kb  | Bij 50 kb/s **kapot** | 3 |
| CMD moodle	| 56.15s | 1.17s | 494kb  | 79kb   | | 8 |
| Conrad.nl	| 	| 2.9m   | 1.39s | 1.2mb  | 54kb   | | 7 |
| Mediamarkt.nl	| 4.7m   | 1.38s | 2mb    | 85kb   | | 6.5 |
| Annefrank.org	| 3.5min | 1.7s  | 1.3mb  | 45kb   | | 7.5 |
| Gmail			| 16.42s | 1.56s | 752kb  | 624kb  | | 7 |
| fontawesome.io| 1.5s   | 1.79mb| 1mb    | 143kb  | | 7 |
| Ah.nl			| 22.26s | 468ms | 1mb    | 17kb   | | 7 |

## Conclusies

De meeste webshops doen het slecht. Echter heeft bol.com het goed gedaan. Daar kan je namelijk nogsteeds bestellen. Ook blijven cookies zonder javascript gewoon opgeslagen. Je ziet dat snelheid en javascript erg met elkaar in verband staat. Dit omdat ze allebei helpen het internet voor de gemiddelde gebruiker aangenamer te maken. Dit heeft betrekking tot iedereen! Daarom is het ook gek om te zien dat website's al AH, Gmail of mijn HVA niet meer bruikbaar zijn zonder deze middelen. Echter zijn hier wel oplossingen voor. Zo heeft Gmail een speciale webversie die bij veel slectere omstandigheden 100% blijft werken. Sommige websites geven het wel aan als er iets mis is met de verbinding of de javascript functionaliteit. Sommige websites zijn echter gemaakt om altijd onder alle omstandigheden te werken. Neem bijvoorbeeld Moodle. Die perfect werkt op trager internet, maar ook goed perfect werkt zonder javascript. **Oplossingen** voor traag internet zouden op diverse manier kunnen worden opgelost. Bijvoorbeeld door connectiesnelheid te meten en grote (onbelangrijke) content delen te skippen. Ook zouden voor webapps speciale HTML versies gemaakt kunnen worden zodat bepaalde informatie toch altijd gewonnen kan worden. Gmail waarschuwd zo bijvoorbeeld ook wanneer een connectie wegvalt. En probeert uit zichzelf opnieuw te verversen. 