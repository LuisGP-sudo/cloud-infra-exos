# Exercice: Quel type de cloud pour quels besoins ?

>Etudiant: 
**Luis Antonio GONZALEZ PATINO**

Pour chacun des cas ci-dessous dire quel type de cloud et de XaaS est le plus adapté et pourquoi. Expliquer avec un maximum de détails et des exemples comment répondre aux besoins dans chaque situation. 
Donner un ordre d’idée du coût de la solution préconisée.

En plus du cours et de vos connaissances de certains outils et logiciels, il est nécessaire de faire des recherches complémentaires sur internet pour apporter un maximum d’informations. Vous pouvez échanger et débattre entre vous des solutions mais chacun doit formuler ses propres réponses. 

Compétences : 
-  Concevoir des architectures évolutives et fiables 
- Surveiller et optimiser l'utilisation des ressources

## Cas n°1

**Eldo est une start-up qui développe un logiciel qui a pour objectif la mise en relation de professionnels du BTP avec des prospects qui souhaitent faire des travaux chez eux. En plus d’un module de mise en relation, Eldo développe un CRM pour les professionnels du BTP.**
**Nombre d’employés : 60** 

**Quelle solution est la plus adaptée pour héberger les logiciels Eldo?
Sachant que Eldo travail dans une startup, que le nombre d'employés**

---
Pour Eldo, qui est une startup de 60 employés en pleine croissance, la solution la plus adaptée est d’utiliser un cloud public en mode PaaS, par exemple AWS.

Permettant de déployer sa solution développé de façon rapide et efficace, leur permettant de ne pas s'occuper de la maintenance d'équippements physiques et attribuer de la flexibilité et scalabilité automatique dans le cas ou les clients augmentent au fur du temps.
Les services managés d’AWS qui peuvent utiliser sont: 
- Elastic Beanstalk pour l’application
- RDS pour la base de données
- S3 pour le stockage

En termes de coût, une architecture PaaS sur cloud public revient généralement à 300 à 800 € par mois pour démarrer backend, base de données managée, stockage, monitoring, sécurité), puis 1 000 à 2 500 € par mois lorsque la plateforme commence à avoir plus d’utilisateurs.

## Cas n°2

**MySecureProtect est une entreprise qui développe et exploite des objets connectés en lien avec la sécurité des habitations des particuliers. Plus d’un million d’objets connectés sont en liaison constante avec les serveurs de l’entreprise. Une application mobile permet de gérer son système de sécurité et de recevoir des notifications en cas d’anomalies. La spécificité de ce système est qu’il sollicite les serveurs dans 3 cas bien précis. Le matin lorsque les personnes quittent le domicile pour activer l’alarme, le soir pour désactiver l’alarme et enfin dans de rare cas lorsqu’une anomalie de sécurité est détectée.**

**Nombre d’employés : 150**

**Quelle solution pensez-vous la plus optimale et pourquoi ?**

---
Dans le cas de MySecureProtect étant une entreprise qui développe et exploite des objets connectés en lien avec la sécurité des habitations des particuliers. avec plus d'un million d'obejts connectés étant en liaison constante avec les serveurs de l'entreprise.
La solution plus adaptée a son besoin est d'utiiser un cloud privé en mode IaaS.

Ceci permettant de garder le contrôle sur la sécurité des données et sa performance, indispensable pour une entreprise qui gère des données sensibles et être affronté a des fortes activités des clients pendant le matin et le soir lorsque les alarmes sont activés.
Ce type de cloud permet d'adapter la puissance des serveurs, la puisance et le stockage selon le besoin et assurant une haute disponibilité du service.
Et disposant par exemple:
-   Des serveurs dédiés et virtualisés pour héberger l’application et traiter les communications avec les objets connectés,
-   Un stockage haute disponibilité pour les données sensibles,
-   Des firewalls et systèmes réseau pour sécuriser les échanges,
-   Des solutions de sauvegarde et de redondance qui granitiseront une continuité du service.

En termes de coût, un cloud privé étant plus cher qu’un cloud public, il faut compter une mise en place initiale entre 150 000 € et 300 000 € (infrastructure, licences, sécurité) et un coût mensuel d’environ 20 000 € à 60 000 € par mois (maintenance des serveurs, l’énergie).

## Cas n°3

**Paul est un particulier de 37 ans qui souhaite reprendre le contrôle de ses données. Il fait beaucoup de photos et apprécie pouvoir les stocker à un seul endroit mais y accéder depuis de nombreux appareils. Il dispose d’environ 800 Go de données et son besoin en stockage évolue relativement peu. Les compétences en informatique de Paul sont limitées.** 

**Nombre d’employé : N/A** 

**Que conseillez-vous à Paul ?**

---
Pour Paul qui lui est un particulier de 37 ans qui souhaite reprendre le contrôle de ses données et disposer d'un stockage accessible depuis plusieurs appareils, la solution étant la plus adapté pour lui est d'utiliser un cloud public en mode SaaS.
Lui permettant de stocker ses photos de façon sécurisée et de 


## Cas n°4
Une grande entreprise française de soutien aux armées du pays, accréditée par le ministère des armées et dont le nom est confidentiel, a besoin de moderniser ses infrastructures informatiques. Les besoins en termes de diversité de service, de quantité de serveurs, stockages et réseaux évoluent très rapidement.

 Nombre d’employés : 5000 

Quelle solution doit être mise en place pour moderniser l’infrastructure de cette entreprise ? 


---
Cloud Privé - NaaS , infra hybride 10M d'euros

## Cas n°5
TheFoodStore est une petite entreprise qui cherche à publier un site e-commerce rapidement afin de générer ses premières ventes en ligne. 

Nombre d’employés : 5 

Quelle solution sera la plus adaptée pour TheFoodStore ? 

---
SaaS - Cloud publique - UberEats, Shopify, etc... entre 10 et 100 euros

## Cas n°6 
DeliverEats est une plateforme permettant de commander et se faire livrer des repas. Elle dispose d’une application mobile et d’un site internet pour passer commande. Les livreurs de commandes disposent d’une application mobile qui les guide dans leurs livraisons, tandis que les restaurateurs reçoivent les commandes à préparer sur une application pour tablette. 

Nombre d’employés : inconnu 

Quels types d'architecture peuvent être envisagées dans ce cas ? Quels sont les avantages et inconvénients des différentes solutions ?

---
PaaS - Cloud Publique penser a la scalabilité, Kubernetes avec Jenkins 

## Cas n°7 
L’entreprise de télévendeurs Onenveutpa a besoin d’un nouveau système pour la gestion des informations de ses potentiels futurs clients. Les télévendeurs travaillent partout dans le monde. 

Nombre de télévendeurs : beaucoup trop 

Quelle solution proposez-vous ?

---
Cloud Privé IaaS. correction: SaaS fait l'affaire.



<!--stackedit_data:
eyJoaXN0b3J5IjpbLTcwNjY2NzYxNyw4MTUzNTIzNjksMTgzNT
c5ODQ0OSw5MDY0Njg4OTMsMTY2NTk0NjI5MywyMzg4NzEzNzQs
MTMwMTcyMjY2MywtMTM5Nzc2MjA2OSwtMTU0NTY3MDk5MSwxMT
E4MDcxODQ4LC0yNTQyNjU1NzUsMTUwMzk1NTA4OCwtODU3NTY5
MzA2LC0zNDcwODIzNTcsMjA4NDEwMDkwMywtMTg3MzU1NjEwNS
wxNzIyMDg4NjUyLC0xMTQ5NTE3MzY5LC0xNjA0MjU0MzQ2XX0=

-->