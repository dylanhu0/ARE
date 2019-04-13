


![](https://www.bayard-jeunesse.com/wp-content/uploads/2018/05/ACT-CAR-Harcelement.jpg "Illustration Le harcelement")

<p>&nbsp; </p>

# Description du projet


<div align="justify">Bullying is unwanted, aggressive behavior among school aged children that involves a real or perceived power imbalance. The behavior is repeated, or has the potential to be repeated, over time. Both kids who are bullied and who bully others may have serious, lasting problems.
Bullying can take on many forms which are just as emotionally and psychologically damaging as physical intimidation and harassment. There are three general forms of bullying: Verbal bullying, Physical bullying and cyberbullying.
Generally, people who are bullied have one or more risk factors like mental disorder, different race or ethnicity, different sexual orientation…


<div align="justify">Our project creates a small environnement that shows us the evolution of the victim's condition according to an initial situation. The aim is to represents how the victim's condition can evolve by adding harassers or friends.</div>

<p>&nbsp; </p>


  
# Modélisation

<div align="justify">Notre projet représente selon certaines conditions l'état d'une victime d'un harcèlement. Tout en refléter la réalité avec le maximum de situations possible, notre objectif est de montrer que cet état peut évoluer selon le type d'individu qui l'entoure.</div>

<p>&nbsp; </p>

## Le modèle d'étude
 
<div align="justify">Dans le but de modéliser le harcèlement, nous avons aménagé un environnement à l'aide de Tkinter. Nous avons simplifié le phénomène pour créer un modèle d'étude qui présente une victime, son (ou ses) harceleur(s), son entourage et des personnes neutres.</div>
<p>&nbsp; </p>

<div align="justify">Dans l'environnement chaque individu est représenté par un cercle coloré selon son influence (positive ou négative) sur la victime :</div>

* Rouge et rouge clair : harceleur
* Vert : entourage de la victime
* Blanc : individu neutre
<p>&nbsp; </p>

<div align="justify">La victime est elle aussi représentée par un cercle, qui selon sa couleur décrit un état plus ou moins atteint par le harcèlement qu'elle subit :</div>

* Cyan : peu atteint
* Bleu : moyennement atteint
* Noir : très atteint
<p>&nbsp; </p>

<div align="justify">Afin de faciliter la lisibilité du modèle, nous avons organisé ces différents cercles de telle sorte à ce qu'ils suivent une orbite autour de la victime.</div>

* Image : Organisation des cercles

<p>&nbsp; </p>

## Paramètres pris en compte

<div align="justify">L'environnement nécessite dans un premier temps l'action de l'utilisateur pour générer une situation initiale qui évoluera dans un temps donné : 30 secondes dans notre cas, où nous pouvons supposer qu'une seconde correspond à un mois durant lequel la victime est harcelée. La situation initiale varie selon une cause et le(s) type(s) d'agression sélectionnés comme le montre le tableau ci dessous :</div>



<div style="image-align:center"><div align="center"><img src=https://www.cjoint.com/doc/19_04/IDnlPVPr416_Tableau-des-conditions-initiales.PNG "Illustration conditions initiales" /></div> 



<p>&nbsp; </p>

<div align="justify">Au cours du temps, et cela à partir des conditions initiales imposées par l'utilisateurs, l'état de la victime empire ou s'améliore.</div>

