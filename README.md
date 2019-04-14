


![](https://www.bayard-jeunesse.com/wp-content/uploads/2018/05/ACT-CAR-Harcelement.jpg "Illustration Le harcelement")

<p>&nbsp; </p>

# Description du projet


<div align="justify">Bullying is unwanted, aggressive behavior among school aged children that involves a real or perceived power imbalance. The behavior is repeated, or has the potential to be repeated, over time. Both kids who are bullied and who bully others may have serious, lasting problems.
Bullying can take on many forms which are just as emotionally and psychologically damaging as physical intimidation and harassment. There are three general forms of bullying: Verbal bullying, Physical bullying and cyberbullying.
Generally, people who are bullied have one or more risk factors like mental disorder, different race or ethnicity, different sexual orientation…</div>


<div align="justify">Our project creates a small environnement that shows us the evolution of the victim's condition according to an initial situation. The aim is to represent how the victim's condition can evolve by adding harassers or friends.</div>

<p>&nbsp; </p>


  
# Modélisation

<div align="justify">Notre projet cherche à représenter selon certaines conditions l'état d'une victime d'un harcèlement, en reflétant la réalité avec le maximum de situations possibles. Notre objectif est de montrer que cet état peut évoluer selon le type d'individu qui l'entoure. Dans un premiers temps, il sera décrit le modèle d'étude utilisé pour illustrer le phénomène, puis les paramètres disponibles seront énoncés. Enfin la dynamique du système sera explicité à l'aide d'un exemple.</div>

<p>&nbsp; </p>

## Le modèle d'étude
 
<div align="justify">Dans le but de modéliser le harcèlement, nous avons aménagé un environnement à l'aide de Tkinter. Nous avons simplifié le phénomène pour créer un modèle d'étude qui présente une victime, son (ou ses) harceleur(s), son entourage et des personnes neutres.</div>
<p>&nbsp; </p>

<div align="justify">Dans l'environnement chaque individu est représenté par un cercle coloré selon son influence (positive ou négative) sur la victime :</div>

* Rouge et rouge clair : harceleurs
* Vert : entourage de la victime
* Blanc : individu neutre



<div align="justify">La victime est elle aussi représentée par un cercle, qui selon sa couleur, décrit un état plus ou moins atteint par le harcèlement qu'elle subit :</div>

* Cyan : peu atteint
* Bleu : moyennement atteint
* Noir : très atteint
<p>&nbsp; </p>

<div align="justify">Afin de faciliter la lisibilité du modèle, nous avons organisé ces différents cercles de telle sorte à ce qu'ils suivent une orbite prédefinie autour de la victime selon son statut dans l'environnement (harceleurs, neutres ou amis).</div>

<p>&nbsp; </p>
<div align="justify">Pour cela, on crée un cercle "Balle" puis on lui donne une vitesse pour enfin le faire apparaître et suivre l'orbite souhaitée à l'aide de coordonnées défini préalablement. On applique ce concept aux différents cercles présent dans l'environnement.</div>
<p>&nbsp; </p>

    1. Balle = canvas.create_oval(X,Y,X,Y,fill='white')
    2. cangle=cmath.exp(0.09j)
       V=cangle*complex(X,Y)       
    3. canvas.coords(Balle,XC+X-RAYON,YC+Y-RAYON,XC+X+RAYON,YC+Y+RAYON)
<p>&nbsp; </p>

![](https://www.cjoint.com/doc/19_04/IDowje6tal6_orbite2.PNG "Organisation de l'environnement")



<p>&nbsp; </p>



## Paramètres pris en compte

<div align="justify">Dans un premier temps, l'action de l'utilisateur est requise pour générer une situation initiale qui évoluera dans un temps donné (30 secondes dans notre cas), où nous pouvons supposer qu'une seconde correspond à une semaine durant laquelle la victime est harcelée. La situation initiale varie selon une cause et un type d'harcèlement sélectionnés comme le montre le tableau ci dessous.</div>

<p>&nbsp; </p>

![](https://www.cjoint.com/doc/19_04/IDnqnAmb8n6_Tableau-des-conditions-initiales-2.PNG "Conditions initiales possibles") 

<p>&nbsp; </p>


## La dynamique du système


<div align="justify">Une fois la situation initiale créée, le groupe d'harceleur apparait au lancement du programme. Au bout de quelques secondes, le groupe s’attaque à un individu qui devient alors la victime. Au cours du temps, son état peut s'améliorer ou s'aggraver. Pour prévenir de possibles changements d'état, ceux-ci sont précédés d'un état "intermédiaire" illustré graphiquement par une variation rapide de la couleur de la victime.  </div>
 
 


<div align="justify">Dans l'exemple ci-dessous, l'utilisateur a sélectionné la cause "Origine, ethnie", le type d'harcèlement "Verbal" et le nombre d'amis "1".</div>

<p>&nbsp; </p>




<div align="justify">Le groupe d'harceleurs est alors composé de 2 individus. Lorsqu'il s'attaque à la victime, cette dernière apparaît et est tout d'abord dans l'état "peu atteinte" :  </div>     



![](https://www.cjoint.com/doc/19_04/IDnuzZd2H46_t5.jpg "Apparition de la victime")  

<p>&nbsp; </p>

<div align="justify">Ensuite la victime passe d'un état "peut atteint" à un état "moyennement atteint":  </div>   



![](https://www.cjoint.com/doc/19_04/IDnuAbJVOa6_t15.jpg "Changement d'etat")  

<p>&nbsp; </p>



<div align="justify">Une fois son entourage apparu, un nouvel état peut s'appliquer à la victime. Dans cet exemple,  le nombre d'amis n'étant pas à la faveur de la victime, son état empire. Elle passe donc de l'état "moyennement atteint" à l'état "très atteint" :   </div>   



![](https://www.cjoint.com/doc/19_04/IDnuAuUD266_t27.jpg "Apparation de l'entourage et résultat sur la victime")  


<p>&nbsp; </p>

# Conclusion

<div align="justify">Les différentes situations initiales possibles, à l'aide des causes et des types d'harcèlement, autorisent une variété de résultats sur l'état final de la victime. En tentant d'ajouter le maximum de paramètres, nous avons pu nous rapprocher au mieux de la réalité. En effet notre modèle d'étude décrit aussi bien l'isolement de la victime que l'intensité du harcèlement qu'elle subit. Néanmoins, il reste quelques facteurs du harcèlement qui ne sont pas décrits par notre projet comme le sexe de la victime par rapport à celui de ses harceleurs (une femme entourée d'hommes ou l'inverse), ainsi que l'influence qu'à la victime sur son entourage (l'aggressivité par exemple) pouvant petit à petit le négliger.</div>


<p>&nbsp; </p>

# Membres du groupe

+ AHMED ELADAWI Haïcem
+ ELGHOUL Elio
+ HU Dylan

<p>&nbsp; </p>

# Bibliograpgie

https://nospensees.fr/5-types-de-harcelement-a-lecole/


http://www.i-share.fr/actualite/le-harcelement-scolaire-quen-est-il-en-2018


https://etudiant.lefigaro.fr/article/enquete-sur-le-harcelement-scolaire-les-filles-sont-surrepresentees-_596f11e6-c554-11e7-b5ea-cfc166fd55ef/  


https://www.nonauharcelement.education.gouv.fr/wp-content/uploads/2012/01/guide_pratique_le_harcelement_entre_eleves1.pdf


https://www.unicef.fr/sites/default/files/userfiles/UNICEF_FRANCE_violences_scolaires_mars_2011.pdf


