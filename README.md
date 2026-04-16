# Performance Audit 

Doe een Performance audit op een bestaande website uit je eigen omgeving en rapporteer daarover.

De instructies van deze opdracht staan in [INSTRUCTIONS](https://github.com/fdnd-task/performance-audit/blob/main/docs/INSTRUCTIONS.md).


## ZARA
Zara.nl is de Nederlandse webshop van het internationale modebedrijf Zara. Op de website kunnen bezoekers kleding, schoenen en accessoires bekijken en bestellen. De site bestaat uit grote sfeervolle foto's en video's, wat de website visueel aantrekkelijk maakt maar ook zwaar om te laden.

### Testresultaten samengevat
De website scoort slecht op performance op zowel mobiel als desktop. De grootste problemen zitten in de hoeveelheid JavaScript, grote afbeeldingen en externe scripts van derde partijen die de pagina vertragen.

* Lighthouse Mobiel gaf een score van 28 uit 100. De grootste afbeelding op de pagina laadde pas na 38 seconden, wat extreem slecht is. De pagina was meer dan 21 seconden geblokkeerd en reageerde niet op klikken of scrollen.
* Lighthouse Desktop gaf een score van 26 uit 100. De tijden waren veel beter dan op mobiel, maar de score bleef laag door dezelfde onderliggende problemen. De grootste afbeelding laadde hier in 4.8 seconden.
* PageSpeed Insights meet echte gebruikers in plaats van een gesimuleerde test. Daaruit bleek dat de werkelijke ervaring beter is dan Lighthouse liet zien. Toch slaagde de site niet voor de officiële Site-vitaliteit beoordeling op zowel mobiel als desktop. Het grootste struikelblok was de INP op mobiel van 527 ms, wat betekent dat de pagina traag reageert als je ergens op klikt.

<img width="1000" height="450" alt="image" src="https://github.com/user-attachments/assets/f20ff935-f844-4654-a37d-985cc7c6f37e" />
<img width="1000" height="450" alt="image" src="https://github.com/user-attachments/assets/bcc5372c-5bc0-4350-ab66-85cf298aefaa" />
<img width="1100" height="370" alt="image" src="https://github.com/user-attachments/assets/751a81c8-97db-4a10-9eb9-5c10548617e0" />
<img width="1100" height="370" alt="image" src="https://github.com/user-attachments/assets/f53c1e6f-7d48-4556-83c6-0a221ea78aea" />




### Belangrijkste problemen
De site laadt te veel JavaScript dat niet eens gebruikt wordt. Externe scripts van advertentie- en analysebedrijven blokkeren de pagina. Afbeeldingen worden niet in moderne formaten aangeboden en foto's die je nog niet ziet worden al meteen ingeladen. Tekstbestanden worden niet gecomprimeerd verstuurd.

### Wat gaat goed
De server zelf reageert snel (0.7 seconden). De website is veilig via HTTPS. Op desktop verspringen er weinig elementen tijdens het laden. De basisopbouw van de site is technisch in orde.

### conclusie
Zara.nl scoort slecht op performance. Op mobiel haalt de site een score van 28 en op desktop 26 uit 100. De officiële Google Core Web Vitals beoordeling is op beide apparaten niet geslaagd. De grootste problemen zijn de trage laadtijd van afbeeldingen, te veel JavaScript en externe scripts die de pagina vertragen.



## Licentie

This project is licensed under the terms of the [MIT license](./LICENSE).
