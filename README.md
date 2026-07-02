# Rapport d'analyse de l'attrition des clients d'une entreprise de télécommunications

## Introduction

Dans le secteur des télécommunications, la fidélisation des clients constitue un enjeu stratégique majeur. Le coût d'acquisition d'un nouveau client étant généralement supérieur au coût de rétention d'un client existant, comprendre les facteurs qui conduisent les abonnés à résilier leur contrat représente une priorité pour les entreprises.

Ce projet a été réalisé à l'aide de Microsoft Power BI afin d'exploiter un jeu de données relatif aux abonnés d'une entreprise de télécommunications. L'objectif est d'identifier les principaux facteurs expliquant l'attrition (Churn), de déterminer les profils de clients les plus susceptibles de quitter l'entreprise et de proposer des recommandations permettant de réduire ce phénomène.

---

# Énoncé du problème métier

L'entreprise fait face à une perte régulière de clients, entraînant une diminution de son chiffre d'affaires et une augmentation des coûts liés à l'acquisition de nouveaux abonnés.

Cette analyse cherche à répondre aux trois questions suivantes :

* Pourquoi les clients résilient-ils leur abonnement ?
* Quels sont les profils de clients les plus susceptibles de quitter l'entreprise prochainement ?
* Quelles actions peuvent être mises en œuvre afin de réduire durablement le taux d'attrition ?

Les résultats de cette étude permettront aux équipes marketing, commerciales et de la relation client de mettre en place des stratégies de fidélisation plus efficaces.

---

# Description du jeu de données

Le jeu de données regroupe les informations relatives aux clients de l'entreprise de télécommunications.

Il contient notamment des variables décrivant :

* les caractéristiques démographiques des clients ;
* leur ancienneté (Tenure) ;
* le type de contrat souscrit ;
* les services utilisés (Internet, support technique, protection des appareils, etc.) ;
* les montants facturés mensuellement et cumulés ;
* le statut d'attrition (Churn).

Afin d'enrichir l'analyse, 2 variables supplémentaires ont été développées à l'aide du langage DAX, notamment :

* La segmentation des clients par ancienneté(tenure bracket) ;
* la classification des clients les plus à risques(High risk) ;

Ces indicateurs offrent une vision plus précise du schéma d'attrition globale.

---

# Processus d'analyse des données

L'analyse a été réalisée selon les étapes suivantes :

### 1. Préparation des données

Les données ont été importées dans Power BI puis vérifiées afin de garantir leur cohérence. Les variables pertinentes ont été identifiées et plusieurs mesures DAX ont été créées afin de calculer automatiquement les principaux indicateurs de performance.

### 2. Création des indicateurs

Des mesures personnalisées ont permis de calculer :

* le taux d'attrition ;
* le nombre de clients ayant quitté l'entreprise ;
* la perte totale de revenus générée par ces départs ;
* les dépenses mensuelles médianes ;
* l'ancienneté médiane des clients.

### 3. Conception du tableau de bord

Le tableau de bord présente plusieurs visualisations interactives permettant d'explorer les causes du churn selon différents axes :

* ancienneté des clients ;
* type de contrat ;
* service Internet utilisé ;
* disponibilité du support technique ;
* protection des appareils.

Ces visualisations facilitent l'identification rapide des segments présentant les risques d'attrition les plus élevés.

---

# Principaux insights

L'analyse met en évidence plusieurs tendances importantes.

### 1. Les nouveaux clients présentent le risque de départ le plus élevé

La répartition des départs selon l'ancienneté montre que les clients ayant une faible durée d'abonnement résilient davantage leur contrat. En effet près de 50% des résiliations ont lieu avant les 10  premiers mois dont 20% les 2 premiers mois.
Cette observation suggère que les premiers mois de la relation client constituent une période critique.

<img width="617" height="277" alt="Screenshot 2026-07-02 180426" src="https://github.com/user-attachments/assets/f1361fa0-9d0b-41fe-9ed0-7b7f1158c313" />



### 2. Les contrats les plus courts génèrent davantage de pertes

L'analyse des pertes financières par type de contrat montre que les contrats de courte durée sont associés à une perte de revenus plus importante. Les contrats de longue durée semblent offrir une meilleure fidélisation.

<img width="437" height="273" alt="Screenshot 2026-07-02 181236" src="https://github.com/user-attachments/assets/f6c16b2e-dc99-4ad8-8d23-d46987b81861" />


### 3. Le support technique influence fortement la fidélité

Les visualisations indiquent que les clients ne bénéficiant pas d'un support technique quittent davantage l'entreprise. La qualité de l'accompagnement apparaît donc comme un facteur déterminant de satisfaction.

### 4. La protection des appareils constitue un facteur de fidélisation

Les clients disposant d'un service de protection des appareils semblent moins enclins à résilier leur abonnement. Les services complémentaires renforcent donc la valeur perçue de l'offre.

### 5. Les services Internet ne présentent pas tous le même niveau de risque

L'analyse par type de connexion Internet révèle que certains services sont davantage associés aux départs que d'autres. Cette différence peut être liée à la qualité du service, aux performances offertes ou au positionnement tarifaire.

<img width="439" height="281" alt="Screenshot 2026-07-02 181617" src="https://github.com/user-attachments/assets/88e82402-9242-42f6-bb24-5669a4290cd3" />


### 6. L'attrition entraîne une perte financière significative

Les mesures DAX montrent que chaque départ représente non seulement une perte d'abonnement futur mais également une perte importante de chiffre d'affaires cumulé. Le coût économique du churn est donc particulièrement élevé.



---

# Enseignements métier

Cette étude met en évidence plusieurs enseignements utiles pour les décideurs.

Premièrement, les premiers mois suivant l'acquisition d'un client représentent une période particulièrement sensible. Des actions de fidélisation précoces peuvent donc avoir un impact significatif.

Deuxièmement, les contrats de longue durée semblent constituer un levier efficace pour réduire l'attrition tout en stabilisant les revenus.

Troisièmement, les services à forte valeur ajoutée, comme le support technique ou la protection des appareils, contribuent à améliorer la satisfaction et la fidélité des clients.

Enfin, l'analyse démontre que le suivi d'indicateurs de churn dans Power BI permet d'identifier rapidement les segments à risque et d'orienter les campagnes marketing de manière plus ciblée.

---

# Recommandations

Au regard des résultats obtenus, plusieurs actions peuvent être envisagées.

* Mettre en place un programme d'accompagnement des nouveaux clients durant leurs premiers mois d'abonnement.
* Encourager la souscription à des contrats de plus longue durée grâce à des remises ou avantages exclusifs.
* Renforcer la qualité et la disponibilité du support technique afin d'améliorer l'expérience client.
* Promouvoir davantage les services complémentaires, notamment la protection des appareils.
* Développer un modèle prédictif permettant d'identifier automatiquement les clients présentant un fort risque de résiliation.
* Mettre en place des campagnes de fidélisation ciblées en utilisant les segments identifiés dans le tableau de bord Power BI.

---

# Conclusion

Cette analyse Power BI a permis d'identifier plusieurs facteurs influençant directement l'attrition des clients dans une entreprise de télécommunications. Les résultats montrent que l'ancienneté, le type de contrat ainsi que la souscription à certains services complémentaires jouent un rôle important dans la décision de résiliation.

Grâce aux indicateurs développés en DAX et aux visualisations interactives, il est désormais possible de suivre les principaux déterminants du churn, d'anticiper les départs futurs et de mettre en œuvre des actions ciblées pour améliorer la fidélisation des clients.

Cette démarche constitue une base solide pour l'évolution vers des modèles prédictifs intégrant des techniques de Machine Learning, permettant d'anticiper encore plus précisément le comportement futur des abonnés et d'optimiser les décisions stratégiques de l'entreprise.
