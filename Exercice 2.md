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
 
 Je suppose que cette infrastructure est utilisée 24/7 sur 30 jours soit 720 heures par jour, en précisant que je compare les options plus économiques et avec les ressources respectés pour chaque fournisseur. 
 Voici les estimations des couts mensuels pour les 5 cloud providers:
 
 - **AWS Cloud**
 Pour cette solutions je vais prendre l'exemple d'un EC2 t4g.xlarge qui a un cout par heure de $0.1344/h et comme stockage EBS gp3 qui coute 0.10/Go. La région étudiée est Europe (Paris) eu-west3.

						0.1344 × 720 h = $96.77
						100 × 0.10 = $10.00
						
						Total de $106.77 / mois
						Soit $1241 / an

 - **Google Cloud**
 Pour cette solutions je vais prendre l'exemple d'un Compute Engine C4 c4a-standard-4 qui comporte exactement les ressources spécifiés a un cout par heure de $0.204736/h et le stockage qui coute $0.000187397/Go. La région étudiée est Europe (London) europe-west2.

						0.204736 × 720 h = $147.41
						100 × 0.11 = $11.00
						
						Total de $158.41 / mois
						Soit $1900.92/ an

 - **Azure**
 Pour cette solutions je vais prendre l'exemple d'une Machine virtuelle Linux (Ubuntu Pro) qui comporte exactement les ressources spécifiés a un cout par heure de $0.204736/h et le stockage qui coute $0.000187397/Go. La région étudiée est France Central

						0.204736 × 720 h = $147.41
						100 × 0.11 = $11.00
						
						Total de $158.41 / mois
						Soit $1900.92/ an

  
## Infrastructure n°2:
- **6 serveurs avec les ressources suivantes :**
  - **6 Go de RAM minimum**
  - **3 vCPU**
  - **20 Go de stockage disque par serveur**
- **Particularité : 3 serveurs sont éteints la nuit de 22h à 6h du matin**

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

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTMyODkxODYwNiwxMjUzNDQxNDA3LC0xND
UwNjY3MTkxLC0yODIxNTE0NSwtMTExMTIyMTc0Niw2MDcxMzEx
OCwtMTIxNDA2NDYwOCwxOTY0MTYwNjI1LC0zMDI1ODI0NjUsMz
k2MzYwMzY2LC0xNDcxMjcwNTYsLTExMDIxNjEwODYsLTIxMjk5
MTYwMTZdfQ==
-->