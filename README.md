# Description du projet


<div align="justify">Bullying is unwanted, aggressive behavior among school aged children that involves a real or perceived power imbalance. The behavior is repeated, or has the potential to be repeated, over time. Both kids who are bullied and who bully others may have serious, lasting problems.
Bullying can take on many forms which are just as emotionally and psychologically damaging as physical intimidation and harassment. There are three general forms of bullying: Verbal bullying, Physical bullying and cyberbullying.
Generally, people who are bullied have one or more risk factors like mental disorder, different race or ethnicity, different sexual orientation…
  
<p>&nbsp; </p>

According to NSCS(National School Climate Survey) 35.3% of students with behavioral and emotional disorders, 25% of African-American students, 74.1% of LGBT students were all bullied.
Research has found that children and adolescents who have been bullied can experience negative psychological(depression, anxiety), physical(being injured from a physical attack), and academic effects(impact on grades) .
However, inclusion and friendship can have extremely positive effects on kids and teens lives and their mental states. Making friends is a social skill that is important, not for popularity purposes, but purely because friendship can provide many benefits and lower the risk of getting bullied.

<p>&nbsp; </p>

Our project demonstrates, hypothetically, the effect of the victim when bullied. With Tkinter, we were able to create a small environnement representing the scene. Each person is represented with a small circle: The victim with a popping circle, the bullies with a red circle, the friends with a green circle and people who don’t take actions are represented with a white circle.

<p>&nbsp; </p>

  
# Modélisation



## Le modèle d'étude


 
  Dans le but de modéliser le harcèlement, nous avons aménagé un environnement à l'aide de Tkinter. Nous avons simplifié le phénomène pour créer un modèle d'étude qui présente une victime, son (ou ses) harceleur(s), son entourage et des personnes neutres. En plus de cela, une échelle de temps a été introduite pour témoigner de l'évolution.

  Dans l'environnement chaque individu est représenté par un cercle coloré selon son influence (positive ou négative) sur la victime :     

* Rouge et rouge clair : harceleur
* Vert : entourage de la victime
* Blanc : individu neutre

  La victime est elle aussi représentée par un cercle, qui selon sa couleur décrit un état plus ou moins atteint par le harcèlement qu'elle subit :

* Cyan : peu atteint
* Bleu : moyennement atteint
* Noir : très atteint

  Afin de faciliter la lisibilité du modèle, nous avons organisé ces différents cercles de telle sorte à ce qu'ils suivent une orbite autour de la victime.

* Image : Organisation des cercles



## Paramètres pris en compte

Pour commencer, l'environnement nécessite dans un premier temps l'action de l'utilisateur pour générer une situation initiale qui évoluera dans un temps donné : 30 secondes dans notre cas où nous pouvons supposer que un mois réel vaut une seconde par exemple.
La situation initiale varie selon une cause et le(s) type(s) sélectionnés comme le montre le tableau ci dessous :

* Image : Tableau C1 T1 etc...

Au cours du temps, et cela à partir des conditions initiales imposées par l'utilisateurs, l'état psychologique de la victime empire ou s'améliore.</div>

