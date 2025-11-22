# Exercice: Calcul des coûts d’une Infrastructure as a Service en fonction de différents Cloud Provider
>Etudiant: 
**Luis Antonio GONZALEZ PATINO**
Lien GitHub: https://github.com/LuisGP-sudo/cloud-infra-exos

Pour chacune des infrastructures décrites ci-dessous calculer le coût sur 5 cloud providers (AWS, GCP, Azure, Scaleway et OVH). Faire apparaître le détail des calculs et comparer les résultats finaux.

Précisions:
- Les coûts sont à présenter en $USD, hors taxes par périodicité mensuelle
-  Aucune licence n’est utilisé
- Aucun plan d’économie / Saving plans / Spot instances / etc …
- Région à considérer : France (Paris) ou à défaut Europe

Avant de démarrer vous devez récupérer les informations concernant les coûts des différents services. Si des éléments ne sont pas donnés dans les énoncés vous choisissez systématiquement l’option la moins chère!

## Infrastructure n°1:
- **1 serveur avec les ressources suivantes :**
  - **16 Go de RAM minimum** 
   - **4 vCPU**
  - **100 Go de stockage disque**
 
 Je suppose que cette infrastructure est utilisée 24/7 sur 30 jours soit 720 heures par jour, en précisant que je compare les options plus économiques, avec les ressources respectés pour chaque fournisseur avec un OS Linux, les taxes et dans des Cloud publics. 
 Voici les estimations des couts mensuels pour quelques cloud providers mentionnés ci-dessus:
 
 - **AWS Cloud**
 Pour cette solutions je vais prendre l'exemple d'un EC2 t4g.xlarge qui a un cout par heure de $0.1344/h et comme stockage EBS gp3 qui coute 0.10/Go. La région étudiée est Europe (Paris) eu-west3.

						0.1344 × 720 = $96.77
						100 × 0.10 = $10.00
						
						Total de $106.77 /mois

 - **Google Cloud**
 Pour cette solutions je vais prendre l'exemple d'un Compute Engine C4 c4a-standard-4 qui comporte exactement les ressources spécifiés a un cout par heure de $0.204736/h et le stockage qui coute $0.000187397/Go. La région étudiée est Europe (London) europe-west2.

						0.204736 × 720 = $147.41
						100 × 0.11 = $11.00
						
						Total de $158.41 /mois

 - **Azure**
 Pour cette solutions je vais prendre l'exemple d'une Machine virtuelle qui comporte exactement les ressources spécifiés a un cout par mois de $81.76 et le stockage de 128 Go qui coute $10.56. La région étudiée est France Central.

						81.76 + 10.56 = $92.32
						
						Total de $92.32 /mois

 - **Scaleway**
 Pour cette solutions je vais prendre l'exemple de l'instance PRO2-XS qui comporte exactement les ressources spécifiés a un cout par mois de $80.30 et le stockage de 100 Go qui coute $8.6 par mois.

						80.30 + 8.60 = $88.90
						
						Total de $88.90 /mois

 - **OVH**
 Pour cette solutions je vais prendre l'exemple de l'instance b3-16 qui comporte exactement les ressources spécifiés le stockage de 100 Go (inclus dans le prix) a un cout par mois de $56.41.

						56.41 x 12 = $88.90
						
						Total de $56.41 /mois


### Conclusion: Tableau récapitulatif des couts

| Service Cloud | Couts mensuels en $ |  
| ----------- | ----------- |  
| AWS| $106.77 |  
| GCP| $158.41|
| Azure| $92.32 |
| Scaleway| $88.90|
| OVH | $56.41|
  
  En comparant les prix d'hébérgement dans la zone européenne. OVH est l'option la moins chère, sans compter pas de licences, ni de plans d'économie et taxes. Ce qui pour une PME serait une option a considérer dans le cas de vouloir héberger une solution ou service avec une disponibilité à plein temps sans pas dépenser beaucoup d'argent. 
  
Suivi par Scaleway avec un cout un peu plus élevé, suivi par Azure et AWS. Finalement Google, qui est la solution la plus cher des trois fournisseurs analysés. 

## Infrastructure n°2: 
- **6 serveurs avec les ressources suivantes :**
  - **6 Go de RAM minimum**
  - **3 vCPU**
  - **20 Go de stockage disque par serveur**
- **Particularité : 3 serveurs sont éteints la nuit de 22h à 6h du matin**

Dans ce cas, 3 serveurs sont utilisés 24h/7 et les autres sont utilisés 16h/7 jour, en précisant que je compare les options plus économiques, avec les ressources respectés pour chaque fournisseur avec un OS Linux et dans des clouds publics. 
 Voici les estimations des couts mensuels pour les deux cloud providers mentionnés ci-dessus:

 - **AWS Cloud**
 Pour cette solutions je vais prendre l'exemple d'un EC2 t4g.xl qui a un cout par heure de $0.1344/h et comme stockage EBS gp3 qui coute 0.10/Go. La région étudiée est Europe (Paris) eu-west3.

					(0.1344 × 720) + (20 × 0.10) = $98.77
					98.77 x 3 = $296.31 pour les 3 serveurs qui tournent 24h/7

					(0.1344 × 480) + (20 × 0.10) = $66.52
					66.52 x 3 = $199.53 pour les 3 serveurs qui tournent 16h/7

					296.31 + 199.53 = $165.39

					Total de $495.84 / mois	

 - **GCP**
 Pour cette solutions je vais prendre l'exemple d'un n2-standard-4 qui a un cout par heure de $0.2326/h et le stockage qui coute 0.1792/Go. La région étudiée est Europe (Paris) europe-west9.

					(0.2326 × 720) + (20 × 0.1792) = $171.056
					$171.056 x 3 = $513.168 pour les 3 serveurs qui tournent 24h/7

					(0.2326 × 480) + (20 × 0.1792) = $115.232
					66.52 x 3 = $199.53 pour les 3 serveurs qui tournent 16h/7

					513.168 + 115.232 = $628.40

					Total de $628.40/ mois	

### Conclusion: Tableau récapitulatif des couts

| Service Cloud | Couts mensuels en $ |  
| ----------- | ----------- |  
| AWS| $495.84 |  
| GCP| $628.40|

 En comparant les prix d'hébérgement dans la zone européenne. AWS Cloud est l'option la moins chère, sans compter pas de licences, ni de plans d'économie et taxes.

## Infrastructure n°3: a faire 
- **3 serveurs avec les ressources suivantes :**
  - **4 Go de RAM minimum**
  - **2 vCPU**
  - **50 Go de stockage disque par serveur**
- **1 load balancer qui répartit 5 Mb/s de données équitablement vers les 3 serveurs ci-dessus**
- **1 service de base de données managé**
  - **8 Go de RAM minimum**
  - **2 vCPU**
  - **10 Go de stockage disque**
  
 Dans ce cas, je suppose que les 3 serveurs sont utilisés 24h/7 avec un load balancer qui distribue 5 Mb/s de trafic entrant/sortant et 1 serveur de base de données managé, en précisant que je compare les options plus économiques, avec les ressources respectés pour chaque fournisseur avec un OS Linux et dans des clouds publics. 
 Voici les estimations des couts mensuels pour les deux cloud providers mentionnés ci-dessus:

 - **Scaleway**
  Pour cette solutions je vais prendre l'exemple de l'instance PLAY2-NANO qui comporte exactement les ressources spécifiés a un cout par heure de $0.000118 et le stockage de 50 Go et pour la base de donnée un POP2-2C-8G qui comporte exactement les ressources spécifiés avec un coût par heure $0.08085 .

## Références

- AWS ([EC2 On-Demand Instance Pricing](https://aws.amazon.com/ec2/pricing/on-demand/?refid=75a4f739-7816-4022-93a6-34a6f58d2910))

- GCP ([Pricing | Compute Engine: Virtual Machines (VMs) | Google Cloud](https://cloud.google.com/compute/all-pricing))

- Azure ([Pricing - Container Instances | Microsoft Azure](https://azure.microsoft.com/en-us/pricing/details/container-instances/?msockid=354b77bbccc66ef91e5b613dcdf56f4e))
- Scaleway ([Virtual Instances Pricing | Scaleway](https://www.scaleway.com/en/pricing/virtual-instances/?cpu=4|4&ram=1|16))
- OVH ([Price list: A comparison of our Public Cloud offers | OVHcloud Worldwide](https://www.ovhcloud.com/en/public-cloud/prices/))

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTM4NDc0ODAzNiw1NTc3MjYxMzMsLTE3ND
YyMDgxMzEsMTc2NDc4NDc4OCw4Njg1MTQ5NywtNjIyMTg4MDY1
LDIwMjE2NDk4NzUsMTMzNjY2NTU5OSwxNjI0NDgxOTUxLC0xMD
U2MTkwNDc1LDEwMzM1MDg3MzMsNjAyOTcxNDg1LDEzODQwNTI1
NTEsLTExOTQ2MjM4NjEsLTE0NTA3NTE0MzIsLTExNTgwMDcwNj
UsNjE2OTc1MDYxLC0xMTI1MjcwNzY5LDU4ODMzNDE5MiwtMTg1
NTY0NTEwOF19
-->