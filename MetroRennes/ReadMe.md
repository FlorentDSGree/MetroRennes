# Statistiques et visualisation du métro de Rennes

## 1. Information

<p align="justify">
Ce document propose une analyse statistique et une visualisation du métro de Rennes. 
Les données proviennent du site Rennes Métropole (https://data.rennesmetropole.fr/page/home/). 
Ces données sont dans un premier temps acquises grâce a l'API du site et sont ensuite adaptées
en vue de leur analyse et visualisation. La visualisation est réalisée avec la librairie "bokeh".
</p>

## 2. Statistiques et analyses

<p align="justify">
La ville de Rennes possède une ligne de métro (ligne a) depuis 2002. Cette ligne transporte environ 140 000 passagers par jour.
 Une deuxième ligne (ligne b) est actuellement en construction dont l'ouverture est prévue pour 2020.
</p>

### 2.1. Analyse des stations de métro

**Tableau 1: Chiffres-clés sur les stations de métro**

|                                               |Ligne a                           |Ligne b                             |
|-----------------------------------------------|---------------------------------:|-----------------------------------:|
|Nombre de station                              | 15                               | 15                                 |
|Terminus 1                                     | J.F. Kennedy                     | Saint-Jacques-Gaité                |
|Terminus 2                                     | La Poterie                       | Cesson Viasilva                    |
|Distance euclidienne entre les terminus        | 6.2km                            | 7.6km                              |
|Distance euclidienne moyenne entre 2 stations  | 583m                             | 800m                               |
|Distance euclidienne médiane entre 2 stations  | 552m                             | 776m                               |
|Distance euclidienne minimale entre 2 stations | 378m<br>Charles de Gaulle - Gares| 535m<br>Saint Germain - Sainte Anne|
|Distance euclidienne maximale entre 2 stations | 782m<br>Gares - Jacques Cartier) | 1 116m <br>Cleunay - Mabilais       |

*La distance euclidienne est la distance la plus courte entre deux points ("vol d'oiseau").*

**Figure 1: Distribution de la distance euclidienne entre 2 stations pour les 2 lignes de métro**
<p align="center">
  <a href="https://florentdsgree.github.io/TransportRennesMetropole/MetroRennes/DistributionDistanceEuclidienneEntreStations.html">
  <img src="https://florentdsgree.github.io/TransportRennesMetropole/MetroRennes/DistributionDistanceEuclidienneEntreStations.png" width="400"/>
  </a>
</p>

<p align="justify">
Les deux lignes de métro comportent le même nombre de station (15), cependant la ligne b est plus longue que la ligne a de 1.4km (+22.6%). Les distances euclidiennes moyennes, minimales et maximales entre deux stations sont plus importante pour la ligne b que pour le ligne a. La figure 1 confirme le plus grand espacement entre les stations de la ligne b.
</p>

### 2.2. Analyse du tracé des lignes de métro

**Tableau 2: Chiffres-clés sur le tracé des lignes de métro**

| Longueur          | Ligne a | Ligne b |Difference (a-b)|
|:------------------|--------:|--------:|---------------:|
|Totale             | 9 696m  | 13 727m | -4 031m (-42%) |
|Entre terminus     | 8 587m  | 12 949m | -4 362m (-51%) |
|Tunnel             | 3 680m  | 8 062m  | -4 382m (-119%)|
|Tranchée couverte  | 3 030m  | 1 782m  | 1 248m (+41%)  |
|Viaduc             | 945m    | 2 077m  | -1 132m (-120%)|
|Station            | 537m    | 919m    | -382 m (-71%)  |
|Zone de transition | 395m    | 109m    | 286m (+72%)    |

<p align="justify">
La longueur totale comprend les zones qui ne sont pas utilisées pour le transport de voyageurs, elles correspondent aux voies de service. Elles représentent un part une part non négligéable des voies, 11,4% de la ligne a et 5,6% de la ligne b. La ligne b est plus longue que la ligne a d'environ 50%. Les voies en tunnel de la ligne b sont quasiment équivalente à la longueur entre terminus de la ligne a, 8 062m contre 8 587m respectivement. Le nombre de station est similaire pour les deux lignes (15), cependant la longueur des voie en station est plus longue pour la ligne b d'environ 30%.
</p>

**Figure 2: Distribution de la longueur des voies de métro par type de voie**

<p align="center">
  <a href="https://florentdsgree.github.io/TransportRennesMetropole/MetroRennes/LongueurVoieMetro.html">
  <img src="https://florentdsgree.github.io/TransportRennesMetropole/MetroRennes/LongueurVoieMetro.PNG" width="400"/>
  </a>
</p>

## 3. Visualisation

**Carte 1: Localisation des stations de métro (Cliquez sur l'image pour l'interactivité!)**

<p align="center">
  <a href="https://florentdsgree.github.io/TransportRennesMetropole/MetroRennes/MetroRennes.html">
  <img src="https://florentdsgree.github.io/TransportRennesMetropole/MetroRennes/MetroRennes.PNG" width="400"/>
  </a>
</p>


## 4. Autres informations

**Tableau 3: Distances entre stations de la ligne a**

|Station 1           |Station 2            | Distance euclidienne [m]|
|--------------------|---------------------|------------------------:|
|J.F. Kennedy        |	Villejean-Université|	544
|Villejean-Université|	Pontchaillou        |	782
|Pontchaillou       	| Anatole France      |	574
|Anatole France     	| Sainte-Anne         |	662
|Sainte-Anne	        | République          |	539
|République	         | Charles de Gaulle   |	509
|Charles de Gaulle   |	Gares               |	378
|Gares	              | Jacques Cartier     |	782
|Jacques Cartier     |	Clemenceau          |	458
|Clemenceau	         | Henri Fréville      |	646
|Henri Fréville      |	Italie              |	528
|Italie	             | Triangle            |	560
|Triangle            |	Le Blosne           |	474
|Le Blosne	          | La Poterie          |	721

**Tableau 4: Distances entre stations de la ligne b**

|Station 1           |Station 2            | Distance euclidienne [m]|
|--------------------|---------------------|------------------------:|
|Saint-Jacques-Gaité |	La Courrouze        |	630
|La Courrouze        |	Cleunay             |	775
|Cleunay             |	Mabilais            |	1 116
|Mabilais            |	Colombier           |	784
|Colombier           |	Gares               |	770
|Gares               |	Saint Germain       |	776
|Saint Germain	      | Sainte Anne         |	535
|Sainte Anne         |	Jules Ferry         |	808
|Jules Ferry         |	Gros Chêne          |	854
|Gros Chêne          |	Les Gayeulles       |	715
|Les Gayeulles       |	Irène Joliot-Curie  |	728
|Irène Joliot-Curie  |	Beaulieu Université |	945
|Beaulieu Université |	Atalante            |	994
|Atalante            |	Cesson Viasilva     |	763
