# Statistiques et visualisation du métro de Rennes

## 1. Information

<p align="justify">
Ce document propose une analyse statistique et une visualisation du métro de Rennes. 
Les données proviennent du site Rennes Métropole (https://data.rennesmetropole.fr/page/home/). 
Ces données sont dans un premier temps acquises grâce a l'API du site et sont ensuite adaptées
en vue de leur analyse et visualisation. La visualisation est réalisée avec la librairie "bokeh".
</p>

## 2. Statistiques

<p align="justify">
La ville de Rennes possède une ligne de métro (ligne a) depuis 2002. Cette ligne transporte environ 140 000 passagers par jour.
 Une deuxième ligne (ligne b) est actuellement en construction dont l'ouverture est prévue pour 2020.
</p>

**Tableau 1: Chiffres-clés sur les infrastructures**

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

## 3. Visualisation

**Carte 1: Localisation des stations de métro (Cliquez sur l'image pour l'interactivité!)**

<p align="center">
  <a href="https://florentdsgree.github.io/TransportRennesMetropole/MetroRennes/MetroRennes.html">
  <img src="https://florentdsgree.github.io/TransportRennesMetropole/MetroRennes/MetroRennes.PNG" width="400"/>
  </a>
</p>
