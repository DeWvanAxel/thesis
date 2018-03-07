## Thesis design comments

* 2018-03-06
* Marx


### Overall
Leuk , nuttig en best ambitieus project wat heel goed binnen DS valt. 
Je ontwerp is goed beschreven en zal je goed kunne sturen. Ik stel wel voor dat je je RQ's nog wat verder uitdiept en opsplitst. Bijv, in je planning schrijf je dat je hoopt mee te gaan helpen met een implementatie van je werk op de site van OSF. Great! Maar waarom is er geen RQ die daarbij hoort? Die kan je makkelijk maken? Iets over het nut van de labels, en dan wat uitsplitsen. 
Ik zou ook een RQ toevoegen over het gebruik van de labels door de overheid. Sowieso is het leuk om wat EDA te doen op die labels, en in kaart te brengen hoe ze gebruikt worden. Je kunt dit dan ook als aparte RQ opnemen en dan heb je er ook wat aan. Hiermee maak je leuke plotjes en biedt inzicht.  

Dus probeer elk stapje van je proces/plan te koppelen aan een vraag/deelvraag zodat je goed ziet waarom je precies wat doet.


## overview
1. **Abstract**    ~~Nice and well written. However, it is not clear with WHAT you will label the documents, and why. ~~
2. **RQ's**  Good. Ik zou ze wel wat breder trekken: bijvoorbeeld niet neuraal vs neuraal. Dan kan je bijv ook SVM meenemen wat wat al wat beter werkt dan NB. Probleem is natuurlijk wel je evaluatie op de gemeente data. Want je hebt geen gouden data daar! 
	* Tobias kijkt naar transfer learning. Dat zou voor jou ook relevant kunen zijn. 
	* Een andere leuke en zeer gerelateerde vraag is om eens te kijken hoe taal/woordgebruik per label veranderd door de tijd. Als dat zo is geeft het al aan hoe lastig jouw taak is, want jij gaat ook nog eens naar een ander domein overschakelen. 
		* Dit is redelijk eenvoudig te onderzoeken (bijv je neemt maar een paar labels, en vergelijkt test/train op willekeurig gehusselde data met train op oude, test op nieuwe data).
3. **Related work**    Prima, maar je gaat hier wel erg op de methodes in, die kunnen beter naar de volgende sectie. Ik zou toch nog wat meer over multi-labels schrijven (want dat wil je doen), en ook over verschillende text clasificatie methodes. 
	* Het is goed dat je uitgebreid beschrijft hoe je de woordvectoren dan wilt gaan toepassen. Alleen zie ik nog niet hoe je die technieken die voor heel korte tekstjes zijn gemaakt (zinnen) nu gaat toepassen voor lange teksten. 
	* ~~Een deelvraag zou ook kunne zijn om juist minder data te gebruiken voor je classifier (bijv alleen de titel en eerste paragraaf).Vaak werkt dit zelfs beter.~~  Zie ook het artikel van Azerbonyad in ECIR over politieke tekst classificatie. 
4.  **Methodology** 
	 * Looks solid. 
	 * Voro de word vectoren kan je ook denken aan al bestaande vectoren voor het nederlands (heeft Google die niet ook?). Ik heb ook veel parlementaire data waarop je zou kunnen trainen. Hier geldt natuurlijk: hoe meer hoe beter.
	 * Kan je geen data dump van Breyten krijgen? Dan heb je alles bij elkaar! 
	 * Voro word2vec wordt meestal geen preprocessing gebrukt. Trowuens , lemmatizers maken best veel fouten op de gekke woorden in politieke docs! Misschien hoeft dat helemaal niet als je word2vec gebrukt! 
	 * Je zou toch prima op de Utrecht data set kunnen werken? Daar kan je je makkelijk beperken tot 1-topic docs (moties, vragen). Je bent daar toch ook geweest? Hebben ze niet meer data, en ook metadata? Of willen ze misschien helpen met labellen? Als je Utrecht data gebruikt kun je allicht redelijk eenvoduig een title of eerste paragraaf uit het document halen. Ook uit hun metadata kan je al veel halen.
5. **Risk**
	*  Heel goed! En allemaal oplosbaar. 
6. **planning**
	7. Ziet er goed uit.
