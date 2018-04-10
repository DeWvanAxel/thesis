### Voortgang
1. Gestage verbetering van SGD/SVM en Naive Bayes .
2. Ik heb een nieuwe introductie geschreven
3. CNN implementie gestolen van deze blog: https://richliao.github.io/supervised/classification/2016/11/26/textclassifier-convolutional/, en die is weer gemodelleerd naar dit paper: https://www.cs.cmu.edu/~diyiy/docs/naacl16.pdf. Grotendeels uitgetraind, verbeterd nog wel op training, maar niet op test.
4. Ik ben bezig geweest met een overzicht van de data. Los van de langere teksten hebben we ook een aantal hele korte van minder dan 5 woorden. Dat schrappen? Verder is de vraag of ik genoeg data heb.
5. GPU training lukt me niet voor elkaar te krijgen
6. Scrapen van gemeentes lukt niet door een fout van OSF, daar werken ze aan.

| Acurracy    | amount_topics=18 | amount_topics=112 |
|-------------|------------------|-------------------|
| CNN            | 0.74                 |   0.52                 |
| Naive Bayes |  0.43                |   0.19                  |
| SGD\SVM    |   0.82               |   0.77                  |


### Agenda
1. De baselines lijken redelijk te werken. Hoeveel werk is daar nog aan nodig? Dit is zowel hoeveel tijd ik moet steken in het uitleggen van hun werking in mijn thesis als hoeveel parameter optimalisatie ik moet doen.
2. De nieuwe introductie bespreken, te vinden in mijn thesis\main.pdf
3. CNN doet het nu redelijk, maar het moet de baselines gaan verslaan. Daarvoor twijfel ik over de beste aanpak om dat te doen: Alleen eerste deel van tekst gebruiken, paragraph2vec, net maken van meerdere lagen, per zin voorspellen en dan meeste stemmen gelden. Graag hierover brainstormen
4. Genoeg data? Deel van de data wegnemen of verpest dat het doel van wat ik doe?
5. Is er iemand die ik kan vragen voor GPU-training
