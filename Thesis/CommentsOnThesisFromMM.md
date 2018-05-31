## comments MM 29 mei, hfd 1,2,3

1. Schrijf je abstract nu ook maar. Goeie titel hoor!
2. gebruik \url{http://zoek.openraadsinformatie.nl/}, dan is het klikbaar.
3. Zet het een sin de ACM 2 columns stijl en kijk eens op hoeveel paginas je zit. Ik denk dat je nog heel wat ruimte hebt. 

#### Algemeen
Dit is een mooi begin en de dingen die erin horen staan er ook in.  Ik denk dat je het moeilijk vond om een lezer in gedachten te nemen, en nu is het volgens mij voor niemand echt gelukt om op haar niveau te schrijven omdat je steeds wisselt. Dat is jammer. Zekere in sectie 1 kan je best wat meer uitleggen, ook zonderdat het stom wordt voor experts. In sectie 2 beschrijf je dingen oppervlakkig. Je zou hier eerst op een hoog niveau het onderscheid tussen lexicale en neurale/semantische methoden kunnen schetsen en allicht iets zggen over "vpcabulary gap" en waarom je denkt dat dat bij jou speelt. Daarna raad ik je ook aan om de state of the art te besprken en resultaten te laten zien op vergelijkbare datasets. Dat plaatst jouw bevindingen dan in perspectief. 

Noem ook de beperking van domain adaptatie (dat je toch nog best een hoop trainingsdata nodig hebt, die er nu dus niet is).



#### sec 1

* eerste paragraaf. 
	* wees maar best wat specifieker hoor. Wat zijn dat voor labels, wat beschriven ze? En zeg iets over het automatisch labellen, want dat doe je nu niet eens. Gebruik allicht het woord thesaurus. Je zou hier Eurovoc kunne noemen, of een andere NL thesaurus die voor politeiek/beleids documenten gebrukt wordt. 
* de eerste par schetst je probleem. In de tweede geef je je oplossing, maardat gaat wel heel snel. Doe het wat rsutiger, en schets de moeilijkheid van je oplossing. Ik zou ook even kort uitleggen hoe zo'n classifier nou werkt (dat je dat trained op voorbeelden), en waarom het niet evident is dat die dan ook gewoon werkt op die gemeente data. 
* l86 _relatable_???
* Dus al met al, je mag hier best wat meer uitleggen. Denk bijv aan de eerste 5 minuten van je presentatie waarin je ook wilt dat je familie het kan volgen, maar waarin je toch echt uitlegt wat er gaat gebeuren. OOk voor Tom en OSF is dit van belang. Dat ze gaan inzien hoe lastig dit is, en dat ML echt niet zomaar hoepsakee tot een oplossing leidt.

#### sec 2

**algemeen** De sectie legt meer de technieken uit dan dat het een overzicht geeft van wat er op de matkt is en hoe goed dat dan werkt op vergelijkbare gevallen. Dat laatste is wel leuk om toe te voegen. Dat geeft dan echt related work. Dus behandel 1 of 2 studies die ook domein adaptatie doen en laat zien wat voor scores die dan vinden.  Je zou dit na je inleidende dingen kunnen doen en die subsectie "State of the art" kunnen noemen.

* _to show how this research relates
95 to it._ kan weg. Wees sowieso bewust als je feiten "motiveert". Vaak kan dat weg. Je hoeft zo'n sectie niet te verantwoorden. 
* Ik zou voordat je met 2.11 en 2.12 begint het onderscehid tussen lexicale methodes en methodes gebaseerd op "semantiek" duidelijk maken. 
* _limited set_ (101) _small_? of anders _finite_
* _its content._ (104) ik zou dan its features zeggen. Probeer te vermijden dat je steeds nieuwe termen gebruikt. Hou het dus heel puur en feitelijk.
* _To evaluate how well the classifiers can do this, a part of D is used as test data
106 which the models attempt to predict accurately _ (105) veranderdat deel vanaf _whcih_ en vertel nu juist hoe die evaluatie in zijn werk gaat (dat je dus het voorspelde label verglijkt met het echte label). 
* 109 weer zo'n bijzin die niets toevoegt: _, which is used to train
109 the classifiers._
* l130 je gebruikt een _logistic function_ niet de log, en een drempel, geen afronding.
* l141: je moet dan juist voor elk label een one vs rest classifier maken, niet "an"


### 2.1.2

* Begin met uit te leggen wat het idee is van die word embeddings. Ze worden zo geleerd dat de representaties van woorden die semantisch verwant zijn in de vector ruimte dicht bij elkaar liggen. 
* _multidimensional vectors_ ? low dimensional bedoel je denk ik.
* 189-194 leg dit beter uit. Je zinnen zijn ook niet grammaticaal.
* Kan je hier wat zeggen over de output layer? Dat zijn dan toch evenveel knopen als je klasses hebt, en ieder knoop krijgt een score? 

### Sec 3

* 3.1 geeft een goed inzicht in de data. Mooi! Ik zou in tabel 1 ook de mediaan aantal woorden en labels toevoegen. En zeker bij woorden geen decimalen! Onzin. Dus evenveel rijen en dan mean/median number fo words: 
* 292: omdat het multi-label si is de formule voor precisie en recall niet evident. Helemaal omdat het ook multiclass is, is dit best lastig. Dus geef die formules. 
* l304 Gebruik je TF-IDF, en zo ja, wat voor soort? Je gebruikt vast ook (standaard) instellingen over minimaal en maximaal aanal voorkomens, etc. je moet hier wel wat over zeggen, of zeggen dat je in de appendix de preciesie instellingen aan geeft. 
* l339 _blocks of length 200_ 200 wat? woorden?
* 338-347 Ik raak hier de kluts kwijt. Twerwijl dit nou juist jouw eigen toevoeging is! Neem dus rustig de tijd.
 
## Comments May 1

1. zet er regelnummers in
2. **Intro**
   * Zeg ook iets overde specifieke data set en het probleem vanuit OSF. Het is nu wel erg technisch
   * Ik zou er 2 setjes RQ's van maken. 1: zoals het nu is: hoe goed kan je die labels leren? en 2. over het generaliseren. 
   * In het laatste paragraafje "structure of this thesis" zou ik gewoon steeds iets schrijven als "In section 2 we discuss the most relevant related work", etc
3. Sectie 3.1
   * Wees specifiek over wat je exact hebt geextraheerd uit die kamerstukken. Geef bijvoorbeeld het schema. 
4. Wees consistent in je woordgebruik! Table 2 is een leuk voorbeeld: je gebruikt hier 3 verschillende woorden voor het zelfde concept! Label, topic categories. Zou de lezer dit begrijpen? En zo ja, approecieren?
5. Denk na of een tabel iets toevoegt> Kijk eens naar Tabel 3. Besteed liever meer aandacht aan de caption.
6. Table 5: druk de winnaar per kolom in bold af. Ik zou ook de macro F1 tonen. Maak in je caption duidelijk om welke tags (de detailed of juist niet) het gaat.
7. Bij Naive Bayes lijkt er iets mis gegaan. Dat kan toch niet zo verschillen?

   
   
