## goals 3-4
1. Load data from zoek.bekendmakingen
2. Load data from waaroverheid
3. finish pre-mature version of naive bayes
4. finish pre-mature version of SVM
5. finish pre-mature version of W2V

## successes
1. although I did not use their API but instead used data from other trainees 
2. Dit leek ook vandaag al te lukken, voor nu maakte ik een gigantische csv met organisatie, catergorie van het document (que soort), de tekst en de titel. Alleen op een gegeven moment krijg ik een server response van 500, dus ik overleg morgen met Breyten over wat dat kan zijn.
3. 9 & 16 percent accuracy, de simpele scikit gebruikt. Het is wel een beetje vreemd dat het zo slecht werkt, aangezien er bij de 16 procent maar een categorie of 20 is. Daar moet ik even naar kijken.
4. 6 & 9 percent accuracy, zelfde verhaal als bij 3.
5. Word2Vec is gemaakt op basis van de data van andere stagiars, lijkt redelijk te werken, maar kan meer testdata gebruiken. Later kan de Word2Vec ook getraind worden met de data van 2 erbij.

## challenges
- De data van de gemeentes is best vies, dus die goed schoonmaken is belangrijk
- Het is nog steeds niet helemaal duidelijk hoe CNN werken op lange zinnen, ook dat moet ik uitwerken. Voor nu heb ik twee oplossingen hiervoor. 1. documenten opslitsen, de zinnen 1 voor 1 gebruiken, en als het ware de meeste stemmen gelden. 2. het op de titels/eerste regels toepassen.

## wat is fijn om af te hebben aan het einde van de week
- API data inladen
- Word2Vec trainen op alle data
- Mogelijkheid creeren meer dat op te halen van bekendmakingen
- Naive Bayes/SVM omhoog krijgen
- CNN methodes uitwerken zodat ik volgende week met Maarten kan brainstormen
