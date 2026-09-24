# _CONSTRUCCIÓ D’ALTAVEUS PERSONALITZA TS VS. ALTAVEUES COMERCIALS_ 

_Arnau | A_ 

_Tutora: 17/4/2026_ 

## **_Índex_** 

|**_Resum............................................................................................................................... 3_**|
|---|
|**_Introducció........................................................................................................................ 3_**|
|Motivació del projecte:.......................................................................................................................3|
|Hipòtesis:.............................................................................................................................................3|
|Objectius:.............................................................................................................................................3|
|**_Marc teòric:.......................................................................................................................4_**|
|El so:....................................................................................................................................................4|
|Característiques del so........................................................................................................................4|
|Els altaveus i el seu funcionament:.....................................................................................................7|
|El driver (peça):...................................................................................................................................7|
|El senyal:............................................................................................................................................15|
|Crossover:..........................................................................................................................................16|
|Capsa:................................................................................................................................................18|
|Directivitat i dispersió:......................................................................................................................20|
|Amplificador:.....................................................................................................................................21|
|L’estèreo, la imatge sonora i l’acústica de la sala:............................................................................24|
|Mesura i identificació de mesura......................................................................................................25|



1 

|**_Marc pràctic:................................................................................................................... 27_**|
|---|
|Introducció:.......................................................................................................................................27|
|Disseny de l’altaveu:..........................................................................................................................27|
|Construcció dels altaveus:.................................................................................................................31|
|**_Resultats i comparació:....................................................................................................34_**|
|Preu final:..........................................................................................................................................34|
|Introducció de productes:.................................................................................................................35|
|Comparació de rendiment:...............................................................................................................37|
|Comparació de preu:.........................................................................................................................40|
|**_Conclusió:........................................................................................................................41_**|
|**_Bibliografia......................................................................................................................42_**|



2 

## **_Resum_** 

#### **_Anglès_** 

This research project focuses on the design and construction of a three-way active loudspeaker with digital signal processing and wireless connectivity. The main objective is to determine whether a relatively low-cost self-built loudspeaker can achieve acoustic performance comparable to that of commercially available high-fidelity systems at a considerably higher price. 

The project analyses the main theoretical aspects involved in loudspeaker design, including sound propagation, frequency response, directivity, distortion, driver technologies, crossover systems, Thiele-Small parameters, enclosure design and amplification. Based on these principles, a three-way loudspeaker was designed using a woofer, a midrange driver and a tweeter, with digital crossover points at 600 Hz and 2.5 kHz. The system incorporates a bassreflex enclosure and digital signal processing for crossover filtering, equalisation, delay and level adjustment. 

The acoustic performance of the prototype was evaluated using a measurement microphone and REW software. Near-field measurements were used to analyse the low-frequency behaviour, while a gated far-field measurement was used for the mid and high frequencies. The measured response covered approximately 40 Hz to 15 kHz with variations of around ±3 dB, while the tweeter's specifications extend the expected response to 20 kHz. Total harmonic distortion remained approximately between 1% and 3% from 100 Hz to 10 kHz at around 77 dB SPL. 

The results show that the prototype can achieve a relatively uniform frequency response at a substantially lower cost than a comparable commercial pair. The project therefore demonstrates that careful acoustic design, measurement and digital signal processing can achieve a substantial level of performance and functionality without requiring the budget typically associated with comparable commercial systems. 

3 

#### **_Castellà_** 

Este trabajo de investigación se centra en el diseño y construcción de un altavoz activo de tres vías con procesamiento digital de señal y conectividad inalámbrica. El objetivo principal es determinar si un altavoz de fabricación propia y de coste relativamente reducido puede alcanzar un rendimiento acústico comparable al de sistemas comerciales de alta fidelidad de un precio considerablemente superior. 

El proyecto analiza los principales aspectos teóricos relacionados con el diseño de altavoces, incluyendo la propagación del sonido, la respuesta en frecuencia, la directividad, la distorsión, las tecnologías de los drivers, los sistemas de crossover, los parámetros Thiele-Small, el diseño de la caja acústica y la amplificación. A partir de estos principios, se diseñó un altavoz de tres vías utilizando un woofer, un midrange y un tweeter, con puntos de crossover digitales a 600 Hz y 2,5 kHz. El sistema incorpora una caja bass-reflex y procesamiento digital de señal para el filtrado del crossover, la ecualización, el ajuste del retardo y del nivel. 

El rendimiento acústico del prototipo se evaluó mediante un micrófono de medición y el software REW. Se utilizaron medidas de campo cercano para analizar el comportamiento a bajas frecuencias, mientras que para las frecuencias medias y altas se realizó una medida de campo lejano con gating temporal. La respuesta medida cubrió aproximadamente de 40 Hz a 15 kHz, con variaciones de alrededor de ±3 dB, mientras que las especificaciones del tweeter amplían la respuesta prevista hasta los 20 kHz. La distorsión armónica total se mantuvo aproximadamente entre el 1 % y el 3 % desde 100 Hz hasta 10 kHz a unos 77 dB SPL. 

Los resultados muestran que el prototipo puede alcanzar una respuesta en frecuencia relativamente uniforme a un coste considerablemente inferior al de un sistema comercial comparable. El proyecto demuestra, por tanto, que un diseño acústico cuidadoso, junto con la medición y el procesamiento digital de señal, puede alcanzar un nivel considerable de rendimiento y funcionalidad sin requerir el presupuesto habitual de sistemas comerciales comparables. 

4 

## **_Introducció_** 

El so és un fenomen que ens envolta cada dia. Gràcies a aquest, la humanitat ha pogut comunicar-se i expressar els seus pensaments, les seves preocupacions i idees. Amb el pas de les dècades hem aconseguit construir i millorar increïbles tecnologies que ens han permès modificar i utilitzar aquest canvi de pressions a favor nostre. Tot i això, sabem realment com funciona un altaveu? 

### **_Motivació del projecte:_** 

Sempre he estat bastant apassionat sobre el món de la reproducció de música (no la música en si, que també, però enfocat a altaveus, auriculars...), des d'amplificadors fins a altaveus i auriculars. Al llarg dels anys he tingut la gran sort i possibilitat d’experimentar amb diferents altaveus i sempre m’he preguntat si seria capaç de construir uns altaveus dignes. 

### **_Hipòtesis:_** 

És possible construir, amb coneixements autodidactes i un pressupost limitat, un altaveu d’alta fidelitat amb un rendiment comparable al d’opcions comercials de gamma mitjanaalta. 

### **_Objectius:_** 

L’objectiu d’aquest treball de recerca és determinar si la construcció d’uns altaveus d’alta fidelitat és viable amb recursos i coneixements relativament limitats. S’investigaran els diferents components que formen un altaveu, com el “ _crossover_ ”, els altaveus, la capsa que allotja tots aquests components... Per tal de demostrar-ho es construirà un altaveu d’alta fidelitat i es faran mesuraments d’aquest tot comparant-lo amb models comercials. 

5 

## **_Marc teòric:_** 

Per entendre com funciona un altaveu, primer s’ha d'entendre el principi fonamental en què es basa, el so. 

### **_El so:_** 

El so és una ona, és a dir, una pertorbació o variació que viatja a través d’un medi. Per exemple, explicat per Dan Russell (htps://www.acs.psu.edu/drussell/Demos/wavest - <u>intro/waves-intro.html), una ona és com la gent d’un partit formant una “ona”. Un grup</u> de gent s’aixeca i s’asseu, el grup del costat repeteix la mateixa acció, generant així una ona que es propaga per tot l’estadi. Tenim una variació, la gent aixecant-se, que es va desplaçant per tot l’estadi. Els individus no es mouen, però l’onada és transportada per tot l’estadi. 

En el cas del so, aquesta pertorbació es manifesta com una variació de pressió que es propaga a través d’un medi material, que pot ser sòlid, líquid o gasós. Quan parlem amb algú, les nostres cordes vocals generen una vibració que produeix variacions de pressió en l’aire. Aquestes variacions es propaguen fins a arribar a l’orella de l’oient, on són detectades i transformades en senyals nerviosos. 

### **_Característiques del so_** 

Una ona sonora es pot descriure mitjançant diferents propietats que permeten determinar com es comporta físicament i com la percebem. Les principals són la freqüència, l'amplitud, la intensitat, la longitud d'ona, la fase i la velocitat de propagació. 

#### **_La freqüència_** 

La freqüència indica quantes vegades es repeteix un cicle de l'ona en un segon i s'expressa en hertzs (Hz). Per exemple, una freqüència de 100 Hz significa que es produeixen 100 cicles cada segon. En el cas del so, la freqüència està relacionada amb l'altura percebuda: les freqüències baixes corresponen a sons greus, mentre que les freqüències altes corresponen a sons aguts. 

6 

#### **_L'amplitud_** 

L'amplitud indica la magnitud de la variació de l'ona respecte del seu punt d'equilibri. En una ona sonora, aquesta variació correspon als canvis de pressió que es produeixen en el medi. Una amplitud més gran implica una variació de pressió més gran i, en general, un so amb un nivell més elevat. L'amplitud és, per tant, una propietat física de l'ona i no s'ha de confondre directament amb la intensitat sonora. 

#### **_La intensitat_** 

La intensitat sonora indica quanta potència acústica travessa una determinada superfície. Es mesura en watts per metre quadrat (W/m²) i permet descriure com es distribueix l'energia transportada per l'ona. Està relacionada amb l'amplitud de l'ona: per a unes mateixes condicions de propagació, una amplitud de pressió més gran implica una intensitat més elevada. 

#### **_La longitud d'ona_** 

La longitud d'ona és la distància entre dos punts consecutius de l'ona que es troben en el mateix estat de vibració, com ara dues compressions consecutives. Es representa amb la lletra grega λ (lambda) i s'expressa en metres. 

La longitud d'ona està relacionada amb la freqüència i la velocitat de propagació mitjançant la següent expressió: 



on λ és la longitud d'ona, c és la velocitat de propagació i f és la freqüència. Per tant, si la velocitat es manté constant, una freqüència més alta correspon a una longitud d'ona més curta, mentre que una freqüència més baixa correspon a una longitud d'ona més llarga. 

#### **_La fase_** 

La fase indica en quin punt del seu cicle es troba una ona respecte d'un punt de referència. Es pot expressar en graus, on un cicle complet correspon a 360°. Dues ones de la mateixa 

7 

freqüència poden estar en fase quan els seus cicles coincideixen, o desfasades quan una està avançada o retardada respecte de l'altra. 

La fase és especialment important quan dues o més ones es combinen. Si les seves variacions coincideixen, poden reforçar-se entre elles, mentre que si es troben desfasades poden produir una reducció parcial o total del nivell resultant. Aquest fenomen d'interferència és especialment important en el funcionament dels altaveus amb diversos drivers. 

#### **_La velocitat de propagació_** 

La velocitat de propagació indica la rapidesa amb què l'ona es desplaça a través del medi. Aquesta velocitat depèn principalment del medi i de les seves propietats. En l'aire, per exemple, varia amb la temperatura i altres condicions ambientals; a una temperatura de 20 °C és d'aproximadament 343 m/s. La velocitat de propagació, la freqüència i la longitud d'ona estan relacionades mitjançant l'expressió anterior. 

#### **_El rang de freqüències audible_** 

L'oïda humana no pot percebre totes les freqüències. De manera aproximada, es considera que el rang audible se situa entre els 20 Hz i els 20 kHz, tot i que aquest límit varia segons la persona i pot disminuir amb l'edat. Dins d'aquest rang, les freqüències es poden dividir de manera aproximada en tres zones: baixes o greus, mitjanes i altes o agudes. 

En el context dels altaveus, aquesta distribució és especialment important, ja que diferents drivers estan dissenyats per reproduir diferents zones de l'espectre. Per aquest motiu, els sistemes que utilitzen diversos drivers han de repartir adequadament les freqüències entre aquests. 

#### **_La resposta en freqüència_** 

La resposta en freqüència descriu com varia el nivell de reproducció d'un altaveu segons la freqüència. Es pot representar mitjançant un gràfic on l'eix horitzontal correspon a la 

8 

freqüència i el vertical al nivell de pressió sonora. Una resposta idealment plana indicaria que totes les freqüències es reprodueixen al mateix nivell, tot i que en un sistema real sempre hi ha determinades variacions. 

La resposta en freqüència és un dels paràmetres més importants per caracteritzar el comportament acústic d'un altaveu i serà analitzada amb més detall posteriorment, juntament amb la interpretació dels gràfics obtinguts durant les mesures. 

### **_Els altaveus i el seu funcionament:_** 

Un dels primers altaveus fou creat el 1876 per Johann Philipp Reis<sup>1</sup> (tot i ser erròniament atribuït a Alexander Graham) i va ser utilitzat pel primer telèfon, però no va ser fins al 1877, amb Werner von Siemens que es va teoritzar el primer altaveu dinàmic<sup>2</sup> . A partir d’aquest, gent com Oliver Lodge i John Stroh van anar perfeccionant aquell invent i, fins avui dia, seguim utilitzant aquest i altres simples conceptes creats fa més d’un segle per escoltar música. Aquesta meravellosa tecnologia aconsegueix, mitjançant una membrana que es mou, generar ones de pressió i, per tant, so. Un altaveu està compost per diverses peces, aquestes sent principalment: driver (l’altaveu, la peça mecànica individual), el “crossover” (si hi ha més d’un altaveu present), la capsa que l’engloba i, en el cas d’un altaveu actiu, l’amplificador. 

### **_El driver (peça):_** 

En aquest treball s’anomenarà l’altaveu (peça individual, sense capsa) com a ‘driver’ per a evitar confusions entre aquesta i l’altaveu sencer (amb capsa). 

El driver és un transductor que converteix un senyal elèctric en moviment mecànic. Aquest moviment desplaça el diafragma i genera variacions de pressió en l'aire que percebem com a so. Tenen diferents propietats que marquen com són i determinen la seva qualitat de reproducció. 

> 1 <u>The Forgotten Johann Philipp Reis</u> 

> 2 <u>Loudspeaker History</u> 

9 

### **_I. Distorsió:_** 

La distorsió és qualsevol alteració del senyal original durant el procés de reproducció. En un sistema ideal, el driver reproduiria exactament el senyal d’entrada, però en la pràctica això no és possible. 

Una de les formes més comunes és la distorsió harmònica total (THD). Aquesta apareix quan es generen freqüències addicionals que no estaven presents en el senyal original, normalment múltiples de la freqüència principal. 

Les causes poden ser diverses: moviments no lineals de la membrana, limitacions del sistema motor o fins i tot problemes en l’amplificació. 

Tot i que certa quantitat de distorsió és inevitable, en sistemes d’alta fidelitat es busca minimitzar-la al màxim. 

## **_II. Sensibilitat:_** 

La sensibilitat d’un driver indica el nivell de pressió sonora que és capaç de produir amb una determinada potència elèctrica. Normalment s’expressa en decibels (dB) a una distància d’un metre aplicant una potència determinada (sovint 1 watt). 

Un driver amb una sensibilitat alta produirà més nivell de pressió sonora amb la mateixa potència que un altre amb sensibilitat més baixa. Una diferència de 3 dB en el nivell de pressió sonora correspon aproximadament al doble d’intensitat acústica. 

Això té implicacions pràctiques importants. Els drivers amb una sensibilitat més baixa necessiten més potència elèctrica per assolir el mateix nivell de pressió sonora que un driver més sensible. Per aquest motiu, la sensibilitat és un dels paràmetres que cal tenir en compte a l’hora de combinar un driver amb un amplificador. 

### **_III. Impedància:_** 

10 

La impedància és una propietat elèctrica que descriu la resistència que presenta un driver al pas del corrent altern. Es mesura en ohms (Ω) i és un factor clau a l’hora de combinar altaveus amb amplificadors. 

A diferència d’una resistència simple, la impedància no és constant, sinó que varia en funció de la freqüència del senyal. Això es deu a la presència de components inductius (com la bobina) i, en alguns casos, capacitatius. 

Per exemple, un altaveu etiquetat com a 8 Ω no té exactament aquest valor en tot moment, sinó que és una aproximació. Aquesta variació pot afectar el comportament de l’amplificador, especialment si aquest no està preparat per treballar amb càrregues variables. 

Si la impedància és massa baixa, l’amplificador pot haver de subministrar més corrent del que pot gestionar, provocant sobreescalfament o distorsió. Una impedància més alta fa que, per a una mateixa tensió de sortida, circuli menys corrent i es transfereixi menys potència al driver. Per això, és important assegurar la compatibilitat entre ambdós components. 

A més de la distorsió, la sensibilitat i la impedància, existeixen altres paràmetres que permeten descriure el comportament d’un driver, entre els quals destaquen els paràmetres Thiele-Small (T/S). Desenvolupats per A. Neville Thiele i Richard H. Small, constitueixen un model que permet descriure el comportament elèctric i mecànic d’un altaveu dinàmic, especialment a les freqüències baixes. Són molt útils en el disseny acústic perquè permeten estudiar com es comportarà un driver quan es combina amb una determinada caixa, sense haver de construir físicament totes les configuracions possibles. 

Entre els principals paràmetres T/S trobem la freqüència de ressonància (Fs), el factor de qualitat mecànic (Qms), el factor de qualitat elèctric (Qes) i el factor de qualitat total (Qts). També són importants el volum d’aire equivalent (Vas), la resistència de la bobina (Re), la superfície efectiva del diafragma (Sd) i l’excursió lineal màxima (Xmax). 

11 

La Fs correspon a la freqüència natural de ressonància del conjunt mòbil del driver. Al voltant d’aquesta freqüència, la massa mòbil i la suspensió interactuen i produeixen un augment característic de la resposta d’impedància. Una Fs baixa pot indicar un major potencial per reproduir freqüències greus, però no determina per si sola fins a quina freqüència baixa podrà arribar el driver, ja que també hi intervenen la caixa acústica, el tipus de càrrega i la resta de paràmetres T/S. 

Els paràmetres Qms, Qes i Qts descriuen el grau d’amortiment del sistema al voltant de la seva ressonància. El Qms està relacionat amb les pèrdues mecàniques, mentre que el Qes descriu les pèrdues associades al sistema elèctric. El Qts representa l’amortiment total i es calcula a partir dels dos anteriors: 



El Vas representa el volum d’aire que tindria una compliància equivalent a la de la suspensió del driver. No correspon al volum de la caixa necessari, sinó que és una propietat del propi driver que, juntament amb Fs i Qts, ajuda a determinar quina càrrega acústica pot resultar adequada. 

Altres paràmetres, com Sd i Xmax, permeten relacionar les característiques físiques del driver amb la quantitat d’aire que pot desplaçar. La Sd és la superfície efectiva del diafragma, mentre que Xmax representa l’excursió màxima aproximadament lineal. La combinació d’ambdós paràmetres és especialment rellevant a baixes freqüències, on per generar pressió sonora és necessari desplaçar una quantitat considerable d’aire. 

Per tant, els paràmetres Thiele-Small no només serveixen per descriure el driver de manera individual, sinó que permeten predir la seva interacció amb una caixa acústica. 

També podem categoritzar els drivers segons el rang de freqüències en què operen, ja que és físicament impossible tenir les mateixes característiques per reproduir tan 

12 

freqüències altes com baixes en el mateix altaveu. Com hem vist abans, hi ha tres rangs principals i hi ha drivers especialitzats en cada un d’aquests rangs. 

### **_I. Subwoofer:_** 

Els subwoofers estan dissenyats per reproduir les freqüències més baixes (normalment per sota dels 80–120 Hz). Aquests drivers solen tenir un diàmetre gran i una gran excursió (capacitat de desplaçar-se endavant i enrere). Això els permet moure grans volums d’aire, necessari per generar sons greus. No obstant això, aquesta mateixa característica fa que siguin menys factibles en freqüències altes. 

### **_II. Woofer:_** 

Els woofers cobreixen la part baixa i part de la gamma mitjana. Són una mena de compromís entre mida, velocitat i precisió. En molts sistemes domèstics, un woofer acostuma a cobrir una gran part de l’espectre audible. 

### **_III. Midrange-woofer:_** 

Els midrange són drivers dissenyats per reproduir les freqüències mitjanes de l'espectre audible, situant-se entre el woofer i el tweeter. El seu rang de funcionament pot variar segons el disseny de l'altaveu, però habitualment cobreix des d'uns centenars de hertzs fins a uns quants quilohertzs. 

Aquesta zona és especialment important per a la reproducció de la veu i de molts instruments musicals. En un sistema de tres vies, el midrange permet que el woofer es concentri en les freqüències baixes i el tweeter en les altes, repartint així l'espectre entre els diferents drivers. 

### **_IV. Tweeters:_** 

Finalment, els tweeters són els encarregats de reproduir les freqüències altes. Com que aquestes freqüències tenen longituds d’ona molt petites, es necessiten elements mòbils de baixa massa capaços de reproduir aquestes variacions ràpides. Per això, 

13 

els tweeters acostumen a ser petits i fabricats amb materials molt lleugers. Existeixen diferents dissenys com el dome tweeter, el ribbon tweeter (semblant al planar que veurem a continuació) i els altaveus de “ _banya_ ”, que s’assemblen a una trompeta. 

A més, existeixen diferents dissenys de driver i els mateixos s’utilitzen també als auriculars. Entrarem en el detall en el funcionament de diversos models. La majoria de noms són anglesos, es farà el millor intent a traduir els noms. 

### **_I. Driver electrodinàmic (Il·lustració 1):_** 

És el tipus de driver més simple i més utilitzat en altaveus. Funciona amb una bobina que, quan hi circula un corrent elèctric, interactua amb el camp magnètic d’un imant permanent. Aquesta bobina està adherida a una membrana que, en desplaçar-se amb la bobina, mou l’aire i genera so. Aquest driver pot ser dividit en tres parts: el sistema motor, el diafragma i el sistema de suspensió. 



##### **Il·lustració  1 -** 

El sistema motor s’encarrega de posar en moviment el **Driver dinàmic** diafragma. Està compost d’un imant (“magnet”), la bobina de veu (“Voice coil”) i l’encapsulament que sosté i dirigeix el camp magnètic de l’imant (“pole piece” i “back plate”). La il·lustració 1 és la secció d’un driver dinàmic i mostra la col·locació normal d’aquests components. Un corrent altern és aplicat a la bobina i, segons les variacions del corrent, la força que actua sobre aquesta varia, provocant el moviment de la bobina dins del camp magnètic. Diversos factors poden afectar el funcionament d’aquest, com, per exemple, la longitud de la bobina, la distància entre les parets i la bobina... A més, hem de controlar correctament el camp magnètic, per això s'utilitzen diferents formes geomètriques en l'encapsulament de l’imant. 

El diafragma és la membrana cònica que, connectada a la bobina, mou l’aire i genera el so. Les seves propietats físiques influeixen molt en el resultat final. Idealment hauria de ser molt rígida, molt lleugera i capaç d’amortir bé les seves pròpies 

14 

vibracions, però en la pràctica és difícil optimitzar les tres propietats alhora, per això cada material representa un compromís diferent. El paper és el més tradicional: és econòmic, està ben amortit i és sensible a la humitat. Els metalls com l’alumini o el titani, que són rígids i lleugers, poden oferir una bona rigidesa amb una massa reduïda, però poden presentar ressonàncies que afectin la resposta del driver. El Kevlar i la fibra de carboni combinen rigidesa i bon amortiment, reduint les vibracions no desitjades, i s’utilitzen en diversos tipus de drivers. En els tweeters són habituals materials com la seda o diferents metalls, cadascun amb propietats físiques diferents. L’elecció del material del diafragma és una de les decisions importants en el disseny d’un driver dinàmic. 

Per últim, tenim el sistema de suspensió, que s’encarrega de sostenir el diafragma mentre li permet moure's lliurement per tal de produir el so. Està format per una vora de goma (surround) i un “centrador” (Spider). La tasca d’aquests dos elements és principalment mantenir el conjunt mòbil centrat i proporcionar una força de restauració que ajudi a retornar-lo cap a la seva posició d’equilibri. 

Driver magnètic “planar” 

Aquesta mena de driver (il·lustració 2) es basa en un principi de funcionament diferent del driver dinàmic tradicional. En lloc d’una bobina concentrada en un punt, utilitza una membrana plana molt fina sobre la qual hi ha distribuït un conductor elèctric. 



<!-- Start of picture text -->
s<br>—= =<br>= Ss<br>= 2<br>=<br><!-- End of picture text -->

Aquesta membrana es col·loca entre dos conjunts **Il·lustració 2 - Driver planar** d’imants. Quan el corrent elèctric passa pel conductor, es genera una força a causa de la interacció entre el camp magnètic produït pel corrent i el dels imants, provocant el moviment de la membrana. 

15 

Aquest sistema té diversos avantatges. En primer lloc, la força s’aplica de manera més distribuïda sobre la superfície de la membrana, fet que pot reduir determinades deformacions i distorsions. A més, en utilitzar una membrana molt lleugera, pot oferir una bona resposta transitòria i una reproducció detallada del senyal. 

Tot i això, també presenten inconvenients, com una sensibilitat generalment més baixa i la necessitat d’una amplificació adequada per assolir nivells de pressió sonora elevats. 

S’utilitza principalment en auriculars, tot i que també existeixen altaveus planarmagnetic. 

### **_Driver ribbon (tweeter de cinta)_** 

Els ribbon drivers (il·lustració 3) són una variant dels drivers planars. Utilitzen una cinta molt fina i lleugera, habitualment d’alumini, suspesa entre dos imants. 

Quan passa el corrent per la cinta, aquesta interactua amb el camp magnètic dels imants i es mou ràpidament cap endavant i cap enrere, generant el so. 



El seu principal avantatge és la baixa massa de la **Il·lustració  3 - Ribbon driver** cinta, que permet una resposta ràpida a les variacions del senyal i pot oferir una bona reproducció de les freqüències altes. També poden presentar una dispersió àmplia en determinades configuracions, cosa que pot afavorir una reproducció més uniforme fora de l’eix. 

Tanmateix, són fràgils, poden tenir una sensibilitat baixa i requereixen un disseny i una amplificació adequats. Normalment s’utilitzen com a tweeters en altaveus, ja que estan especialment orientats a la reproducció de les freqüències altes. 

16 

### **_II. Driver electroestàtic:_** 

Reconeguts per la seva precisió, aquest tipus de driver (il·lustració 4) canvia totalment el sistema que utilitza per a desplaçar l’aire. En lloc d’utilitzar camps magnètics, funciona mitjançant forces electroestàtiques. 



**Il·lustració  4 - Driver electroestàtic** 

Consisteix en una membrana extremadament **Il·lustració  4 - Driver electroestàtic** fina situada entre dues plaques metàl·liques anomenades, en anglès, “stators”. Aquesta membrana es carrega elèctricament i, quan s’aplica un senyal d’àudio a les plaques, es genera un camp electroestàtic variable que atrau o repel·leix la membrana. 

Això provoca el seu moviment i, en conseqüència, la generació d’ones sonores. Com que la massa de la membrana és molt reduïda, aquests altaveus ofereixen una resposta molt ràpida i una distorsió mínima. 

No obstant això, tenen limitacions importants: requereixen altes tensions per funcionar, són més difícils de fabricar i, generalment, tenen dificultats per reproduir freqüències molt baixes. Com els planars, acostumen a utilitzar-se en auriculars. 

Els auriculars més cars del món, els Sennheiser HE-1 (il·lustració 5), amb un preu de 89.990,00 € (al temps d’escriptura) utilitza aquesta mena de driver. 

**Il·lustració  5 - Sennheiser HE-1** 

### **_El senyal:_** 

Perquè un altaveu pugui reproduir so, necessita un senyal elèctric que representi aquest so. Aquest senyal és, essencialment, una representació elèctrica de l’ona sonora original. 

17 

Quan es grava o es genera un so digitalment, aquest es transforma en una seqüència de valors numèrics que representa l’ona sonora de forma discreta en el temps. Per poder reproduir aquest so mitjançant un altaveu, aquests valors s’han de convertir en un senyal elèctric analògic, que consisteix en una variació contínua de tensió. 

L’altaveu rep aquest senyal i el converteix de nou en moviment mecànic mitjançant els sistemes descrits anteriorment. Aquest moviment provoca variacions de pressió en l’aire que es propaguen en forma d’ona sonora. Per tant, la qualitat del senyal repercuteix en la fidelitat de reproducció final. Qualsevol interferència, distorsió o pèrdua d’informació en el senyal pot afectar el resultat final. 

En el món modern, una gran part de l’àudio es troba emmagatzemat i processat en format digital. Un fitxer d’àudio, ja sigui un MP3, un FLAC o un WAV, emmagatzema el so com una seqüència de números que descriuen l’ona sonora de forma discreta en el temps. Per poder reproduir aquest so, cal convertir-lo a un senyal analògic. Aquesta és la funció del convertidor digital-analògic, més conegut com a DAC (de l’anglès Digital-to-Analogue Converter). 

La cadena de so, doncs, segueix un camí bastant definit: el senyal digital surt del reproductor (un ordinador, un telèfon, un reproductor dedicat...) i passa pel DAC, que el converteix en un senyal analògic. Aquest senyal analògic és encara massa feble per moure un altaveu directament, per tant s’envia a l’amplificador, que augmenta la potència del senyal, i finalment arriba a l’altaveu, que el converteix en so. Cada pas d’aquesta cadena és important: una alteració en qualsevol punt pot afectar els següents. 

### **_Crossover:_** 

La majoria d’altaveus d’alta qualitat disposen de més d’un driver, ja que és pràcticament impossible que un sol driver reprodueixi tot el rang de freqüències de manera òptima. Per aquest motiu, es divideix el senyal en diferents bandes de freqüència, cadascuna dirigida a un driver específic. Aquesta funció la realitza el “crossover”. 

18 

El crossover és un sistema de filtratge que agafa el senyal d’entrada i el separa en diferents parts. Aquest filtratge es realitza mitjançant components electrònics bàsics. Els capacitadors permeten el pas de freqüències altes però bloquegen les baixes, mentre que els inductors fan el contrari. Un cop separat el senyal, s’utilitzen aquest component per a atenuar el so que el driver no pot reproduir. D’aquesta manera, cada altaveu només treballa en el rang per al qual ha estat dissenyat, millorant la qualitat del so i reduint distorsions. Per últim, els resistors, s’utilitzen per ajustar el nivell (volum) de cada driver i equilibrar el conjunt. 

Així el crossover envia les freqüències baixes al woofer, les mitjanes al midrange i les altes al tweeter. 

El filtratge no és instantani: cap component talla una freqüència de cop, sinó que atenua progressivament el senyal a mesura que ens allunyem del punt de tall. Aquesta progressió es mesura en dB per octava (una octava és cada vegada que la freqüència es duplica o es divideix per dos). Com més component de filtratge s'acumulen en cascada (a més "ordre" del filtre), més pronunciada és aquesta caiguda: un filtre de primer ordre “cau” uns 6dB/octava, un de segon ordre uns 12dB/octava, i així successivament. Un pendent més pronunciat separa millor els drivers adjacents (menys superposició de freqüències), però també augmenta considerablement la complexitat i dificulta l’alineació de la fase. 

La fase descriu la posició temporal d'una ona sonora en el seu cicle. Quan dos altaveus reprodueixen simultàniament la mateixa freqüència (com passa en la zona de creuament del filtre), és imprescindible que les seves ones estiguin alineades en el temps. Tanmateix, els crossovers modifiquen 

**Il·lustració  6 - Distorisió de fases** 

aquesta relació temporal introduint un desfasament (il·lustració 6). Si les ones arriben desfasades —és a dir, si el pic d'una ona coincideix amb la vall de l'altra—, es produeixen interferències: les freqüències es poden cancel·lar parcialment o reforçar de manera 

19 

irregular. Això altera la resposta en freqüència del sistema i degrada la naturalitat del so, motiu pel qual el disseny d'un crossover requereix un equilibri rigorós entre teòrica i proves pràctiques. 

També cal diferenciar entre crossovers passius i digitals. Els passius són els més comuns en altaveus comercials i es col·loquen després de l’amplificador, mentre que els digitals funcionen abans de l’amplificació i permeten un control molt més precís, tot i que fan el sistema més complex. 

### **_Capsa:_** 

La capsa no només serveix per contenir els components, sinó que té un paper fonamental en el comportament acústic de l’altaveu. De fet, pot arribar a afectar tant el so com el propi driver. 

Una de les seves funcions principals és controlar les ones generades per la part posterior de la membrana. Sense capsa, aquestes ones poden interferir amb les de la part frontal i provocar cancel·lacions, especialment en les freqüències baixes. 

El tipus de capsa influeix molt en el resultat final. Les capses tancades ofereixen un comportament més controlat, mentre que les bass-reflex utilitzen un port (una obertura) per reforçar els greus i augmentar l’eficiència (il·lustració 7). Aquesta obertura pot estar 



<!-- Start of picture text -->
Ci l,<br>Acoustic Suspension Bass Reflex<br>(Sealed) Enclosure (Ported) Enclosure<br><!-- End of picture text -->

**Il·lustració  7 - Tipus de capses** 

integrada directament dins de la capsa o adoptar la forma d’un tub. La seva mida i longitud determinen la freqüència a la qual està sintonitzada la capsa, permetent aprofitar el moviment de l’aire del seu interior per reforçar les freqüències baixes. 

Els materials també tenen un impacte directe. Materials com el MDF són molt utilitzats perquè tenen una bona densitat i absorbeixen vibracions. Si la capsa vibra massa, 

20 

aquestes vibracions es converteixen en so no desitjat i degraden la qualitat final. Per això, en molts dissenys s’afegeixen reforços interns i materials absorbents per reduir ressonàncies/vibracións. 

El volum intern de la caixa influeix en la resposta de baixa freqüència del sistema. En una configuració bass-reflex, aquest volum interactua amb el port i amb els paràmetres Thiele-Small del driver, determinant en part la freqüència de sintonia i el comportament de l'altaveu a baixes freqüències. 

Per tant, el volum de la caixa s'ha d'escollir en funció de les característiques del driver i del tipus de càrrega acústica que es vol obtenir, ja que un volum més gran o més petit pot modificar considerablement la resposta del sistema. 

A part del tipus de driver, la disposició física dels drivers també influeix en el comportament del sistema. No només és important quins drivers s'utilitzen, sinó també com es distribueixen dins de la capsa. 

La configuració més comuna és la de dues vies, formada per un woofer i un tweeter. El woofer s’encarrega de les freqüències baixes i mitjanes, mentre que el tweeter reprodueix les freqüències altes. Aquesta configuració és molt utilitzada perquè és relativament simple, econòmica i pot oferir molt bons resultats si està ben dissenyada. 

En sistemes més avançats, es fa servir la configuració de tres vies, on s’afegeix un altaveu específic per a les freqüències mitjanes. Això permet repartir millor el treball entre els diferents drivers i millorar la fidelitat, especialment en la reproducció de veus i instruments. Tot i això, també augmenta la complexitat del crossover i del disseny general. 

També és bastant habitual trobar configuracions amb més d’un woofer, com per exemple sistemes amb dos woofers i un tweeter (MTM). Això permet augmentar la capacitat de reproduir greus i millorar la pressió sonora (volum) sense necessitat d’utilitzar un altaveu molt gran. En altres casos, especialment en sistemes professionals o de grans dimensions, 

21 

es poden utilitzar múltiples drivers alineats verticalment (line array). Aquesta disposició permet controlar millor la dispersió del so i mantenir una cobertura més uniforme en espais grans. 

Cal destacar el driver coaxial (il·lustració 8). En aquest cas, el tweeter es col·loca al centre del woofer, compartint el mateix eix. A diferència de les configuracions tradicionals, on cada driver està separat físicament, aquí el so de totes les freqüències prové pràcticament del mateix punt. Això té avantatges importants en termes de coherència i fase, ja que es redueixen els problemes derivats de la separació entre **Il·lustració  8 – Driver coaxial** altaveus. Aquesta característica pot millorar la imatge estèreo i la precisió espacial del so, fent que la localització dels instruments sigui més clara. No obstant això, també presenta dificultats. El disseny és més complex, ja que el tweeter s’ha d’integrar dins del woofer sense interferir en el seu funcionament. A més, poden aparèixer limitacions en la dispersió de les freqüències altes. 

Els altaveus coaxials són molt comuns en sistemes d’automòbil i també en alguns monitors d’estudi, on es busca una bona coherència del so en espais reduïts. 

En general, la configuració dels drivers afecta com es distribueix el so en l’espai, com interactuen les diferents freqüències i com percep l’oient el conjunt. Per això, és un aspecte clau en el disseny d’altaveus d’alta fidelitat. 

### **_Directivitat i dispersió:_** 

La directivitat descriu com es distribueix el so que emet un altaveu en les diferents direccions. Aquesta distribució varia principalment segons la freqüència i la mida del driver. 

22 

A freqüències baixes, la longitud d'ona és gran en comparació amb les dimensions del driver, de manera que el so tendeix a dispersar-se de forma més àmplia. A mesura que augmenta la freqüència, la longitud d'ona disminueix i el driver tendeix a concentrar més el so cap a la seva direcció frontal. Per això, un mateix driver pot passar de tenir una dispersió àmplia a freqüències baixes a ser més directiu a freqüències altes. 

#### **_Directivitat horitzontal i vertical_** 

La directivitat pot variar segons la direcció relativa a l'altaveu. La directivitat horitzontal descriu com varia el so quan l'oient es desplaça cap als costats, mentre que la vertical descriu què passa quan es mou cap amunt o cap avall. 

Aquest comportament es pot estudiar mitjançant mesures fora de l'eix, conegudes com a mesures off-axis. En aquestes mesures es registra la resposta de l'altaveu des de diferents angles i es compara amb la resposta frontal, habitualment a 0°. 

Aquestes mesures permeten observar si la resposta de l'altaveu es manté uniforme quan l'oient es desplaça respecte de l'eix principal. 

#### **_Disposició dels drivers_** 

La disposició física dels drivers també pot influir en la directivitat del conjunt. La seva separació i orientació poden fer que la dispersió sigui diferent en el pla horitzontal i en el vertical. 

Per aquest motiu, en el disseny d'un altaveu és important tenir en compte la disposició dels diferents drivers i no només les seves característiques individuals. En aquest projecte, aquest aspecte s'ha considerat en la disposició vertical i asimètrica del tweeter, el midwoofer i el woofer, buscant obtenir una resposta més uniforme fora de l'eix. 

### **_Amplificador:_** 

Un amplificador d'àudio és un dispositiu electrònic que augmenta la potència d'un senyal elèctric d'àudio per tal de poder alimentar un altaveu. Rep un senyal d'entrada de baixa 

23 

potència i, mitjançant l'energia proporcionada per la seva font d'alimentació, genera a la sortida un senyal capaç de proporcionar la tensió i el corrent necessaris per moure el driver. L'objectiu és mantenir la forma del senyal original amb la mínima distorsió possible. 

### **_I. Classe A_** 

Per entendre el funcionament d’un amplificador, primer cal entendre el paper del transistor. Aquest component permet controlar el corrent que circula per un circuit a partir d’un senyal elèctric més petit. Es pot imaginar de manera simplificada com un interruptor controlable: en lloc de limitar-se a estar obert o tancat, el transistor pot regular de manera gradual el corrent que el travessa. D’aquesta manera, un senyal d’àudio de poca potència pot controlar un corrent més gran proporcionat per la font d’alimentació i generar a la sortida un senyal amb més potència. 

En un amplificador de classe A, el transistor està preparat per conduir durant tot el cicle del senyal d’àudio, tant en la part positiva com en la negativa. Això permet amplificar el senyal complet sense haver de repartir-lo entre diferents transistors. 

Aquest funcionament fa que els amplificadors de classe A puguin aconseguir una baixa distorsió, ja que el transistor no ha de passar contínuament entre un estat de conducció i un estat de no conducció durant la reproducció del senyal. El principal inconvenient és l’eficiència: el transistor continua conduint fins i tot quan no hi ha senyal d’àudio, de manera que una part important de l’energia elèctrica es dissipa en forma de calor. Per aquest motiu, els amplificadors de classe A necessiten una dissipació tèrmica considerable i són poc eficients comparats amb altres classes d’amplificació. 

### **_II. Classe AB_** 

24 

En un amplificador de classe AB, el funcionament és similar al de la classe A, però el senyal es reparteix entre dos transistors. Un transistor s'encarrega principalment de la part positiva del senyal i l'altre de la part negativa. Per evitar que hi hagi un buit entre les dues parts, els dos transistors condueixen durant una petita part del cicle al mateix temps. D'aquesta manera, es redueix la distorsió que es produiria si cada transistor només funcionés durant exactament la meitat del cicle. 

Aquest funcionament permet obtenir una eficiència superior a la de la classe A, ja que els transistors no han de conduir durant tot el cicle quan no és necessari. Al mateix temps, manté una distorsió relativament baixa, tot i que el circuit és una mica més complex que el d'un amplificador de classe A. Per aquest motiu, la classe AB s'ha utilitzat àmpliament en amplificadors d'àudio, ja que ofereix un compromís entre el baix nivell de distorsió de la classe A i un consum d'energia més reduït. 

### **_III. Classe D_** 

A diferència dels amplificadors de classe A i AB, en un amplificador de classe D els transistors no s'utilitzen principalment per regular de manera contínua el corrent, sinó que funcionen com interruptors que commuten ràpidament entre un estat de conducció i un estat de no conducció. El senyal d'àudio controla aquesta commutació a una freqüència molt elevada, de manera que el corrent mitjà obtingut a la sortida segueix les variacions del senyal original. 

Abans d'arribar a l'altaveu, aquest senyal passa per un filtre que elimina els components d'alta freqüència produïts per la commutació i recupera el senyal d'àudio amplificat. Aquest funcionament permet reduir considerablement la quantitat d'energia que es dissipa en forma de calor i aconseguir una eficiència elevada. Per aquest motiu, els amplificadors de classe D són especialment 

25 

adequats per a sistemes d'àudio on es necessita una potència elevada amb un consum i una dissipació de calor reduïts. 

### **_L’estèreo, la imatge sonora i l’acústica de la sala:_** 

Quan escoltem so en la vida real, el cervell utilitza diferències de temps i d’intensitat entre les dues oïdes per determinar d’on prové aquest. L’estèreo aprofita aquest mateix principi utilitzant dos canals (esquerra i dreta), reproduïts per dos altaveus separats. Això permet crear la sensació d’espai i posicionar els sons, el que es coneix com a imatge sonora o “soundstage”. 

Quan el sistema està ben configurat, l’oient pot identificar on es troba cada instrument dins l’escena sonora. Aquesta percepció depèn molt de la col·locació dels altaveus, que idealment han de formar un triangle equilàter amb l’oient, i també de la coherència de fase del sistema. Si hi ha desfasaments o mala alineació, la imatge es torna imprecisa. 

Ara bé, els altaveus no funcionen en el buit. El so interactua amb la sala, reflectint-se a parets, sostre i terra. Aquestes reflexions arriben amb retard respecte al so directe i poden afectar la claredat i la localització dels sons. Quan moltes reflexions s’acumulen, es produeix la reverberació. 

Un altre problema habitual a les habitacions són les ones estacionàries. Això passa quan la distància entre dues parets paral·leles coincideix amb la longitud d’ona d’una freqüència. En aquests casos, alguns greus sonen molt forts en certs punts de l’habitació i gairebé desapareixen en d’altres. Això fa que la resposta en freqüència sigui molt irregular, sobretot en els baixos. 

Per reduir l’efecte d’aquests problemes, s’utilitzen materials absorbents (com escuma acústica, catifes, cortines gruixudes o panells de llana mineral) que absorbeixen l’energia sonora de les reflexions, i difusors, que dispersen el so de manera més uniforme en comptes de reflectir-lo cap a un sol punt. En sales professionals d’enregistrament o de monitoratge, el tractament acústic és tan important com els mateixos altaveus. En un 

26 

entorn domèstic, tot i que no cal arribar a l’extrem d’un estudi professional, una bona col·locació dels altaveus i alguns elements absorbents estratègics poden marcar una diferència notable en la qualitat del so. 

### **_Mesura i identificació de mesura_** 

Per conèixer el comportament d'un altaveu és necessari realitzar mesures que permetin analitzar com reprodueix diferents freqüències i nivells de pressió sonora. Aquestes mesures permeten representar gràficament diferents característiques del sistema i comparar-ne el comportament. 

#### **_Resposta en freqüència_** 

La resposta en freqüència permet observar com varia el nivell de pressió sonora d'un altaveu al llarg de l'espectre audible. En la seva representació gràfica, l'eix horitzontal correspon a la freqüència, normalment en Hz, i l'eix vertical al nivell de pressió sonora, expressat en dB. (Il·lustració 10) 

Una resposta completament plana indicaria que totes les freqüències es reprodueixen al mateix nivell. En la pràctica, però, sempre existeixen variacions. Per interpretar una gràfica és important observar la tendència general de la resposta i les variacions que apareixen al llarg de l'espectre. 



<!-- Start of picture text -->
4109 FR Magnitude dB re 20uPa/2.83V (U6 oct)<br>CTO TTT Ts<br>smCT TT<br>cotLUTMT 7s TTrTATT<br>odPA<br>LY<br>|<br>oT<br>UA nt<br>awo ZL<br>a<br>er ineeson<br>Pveictld<br><!-- End of picture text -->

**Il·lustració 10 – Gràfic de resposta en freqüència** 

Les pujades indiquen que una determinada zona de freqüències es reprodueix amb més nivell, mentre que les caigudes indiquen una menor reproducció. També és important diferenciar entre variacions suaus i àmplies i variacions molt pronunciades, ja que poden tenir causes diferents. 

27 

#### **_Resposta fora de l'eix_** 

La resposta en freqüència també es pot mesurar des de diferents angles respecte de l'eix principal de l'altaveu. Aquestes mesures, conegudes com a mesures “off-axis” (fora d’eix), permeten observar com varia la resposta quan canvia la posició de l'oient. 

En comparar les diferents corbes, es pot observar quines freqüències mantenen un comportament similar i quines disminueixen a mesura que augmenta l'angle. Aquesta informació permet analitzar la directivitat de l'altaveu i determinar fins a quin punt la resposta es manté uniforme fora de l'eix principal. 

#### **_Distorsió harmònica total_** 

La distorsió harmònica total, o THD, indica la proporció de components harmònics generats durant la reproducció respecte del senyal original. Com s'ha explicat anteriorment, aquests components poden aparèixer a causa de les no-linealitats dels diferents elements de l'altaveu. 

La THD es pot representar en funció de la freqüència i del nivell de pressió sonora. En general, un augment de la THD indica que el sistema està introduint més distorsió en aquella zona. 

El nivell de pressió sonora és especialment important, ja que en augmentar el volum també augmenta l'excursió del diafragma. Si aquesta excursió s'apropa als límits de funcionament del driver, les no-linealitats poden augmentar i, amb elles, la distorsió. 

#### **_Limitacions de les mesures acústiques_** 

Les mesures d'un altaveu poden estar afectades per l'entorn on es realitzen. Les reflexions produïdes per les parets, el terra, el sostre i altres superfícies poden arribar al micròfon juntament amb el so directe i modificar la resposta registrada. 

Per reduir aquest efecte es poden utilitzar tècniques com el “gating” temporal, que permet analitzar principalment el so directe abans que arribin les primeres reflexions. Aquesta tècnica és especialment útil a freqüències mitjanes i altes. 

28 

A freqüències baixes, però, la longitud d'ona és més gran i les reflexions es troben més relacionades amb el comportament de la sala. Per aquest motiu, la mesura dels greus presenta més dificultats i pot requerir mètodes específics per obtenir una representació fiable. 

## **_Marc pràctic:_** 

### **_Introducció:_** 

Un cop establerts els fonaments teòrics necessaris per entendre el funcionament d'un altaveu, aquest apartat es centra en l'aplicació pràctica d'aquests coneixements. L'objectiu d'aquest projecte és dissenyar i construir un altaveu d'alta fidelitat utilitzant recursos i coneixements relativament limitats, per posteriorment mesurar-ne el rendiment i comparar-lo amb models comercials de qualitat. A continuació es defineixen els requisits orientatius que guiaran el disseny: 

_Requisits orientatius:_ 

- _Reproducció màxima del espectre auditiu:_ 

Un so present des-de els baixos fins els aguts. 

- _Reproducció lineal fora d’eix (no estar “davant l’altaveu”):_ 

L’altaveu estarà col·locat en un espai de moviment, per tant es vol un so de qualitat independentment de la posició de l'oient. 

- _Distorsió mínima a volums elevats:_ 

La cuina es un lloc espaiós, per tant l’altaveu ha de poder assolir volums elevats sense saturar. 

- _Visualment agradable_ 

### **_Disseny de l’altaveu:_** 

29 

#### **_Arquitectura del sistema:_** 

Després d’investigació i prova de diferents opcions es va decidir construir la següent opció: 

- Altaveu de 3 vies amb port per baixos (3-way ported speaker) amb un crossover digital amplificat 

Aquesta configuració permet repartir el so en les 3 vies principals i, per tant, que cada altaveu funcioni en el seu rang òptim, evitant així distorsions o saturacions. A més, degut a la utilització d’un crossover digital, la dificultat del disseny del crossover es veu dràsticament reduïda, aspecte en el qual s’aprofundirà més endavant. 

Pel que fa a la disposició física dels altaveus en el “baffle” (part frontal), s'ha optat per col·locar el “tweeter”, el “mid-woofer” i el “woofer” de forma fo 2 ‘Tweeter desalineada en un eix vertical, situant el “bass port” al costat del “mid-woofer” (il·lustració 11). Aquesta configuració té com \ FA Fo Mid-woofer| a objectiu optimitzar la dispersió acústica i minimitzar la \ \ [a Pee \ }( ) cancel·lació de freqüències en el plànol horitzontal. NO ZZ ~ a 

La idea inicial era basar-se en el monitor d'estudi <u>ATC SCM25A</u> { \ ~~———__~~ / " \ <u>Pro Mk2, que té una disposició horitzontal. Tot i això, es va</u> decidir canviar aquest plantejament perquè els altaveus e. 74 horitzontals solen crear cancel·lacions de so quan l'oient es **Il·lustració 11 - "Baffle"** mou cap als costats. Per aquest motiu, el disseny va evolucionar cap a una topologia . vertical asimètrica, inspirada en el <u>JBL L100 Mk2</u> 

Aquesta estructura s'ha allotjat en un recinte de 12,8 litres amb un subcompartiment aïllat pel “mid-woofer” i el “tweeter”. 

#### **_Selecció de drivers:_** 

La selecció dels drivers per a un sistema de 3 vies s'ha de realitzar pensant en com s'enllacen els seus rangs de freqüència per poder fer les transicions entre drivers sense 

30 

deixar “buits”. Altres paràmetres com la sensibilitat o la impedància no són tan rellevants degut a l’ús d’un crossover digital: 

31 

- HiVi Swan M6N 6”, 8 Ω 

   - S'ha seleccionat com a woofer principal per la seva bona relació qualitatpreu i pel fet d'estar dissenyat específicament per a rendir en un recinte ventilat amb ‘bass port’. A més, s'ha escollit pel seu acabat de color coure (fet d'un aliatge de magnesi i alumini). 

- HiVi Swan M3N-B 3”, 8 Ω 

Degut a ser un altaveu de rang complet, destaca en la reproducció de mitjans, cosa que l’ha fet una elecció ideal per a complementar-lo amb el M6N de la mateixa família i el ‘tweeter’. 

- Dayton Audio ND25FW-4 1”, 4 Ω 

   - S'ha escollit per la seva Fs (freqüència de ressonància) baixa, la qual permet tallar l'altaveu a freqüències més greus de l'habitual sense patir distorsió. També destaca pel seu waveguide (guia d'ones) integrat, que ajuda a controlar la dispersió del so i a millorar notablement la resposta fora d'eix , tot presentant una excepcional relació qualitat-preu. 

#### **_Crossover:_** 

Amb 3 drivers diferents, el disseny i prova de les diferents separacions de freqüències, atenuacions individuals de cada driver i les correccions de fases haguessin comportat un procés massa tediós en una construcció passiva 



Per aquest motiu, s'ha optat per un disseny digital, que permet fer ajustos amb programari sense requerir modificació dels components ja instal·lats. Això ofereix una gran flexibilitat pel que fa al so final, permetent, per exemple, l'equalització a partir de l'habitació o la correcció del desfasament detectat en un dels altaveus. A més, això suposa un estalvi econòmic 

**Il·lustració 12 - "SigmaStudio", el programari per a** 

**configurar el crossover digital** 

32 

important durant la fase de "prototipatge", ja que permet provar diferents ajustos sense haver de comprar nous components cada vegada. 

En productes comercials, es pot preferir un crossover passiu per la seva simplicitat, cost de producció i relativa facilitat de reparació. El crossover digital s'ha implementat mitjançant tres components principals. L'unitat de comput actua com a receptor AirPlay, permetent rebre l'àudio sense fils directament des de dispositius Apple. Aquest senyal digital passa per un DAC (PCM5102), que el converteix a senyal analògic. Finalment, aquest senyal arriba al JAB4, que incorpora un DSP encarregat de separar el senyal en les tres vies i amplificar cada driver de manera independent. Tot això s'alimenta amb una única font d'alimentació, de manera que l'altaveu només requereix un cable extern. 

Els punts de tall entre vies (entre cada driver) s'han establert a 600 Hz (entre el “woofer” i el “mid-woofer”) i 2.500 Hz (entre el “mid-woofer” i el “tweeter”) per jo prioritzar la resposta fora d’eix. Per implementar-los, s'ha utilitzat un @ee\eD filtre Linkwitz-Riley de vuitè ordre (LR8), amb un pendent de 48 dB/oct, un tipus de filtre en què els dos drivers adjacents tanquen exactament a la mateixa freqüència, fent que, en sumar-se les seves respostes, el resultat sigui pla i sense pics ni caigudes al punt de tall. Tot i que la **Il·lustració 13 – “Baffle” de** diferència audible és petita, un pendent més pronunciat redueix encara **dues planxes d’MDF** més la superposició entre drivers adjacents. A més, en tractar-se d'un crossover digital, optar per un pendent més agressiu no comporta cap component addicional ni complexitat extra, a diferència del crossover passiu. 

**Il·lustració 13 – “Baffle” de dues planxes d’MDF** 

#### **_Disseny de la capsa:_** 

La capsa té un volum intern de 12,8 L, lleugerament per sota de l'objectiu inicial de 14 L (veure “Construcció dels altaveus”). Les dimensions externes són d'aproximadament 40x20x21 cm, amb un “baffle” (part frontal del altaveu) de MDF de 2 cm de gruix (ajuntant dos panells de 1cm, il·lustració 13) i la resta de panells en contraxapat d'1 cm. El mid- 

**Il·lustració 14 – Subcompartiment amb forma de “L”** 

33 

woofer i el tweeter estan allotjats en un subcompartiment aïllat amb forma de "L" (il·lustració 14). Aquesta forma permet aïllar els dos drivers sense afectar el “bass port” ni sacrificar un volum excessiu de la capsa, ja que cap d'aquests dos drivers necessita tant d'espai com el woofer. 

Degut al volum reduït de la capsa, el port bass-reflex té 5 cm de diàmetre i 18 cm de fondària, i està sintonitzat a uns 46 Hz. Aquesta freqüència, coneguda com a freqüència de sintonia de la caixa (Fb), correspon a la ressonància del sistema format pel volum d'aire de la caixa i l'aire contingut en el port. Al voltant d'aquesta freqüència, el port contribueix de manera significativa a la reproducció de les freqüències baixes i redueix l'excursió del woofer. Per sota de Fb, aquesta contribució disminueix ràpidament, la resposta acústica cau i l'excursió del woofer pot augmentar considerablement. 

En una primera versió, el port es va dissenyar amb una fondària d'uns 15-16 cm, però això sintonitzava la capsa per sobre de la freqüència desitjada, ja que la caixa va acabar sent més petita del calculat. Es va deixar el port als 18 cm actuals per corregir-ho. 

Per reduir vibracions i ressonàncies no desitjades, s'ha afegit un reforç estructural ("bracing", il·lustració 15) de dalt a baix i de dreta a esquerra, fet amb una barra de contraxapat d'uns 2 cm d'amplada **Il·lustració 15  – “Bracing”** i 1 cm de gruix. Aquest reforç és purament estructural, sense dividir l'interior de la capsa en compartiments separats. També, s'ha afegit farciment de polièster acústic per esmorteir l'interior de la capsa. 

**Il·lustració 15  – “Bracing”** 

### **_Construcció dels altaveus:_** 

El procés de construcció no va seguir estrictament un pla tancat des de l'inici. Un error d'arrodoniment en les dimensions externes de la caixa (uns 2 cm de més per banda) va donar un volum final superior al calculat inicialment. Tot i ser un error, això va acabar jugant a favor, ja que va evitar haver d'escurçar encara més el bass port. 

34 

Un cop el disseny acabat, es van tallar les fustes amb una serra circular de taula (il·lustració 15, 16 i 17) i es van encolar. Mentrestant, també es van fer els panells frontals ("baffles") on reposen els drivers. Els forats es van tallar amb serra de calar. 







**Il·lustració 15, 16, 17  – Tall de fustes** 

Amb la capsa completa, es va pintar, s'hi van afegir els suports estructurals interns, es va deixar assecar, es van passar els cables i es va segellar amb silicona. Tot seguit, es va col·locar el polièster acústic, es va posar el panell frontal, es va segellar i es va reforçar amb claus. 



<!-- Start of picture text -->
; 8 “ & } _<br><!-- End of picture text -->



<!-- Start of picture text -->
| % Ce Z| =-<br><!-- End of picture text -->

Finalment, es va soldar l’unitat de comput juntament amb el DAC (PCM5102), i es van fixar la font d'alimentació i el JAB4 a la part posterior de l'altaveu. Es van soldar els cables als drivers i es van connectar al JAB4. 

Resultat final: 

35 

36 

## **_Resultats i comparació:_** 

### **_Preu final:_** 

El cost total de construcció dels altaveus (parell) ha estat d'aproximadament **413 €** i **207 €** per unitat, desglossat de la següent manera: 

|**Preu final**||
|---|---|
|Drivers, bass port i|172€|
|Electrònica<br>(PSU,|79,79€|
|DAC...)||
|Amplificador|107€|
|Materials<br>(Fusta,|55€|
|pintura, cola)||
|**TOTAL**|413,79€|
|**TOTAL per unitat**|206,90€|



Aquest cost inclou tots els components electrònics, mecànics i de construcció necessaris per completar el parell d'altaveus, però no inclou el temps invertit en disseny, prototipatge i muntatge, ni eines ja disponibles prèviament (com la serra circular de taula). 

37 

### **_Introducció de productes:_** 

Per contextualitzar el rendiment i el cost de l'altaveu, es presenten a continuació les especificacions pròpies juntament amb les de dos productes comercials amb els quals es compararà l'altaveu. 

**Wharfedale Linton Heritage** : altaveu passiu de gamma mitjana-alta, amb un disseny clàssic de 3 vies no coaxial que separa verticalment cada driver, amb un “mid-range” fet de kevlar. Especificacions: resposta en freqüència de 40 Hz a 20 kHz (±3 dB), sensibilitat de 90 dB, i freqüències de tall a 630 Hz i 2,4 kHz. Preu: ~1.200-1.500 € el parell (sense suports). 



<!-- Start of picture text -->
© Erin's Audio Corner CEA2034 -- Wharfedale Linton 85 (Grille Off)<br>On Axis, = === Listening Window == Early Reflections === Sound Power<br>——= Sound Power DI = === Early Reflections DI == = = Dioffset<br>E 9085 J Vie eam : peeTAls fr:  eyon<br>3 75 .<br>S j<br>= 70<br>& f<br>2/<br>& 65 f<br>33 60 a<br>3 55<br>A<br>2 50<br>3 45 :<br>3<br>% 40 Le<br>100 1000 10000<br>Frequency<br>/ Hz<br><!-- End of picture text -->

**Genelec 8341A** : altaveu actiu professional amb DSP integrat, pensat per a estudis de gravació i monitoratge d'àudio. Incorpora tres amplificadors dedicats (un per driver) i calibratge de sala automàtic (GLM, programari de la empresa). Especificacions publicades: resposta en freqüència de 45 Hz a 20 kHz (±1,5 dB), SPL (com de “fort” pot sonar) màxim de 110 dB. Preu: ~4.620 € el parell. 

38 



<!-- Start of picture text -->
CEA2034 -- Genelec 8331A<br>—— OnAxis === = Listening Window ——=—— Early Reflections em= = Sound Power<br>1 og Sound Power DI! = mmm Early Reflections DI = = = = Di offset<br>100 eT aN A = X~<br>E 95 /<br>3 90 j<br>& 85 j<br>2 80 j<br>8{<br>=75 f<br>3<br>& j<br>2 70 /<br>8 65 |<br>é |<br>Ss 60 | hi)<br>8 NN<br>55 uv<br>100 1000 10000<br>Frequency / Hz © Erin's Audio Corner<br><!-- End of picture text -->

**Altaveu propi** : altaveu actiu de 3 vies amb crossover digital, punts de crossover a 600 Hz i 2.500 Hz. Resposta en freqüència d'aproximadament 40 Hz a 20 kHz (rang superior especificat pel fabricant del tweeter), amb variacions de ±3 dB en la resposta mesurada. Capsa de 12,8 L, amb port bass-reflex sintonitzat a 46 Hz. Preu: ~414 € el parell. 



<!-- Start of picture text -->
PL Sub bass Bass Low mid Nig Uppermid Presence Bila<br>95<br>85<br>a<br>/A<br>/<br>\ /<br>4 \/<br>© Vy,<br><!-- End of picture text -->

39 

### **_Comparació de rendiment:_** 

||_Disseny propi_|_Wharfedale_|_Genelec 8341A_|
|---|---|---|---|
|||_Linton Heritage_||
|_Resposta en_|40Hz–20kHz (±3dB)|40Hz–20kHz (±3dB)|45Hz–20kHz (±1,5dB)|
|_frequència_||||
|_THD* (Distorsió_<br>_harmònica_<br>_total)_|~1–3% entre 100Hz–<br>10kHz a ~77dB SPL|n/a|<2% entre 50-100Hz i<br><0,5% per sobre de<br>100Hz, a 90dB SPL|
|_Sensibilitat_|Actiu, no aplicable|90dB|Actiu, no aplicable|
|_SPL màxim*_|97dB (curt termini)|110dB (curt termini)|110dB (curt termini)|
|_(volum)_||||
|_Punts de_|600Hz / 2.500Hz, actiu|630Hz / 2.400Hz, passiu|500Hz / 3.000Hz, actiu|
|_crossover_||||
|_Preu (parell)_|~414€|~1.100–1.500€|~4.500–4.620€|



* Les dades de THD i SPL màxim no són directament comparables, ja que s'han obtingut sota diferents nivells de pressió sonora i condicions i mètodes de mesura. Tot i això, s'inclouen com a referència per poder contextualitzar els resultats obtinguts en aquest projecte respecte dels models comercials. 

#### **_Metodologia de mesura:_** 

Les mesures s'han realitzat amb un micròfon ECM8000 i el programari REW, utilitzant tres mesures independents. Dues d'elles corresponen a mesures de near field, una realitzada directament sobre el woofer i l'altra sobre el port de baixos. Aquest tipus de mesura permet analitzar amb més precisió el comportament de les freqüències baixes, on les reflexions de la sala poden afectar considerablement el resultat. 

40 

La tercera mesura correspon a una mesura a 1 metre amb “gating” temporal. Aquesta tècnica permet eliminar de la mesura, dins d'un determinat interval de temps, les reflexions de les parets i altres superfícies de la sala. D'aquesta manera, es pot obtenir una resposta més representativa del comportament de l'altaveu a freqüències mitjanes i altes. 

A diferència dels fabricants, que poden realitzar les seves mesures en cambres anecoiques o en altres condicions controlades, aquestes mesures s'han realitzat en un entorn domèstic. A més, l'ECM8000 utilitzat no disposa d'un calibratge individual verificat, fet que pot introduir desviacions en els valors absoluts obtinguts. En determinades freqüències, aquestes desviacions poden arribar a ser, en casos extrems, de l'ordre de 5 dB, per la qual cosa els valors absoluts s'han d'interpretar amb certa cautela. Tot i això, aquesta possible desviació del sistema de mesura és independent de la variació observada en la resposta de l'altaveu. Així, el marge aproximat de ±3 dB observat en la corba descriu la variació de la resposta mesurada i no l'error del micròfon. 

#### **_El so:_** 

L’altaveu construït aconsegueix una resposta en freqüència (40 Hz–20 kHz, ±3 dB) molt similar a la del Wharfedale Linton Heritage i propera a la del Genelec 8341A. Aquesta similitud indica que, en termes de resposta en freqüència, les diferències entre el prototip i els models comercials analitzats són relativament reduïdes. 

Tot i que això no permet afirmar que els tres sistemes siguin acústicament equivalents en tots els aspectes, les diferències observades en la resposta en freqüència no necessàriament resulten fàcils de percebre en una escolta convencional. La capacitat per identificar diferències petites en la reproducció sonora depèn, entre altres factors, de l’experiència auditiva de l’oient, de les condicions d’escolta i de la magnitud i naturalesa de les diferències existents. Per tant, per a un oient sense experiència específica en escolta crítica, aquestes diferències poden resultar poc, sinó gens, evidents, especialment en una escolta no comparativa. 

41 

Així, els resultats obtinguts suggereixen que el prototip pot oferir una experiència de reproducció sonora propera a la dels models comparats en els aspectes analitzats, tot i que no es pot considerar equivalent a aquests en termes globals, ja que existeixen diferències en altres paràmetres, com el SPL màxim, la distorsió i les prestacions associades al sistema d’amplificació i calibratge. 

#### **_Acabat i construcció:_** 

Com a disseny artesanal, la construcció d'un altaveu propi pot generar un vincle personal i un valor afectiu entre el creador i l'objecte que un producte fabricat en sèrie no pot aportar, gràcies al disseny a mida i a les petites diferències que fan única cada unitat. Ara bé, aquest caràcter artesanal depèn directament de l'habilitat de qui el construeix.  Per contra, el Genelec 8341A utilitza una carcassa d'alumini injectat amb toleràncies mínimes, i el Wharfedale Linton Heritage un xapat de fusta natural amb control de qualitat industrial. La consistència i precisió d'acabat d'aquests productes comercials, evidentment, no es pot igualar amb eines i experiència limitades. 

#### **_“Diminishing returns”:_** 

El concepte de diminishing returns (rendiments decreixents) descriu com, a partir d'un cert punt, cada unitat addicional d'inversió produeix una millora cada cop més petita. Aquest projecte n'és un exemple clar: amb un pressupost molt limitat (~414€/parell) s'ha aconseguit una resposta en freqüència (40Hz-20kHz ±3dB) comparable a la del Linton Heritage (~1.100-1.500€/parell) i no gaire lluny de la del Genelec 8341A (±1,5dB, ~4.620€/parell). Multiplicar el pressupost per 3 o per 10 no implica multiplicar el rendiment acústic en la mateixa proporció. A partir d'un cert nivell, cada increment addicional d'inversió pot produir millores progressivament més petites en el rendiment acústic. 

#### **_Dependència de la configuració del crossover digital:_** 

A diferència del Genelec 8341A, que ve calibrat de fàbrica i disposa d'eines de calibratge automàtic (GLM), el rendiment del disseny propi depèn directament de qui configura el 

42 

crossover. Un exemple concret és la inversió de fase del tweeter en un dels dos altaveus, detectada per una caiguda a la resposta al punt de tall i corregida manualment amb programari; sense aquesta detecció, l'altaveu hauria quedat amb un error de configuració permanent. Això posa de manifest una limitació estructural del disseny: el resultat final no és fix com en un producte comercial acabat, sinó tan bo com el coneixement tècnic de la persona que l'ajusta. 

### **_Comparació de preu:_** 

El cost total del prototip és d’aproximadament 413 € per parell, una quantitat considerablement inferior a la dels dos models comercials utilitzats com a referència. El Wharfedale Linton Heritage té un preu aproximat d’entre 1.100 i 1.500 € per parell, 

mentre que el Genelec 8341A se situa al voltant dels 4.500 € per parell. En comparació, el disseny propi representa aproximadament entre un 27 i un 38 % del cost del Linton, i menys d’un 10 % del cost del Genelec. 

Aquesta diferència de preu és especialment significativa si es té en compte que el prototip aconsegueix unes prestacions acústiques comparables en alguns dels paràmetres analitzats, especialment pel que fa a la resposta en freqüència. Per tant, el projecte mostra que una inversió econòmica molt inferior pot permetre assolir un nivell de rendiment acústic elevat, tot i que els productes comercials continuen oferint avantatges en altres aspectes, com la potència màxima, les toleràncies de fabricació, el control de qualitat i la integració del sistema. 

Cal tenir en compte, però, que aquest resultat depèn directament dels coneixements i de l’experiència de la persona que dissenya i ajusta el sistema. En un altaveu amb crossover digital, una configuració incorrecta dels nivells, les freqüències de tall o la fase pot deteriorar considerablement el resultat final. Per tant, el cost reduït del projecte no 

43 

implica que es puguin obtenir les mateixes prestacions sense els coneixements tècnics necessaris per dissenyar, mesurar i ajustar correctament el sistema. 

A més, el baix cost econòmic no representa el cost total del projecte. Una part important de la inversió s’ha realitzat en forma de temps i treball, dedicats al disseny, la fabricació de les caixes, el muntatge, les mesures acústiques, la configuració del DSP i els diferents ajustos i proves. D’aquesta manera, el projecte substitueix una part de la inversió econòmica pròpia dels productes comercials per una inversió considerable d’hores de treball i coneixement tècnic. 

## **_Conclusió:_** 

En conclusió, el projecte demostra que és possible construir un sistema d’altaveus de tres vies amb un cost relativament reduït i obtenir unes prestacions acústiques elevades, comparables a les de productes comercials. El prototip presenta una resposta en freqüència de 40 Hz a 20 kHz dins d’un marge de ±3 dB, comparable amb la del Wharfedale Linton Heritage i propera a la del Genelec 8341A, tot i existir diferències en altres aspectes tècnics, com la distorsió, el nivell de pressió sonora màxim o el sistema de calibratge. 

Aquesta proximitat en la resposta mesurada també té una conseqüència important des del punt de vista de l’escolta. Les diferències entre els sistemes no necessàriament són fàcils de percebre en una escolta convencional i, per a un oient sense experiència específica en escolta crítica, poden resultar poc, si no gens, perceptibles, especialment quan no es realitza una comparació directa i controlada. Per tant, la diferència de preu entre els sistemes no es tradueix necessàriament en una diferència de qualitat sonora fàcilment audible. 

Tanmateix, això no significa que el prototip sigui tècnicament equivalent als models comercials. Aquests ofereixen avantatges en aspectes com la capacitat de reproducció a nivells elevats, les toleràncies de fabricació, el control de qualitat i, en el cas del Genelec 8341A, els sistemes de calibratge. El disseny propi, en canvi, permet un control molt més 

44 

directe sobre el sistema, especialment gràcies al crossover digital, però fa que el resultat final depengui dels coneixements i de la precisió de qui el dissenya, construeix i ajusta. 

Finalment, cal tenir en compte que les mesures s’han realitzat en un entorn domèstic i amb un micròfon sense calibratge individual verificat, de manera que els valors obtinguts no poden considerar-se equivalents a mesures de laboratori. Tot i això, són suficients per analitzar les tendències i situar el comportament del prototip respecte dels models de referència. En conjunt, els resultats mostren que una part important del rendiment acústic d’un altaveu comercial de gamma alta es pot assolir mitjançant un procés de disseny, construcció, mesura i ajust adequadament plantejat, sense que l’increment del cost impliqui necessàriament una diferència de qualitat sonora fàcilment perceptible per a qualsevol oient. 

## **_Bibliografia_** 

**Invalid source specified.** 

45 

