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
 
 Je suppose que cette infrastructure est utilisée 24/7 sur 30 jours soit 720 heures par jour, en précisant que je compare les options plus économiques et avec les ressources respectés pour chaque fournisseur sans compter d'OS. 
 Voici les estimations des couts mensuels pour quelques cloud providers mentionnés ci-dessus:
 
 - **AWS Cloud**
 Pour cette solutions je vais prendre l'exemple d'un EC2 t4g.xlarge qui a un cout par heure de $0.1344/h et comme stockage EBS gp3 qui coute 0.10/Go. La région étudiée est Europe (Paris) eu-west3.

						0.1344 × 720 = $96.77
						100 × 0.10 = $10.00
						
						Total de $106.77 /mois
						Soit $1241 /an

 - **Google Cloud**
 Pour cette solutions je vais prendre l'exemple d'un Compute Engine C4 c4a-standard-4 qui comporte exactement les ressources spécifiés a un cout par heure de $0.204736/h et le stockage qui coute $0.000187397/Go. La région étudiée est Europe (London) europe-west2.

						0.204736 × 720 = $147.41
						100 × 0.11 = $11.00
						
						Total de $158.41 /mois
						Soit $1900.92 /an

 - **Azure**
 Pour cette solutions je vais prendre l'exemple d'une Machine virtuelle qui comporte exactement les ressources spécifiés a un cout par mois de $81.76 et le stockage de 128 Go qui coute $10.56. La région étudiée est France Central.

						81.76 + 10.56 = $92.32
						
						Total de $92.32 /mois
						Soit $1107.84 /an


### Conclusion: Tableau récapitulatif des couts

| Service Cloud | Couts mensuels en $ |  
| ----------- | ----------- |  
| AWS | $106.77 |  
| GCP | $158.41|
| Azure| $92.32 |
  
  En comparant les prix d'hébérgement dans la zone européenne. Azure est l'option la moins chère, sachant en plus que pour respecter les contraintes j'ai augmenté le stockage de 28 Go et sans compter pas de licences, ni de plans d'économie. Ce qui pour une PME serait une option a considérer dans le cas de vouloir héberger une solution ou service avec une disponibilité à plein temps sans pas dépenser beaucoup d'argent. 
  
Suivi par AWS avec un cout un peu plus élevé et finalement Google, qui est la solution la plus cher des trois fournisseurs analysés. 

## Infrastructure n°2:
- **6 serveurs avec les ressources suivantes :**
  - **6 Go de RAM minimum**
  - **3 vCPU**
  - **20 Go de stockage disque par serveur**
- **Particularité : 3 serveurs sont éteints la nuit de 22h à 6h du matin**

Dans ce cas, cette infrastructure 3 serveurs sont utilisés 24h/7 et les autres sont utilisés 16h/7 jour, en précisant que je compare les options plus économiques et avec les ressources respectés pour chaque fournisseur sans compter d'OS. 
 Voici les estimations des couts mensuels pour quelques cloud providers mentionnés ci-dessus:

## Infrastructure n°3:
- **3 serveurs avec les ressources suivantes :**
  - **4 Go de RAM minimum**
  - **2 vCPU**
  - **50 Go de stockage disque par serveur**
- **1 load balancer qui répartit 5 Mb/s de données équitablement vers les 3 serveurs ci-dessus**
- **1 service de base de données managé**
  - **8 Go de RAM minimum**
  - **2 vCPU**
  - **10 Go de stockage disque**

## Références bibliographiques

- AWS ([EC2 On-Demand Instance Pricing](https://aws.amazon.com/ec2/pricing/on-demand/?refid=75a4f739-7816-4022-93a6-34a6f58d2910))

- GCP ([Pricing | Compute Engine: Virtual Machines (VMs) | Google Cloud | Google Cloud](https://cloud.google.com/compute/all-pricing))

- Azure ([Pricing - Container Instances | Microsoft Azure](https://azure.microsoft.com/en-us/pricing/details/container-instances/?msockid=354b77bbccc66ef91e5b613dcdf56f4e))

<!--stackedit_data:
eyJoaXN0b3J5IjpbNzM2Njc0NjU4LC02ODYwMzAxOTYsNzAwNz
I3NjIzLC03Nzg4NzU4NTgsLTUwNTEyMzUzOCwxMjUzNDQxNDA3
LC0xNDUwNjY3MTkxLC0yODIxNTE0NSwtMTExMTIyMTc0Niw2MD
cxMzExOCwtMTIxNDA2NDYwOCwxOTY0MTYwNjI1LC0zMDI1ODI0
NjUsMzk2MzYwMzY2LC0xNDcxMjcwNTYsLTExMDIxNjEwODYsLT
IxMjk5MTYwMTZdfQ==
-->