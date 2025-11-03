# Exercice: Calcul des coûts d’une Infrastructure as a Service en fonction de différents Cloud Provider
>Etudiant: 
**Luis Antonio GONZALEZ PATINO**

Pour chacune des infrastructures décrites ci-dessous calculer le coût sur 5 cloud providers (AWS, GCP, Azure, Scaleway et OVH). Faire apparaître le détail des calculs et comparer les résultats finaux.

Précisions:
- Les coûts sont à présenter en $USD, hors taxes par périodicité mensuelle
-  Aucune licence n’est utilisé
- Aucun plan d’économie / Saving plans / Spot instances / etc …
- Région à considérer : France(Paris) ou à défaut Europe

Avant de démarrer vous devez récupérer les informations concernant les coûts des différents services. Si des éléments ne sont pas donnés dans les énoncés vous choisissez systématiquement l’option la moins chère !

## Infrastructure n°1:
- **1 serveur avec les ressources suivantes :**
  - **16 Go de RAM minimum** 
   - **4 vCPU**
  - **100 Go de stockage disque**
 
 Je suppose que cette infrastructure est utilisée 24/7 sur 30 jours soit 720 heures par jour, voici les estimations des couts mensuels pour les 5 cloud providers:
 
  
## Infrastructure n°2:
- **6 serveurs avec les ressources suivantes :**
  - **6 Go de RAM minimum**
  - *3 vCPU
  - 20 Go de stockage disque par serveur
- Particularité : 3 serveurs sont éteints la nuit de 22h à 6h du matin

## Infrastructure n°3:
- 3 serveurs avec les ressources suivantes :
  - 4 Go de RAM minimum
  - 2 vCPU
  - 50 Go de stockage disque par serveur
- 1 load balancer qui répartit 5 Mb/s de données équitablement vers les 3 serveurs ci-dessus
- 1 service de base de données managé
  - 8 Go de RAM minimum
  - 2 vCPU
  - 10 Go de stockage disque

<!--stackedit_data:
eyJoaXN0b3J5IjpbODg4MDg0MjYsLTExMDIxNjEwODYsLTIxMj
k5MTYwMTZdfQ==
-->