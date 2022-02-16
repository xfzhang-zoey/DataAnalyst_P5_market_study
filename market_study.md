# DataAnalyst_P5_market_study
Aider une entreprise agroalimentaire de réaliser une étude de marché international pour mieux cibler ses nouveaux pays clientèle. 

**Highlights: **

- Descriptive statistics, 
- Clustering (hierarchical classification, K-means), 
- Principal Component Analysis, 
- Statistical inference analysis (statistical hypothesis test: Chi-squared test for variance in a normal distributed population, test IID) 

**Prérequis**

Pour effectuer ce projet, vous devrez maîtriser la manipulation de données en Python ou R, appliquer ces langages à la **statistique descriptive** ainsi qu'à la **classification automatique**.


**Scénario**

Votre entreprise d'agroalimentaire souhaite se développer à l'international. Elle est spécialisée dans le poulet !

L'international, oui, mais pour l'instant, le champ des possibles est bien large : aucun pays particulier ni aucun continent n'est pour le moment choisi. Tous les pays sont envisageables !

Votre objectif sera d'**aider à cibler plus particulièrement certains pays**, dans le but d'**approfondir ensuite l'étude de marché**. Plus particulièrement, l'idéal serait de produire des "groupes" de pays, plus ou moins gros, dont on connaît les caractéristiques.

Dans un premier temps, la stratégie est plutôt d'exporter les produits plutôt que de produire sur place, c'est-à-dire dans le(s) nouveau(x) pays ciblé(s).


**Les données**

Vous vous souvenez de la FAO, dans l'un de vos précédents projets ? Allez, on y retourne ! Vous connaissez déjà l'interface du site, à vous de retrouver les données qui vous seront utiles pour le projet.


**Votre mission**

Pour identifier les pays propices à une insertion dans le marché du poulet, il vous a été demandé de cibler les pays. Il vous faudra également étudier les régimes alimentaires de chaque pays, notamment en termes de protéines d'origine animale et en termes de calories.

Construisez votre échantillon contenant l'ensemble des pays disponibles, chacun caractérisé par ces variables :

- différence de population entre une année antérieure (au choix) et l'année courante, exprimée en pourcentage ;
- proportion de protéines d'origine animale par rapport à la quantité totale de protéines dans la disponibilité alimentaire du pays ;
- disponibilité alimentaire en protéines par habitant ;
- disponibilité alimentaire en calories par habitant.

Construisez un dendrogramme contenant l'ensemble des pays étudiés, puis coupez-le afin d'obtenir 5 groupes.

Caractérisez chacun de ces groupes selon les variables cités précédemment, et facultativement selon d'autres variables que vous jugerez pertinentes (ex : le PIB par habitant). Vous pouvez le faire en calculant la position des centroïdes de chacun des groupes, puis en les commentant et en les critiquant au vu de vos objectifs.

Donnez une courte liste de pays à cibler, en présentant leurs caractéristiques. Un découpage plus précis qu'en 5 groupes peut si besoin être effectué pour cibler un nombre raisonnable de pays. 

Visualisez vos  partitions dans le premier plan factoriel obtenu par ACP.

Dans votre partition, vous avez obtenu des groupes distincts. Vérifiez donc qu'ils diffèrent réellement. Pour cela, réalisez les tests statistiques suivants :

- **un test d'adéquation** : parmi les 4 variables, ou parmi d'autres variables que vous trouverez pertinentes, trouvez une variable dont la loi est normale ;
- **un test de comparaison** de deux populations (dans le cas gaussien) : choisissez 2 clusters parmi ceux que vous aurez déterminé. Sur ces 2 clusters, testez la variable gaussienne grâce à un test de comparaison.
