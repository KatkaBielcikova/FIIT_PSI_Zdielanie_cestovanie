# FIIT_PSI_Zdielanie_cestovanie

https://www.youtube.com/playlist?list=PLE0e2tyElyE8jpNQQbt5BjtnOhdnFRsDm

cviko 8: <br /> 
UI: <br /> 
UI01 registrcia - pouzit trace alebo use... <br />  
UI02 - auto - vybrat z comboboxu (zoznam soferovych aut) <br /> <br /> 

cviko 7: <br /> 
Sekvencny diagram: <br /> 
- pouzivatel nie je sucast systemu - dat prec <br />
- to ze bude pouzivatel nieco kontrolovat - dat prec <br />
- spravca je control, pouzivatel entita (ma sa nachadzat v diagrame tried) <br />
- specializovat spravcu (spravca pouzivatelov...) <br /><br /> 

cviko 6: <br />

- Analyticky model tried - ~~"aplikacia" - zrusit~~ <br />
			- ~~"pouzivatel" - nemusi tam byt~~ <br />
			- ~~"vytvorenie poziadavky" = to je use case, nie trieda, zmenit na "poziadavka"~~ <br />
			- ~~doplnit "ponuka"(alebo zoznam jazd...),~~ zoznamy definovat ako nejake agregacie <br />
			- spolujazdec nema byt v atributoch triedy sofer <br />
			- ~~doplnit "auto"~~  <br />
			- doplnit "rozvrh" alebo "zoznam" aby sa nestalo, ze jeden clovek bude na dvoch jazdach naraz 
			zmenit aby sofer a spolujazdec mohli ist na viacero jazd) <br />
			- ~~mozno este doplnit nejaku platbu alebo kredit~~ <br /> <br />




cviko 5: <br />
use case model - zaregistruj sa ak vodic musi mat podmienku, ze uz je pouzivatel zargistrovany <br /><br />
		

nie-funkcne poziadavky - "aplikacia dostupna vsade na svete" - zmenit na napr: dostupna vsade kde je internet, v roznych krajinach.... <br />
			- poziadavky by mali byt meratelne - "intuitivna aplikacia" - klient moze argumentovat ze nie je intuitivna <br />
			- "dostupna 24/7" - to je drahe a narocne na servery - zmenit na: vypadok aplikacie moze trvat max 30 min.... <br /><br />


cviko 4: <br />
diagram tried - ~~bez diakritiky, popis ciary musi byt podla hodinovych ruciciek~~	<br />
		~~poziadavka na jazdu - zrusit "obsahuje" auto~~	<br />
		~~pridat vztah medzi jazdou a poziadavkou na jazdu~~ 	<br />
		~~Hodnotenie by mali ist nejako po jazde - aby sme nehodnotili niekoho s kym sme nesli~~ <br />
		~~Zmenit pouzivatela na spolucestujuceho~~	<br /> <br />   		
				
Hodnotenie = ericsonn diagram - pridat druheho aktera	- toto neviem ako pridat <br />
~~Hodnotenie = activity diagram - activity treba nejako ukoncit, nemoze ostat "visiet" <br /> <br />~~
				

~~Registrovanie = ericsonn diagram - ciel - zmenit na pohlad z biznisu - napr ziskat co najviac klientov <br />~~
~~Registrovanie = activity diagram - premenovat akterov na "buduci sofer" a "buduci spolujazdec", zmenit <br />
					tie 3 plavebne drahy na jednu (pouzivatel)<br /><br />~~

~~Vytvorenie ponuky = ericsonn diagram - zmenit nazvy "vystup jazdy" na poziadavku a ponuku jazdy <br />~~
~~Vytvorenie ponuky = activity diagram - po kontrole moze ist este rozhodovanie ci su udaje spravne a podla toho pojde sipka bud dakej alebo naspat <br />~~
~~Vytvorenie dopytu = activity diagram - zmenit na "poziadavka", pridat rozhodovanie ako vyssie <br /><br />~~

Prihlasovanie na ponuku = activity diagram - ? - nezachytila som co povedal <br /><br />

~~Upravenie ponuky= ericsonn diagram - doplnik aktera spolujazda, information bude resources, chyba ciel - napr spokojnost pouzivatelov <br />~~
Upravenie ponuky = activity diagram - ? - nezachytila som co povedal <br /><br />

******************** INFO K APPKE *********************************
Udaje ktore zada:
- pouzivatel: Meno, priezvisko, email a telefon (overuje sa kodom), pouzivatelske meno, heslo, datum narodenia (musi mat 18r), trvaly pobyt, scan OP z ktoreho sa vyberie cislo OP a udaje ktore sa porovnaju s tymi co zadal pouzivatel (meno, priezvisko, datum narodenia, trvaly pobyt)
- sofer: scan vodicskeho, platnost VP, 
- vozidlo: SPZ (overuje sa STK), 5fotografii vozidla, vykon motora, vyrobca, model, ci je majitelom vozidla (ak nie tak potvrdenie od majitela napr ak manzelka atd.), max pocet miest (aj s vodicom), najazdenych km
