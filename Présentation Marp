---
marp: true
theme: gaia
markdown.marp.enableHtml: true
paginate: true
---
<!-- backgroundImage: "linear-gradient(to bottom, #ffb7c5, #DCD0FF)" -->

<!--
_color: black
-->

# Présentation Brief 4
#### Déploiement automatique du service applicatif Gitea avec Terraform
Groupe 4
*Baptiste, Dunvael, Luna, Noa*  

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![Gitea](https://user-images.githubusercontent.com/108001918/192715095-fc639c6f-5fa1-4c9d-bf82-a52c6de8d410.png)


<!-- paginate: false -->

---
# SOMMAIRE  
1 - Ressources utilisées
2 - Choix particuliers
3 - Nombre de scripts
4 - Plan projet prévu VS plan projet exécuté
5 - Compréhension des outils et des logiciels
6 - Difficultés rencontrées
7 - Solutions trouvées
8 - Bonus


<!-- paginate: true -->
<!--
_color: black
-->

---
## 1 - Ressources utilisées  
* Documentation Microsoft Azure
* Documentation Terraform
* Portail Azure pour l'interface graphique
* Cloudshell du portail Azure
* Moteur de recherche Google
* Visual Studio Code
* Github
* *(Alfred et Bryan encore et toujours :p)*

<!--
_color: black
-->

---

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![width:900px height:600px](https://user-images.githubusercontent.com/108001918/192770734-76a1ceac-ad0a-447d-9c47-e738956c09d6.png)

<!--
_color: black
-->

---
## 2 - Choix particuliers
* Script en langage Terraform adapté à Azure
* Installation de l'application Gitea
* Utilisation d'Ubuntu 20.3

<!--
_color: black
-->

---
## 3 - Nombre de scripts
Nous avons choisi de réaliser plusieurs scripts et un fichier contenant les clés SSH des administrateurs autorisés. Cela permet de  définir et d'enchaîner les étapes importantes du brief 4. Mais aussi de faciliter la lisibilité et la modification des scripts.
* 1er script : Script jusqu'à passation de projet
* 2ème script : Script Terraform d'Alfred avec scale set
* 3ème script : Script Ansible d'Alfred avec scale set

<!--
_backgroundColor: black
_color: black
-->

--- 
## 4 - Plan projet prévu VS plan projet exécuté 
|  | *Plan projet prévu* | *Plan projet exécuté* |
|-----------|:----------:|:------------:|
| GR|&#9745;|&#9745;|
| Bastion et clés SSH |&#9745;|&#9745;|
| VMs |&#9745; |&#9745;|
| Disque dur |&#9745;|&#9745;|
| Gitea |&#9745;|&#9745;|
| Backup  Vault |&#9745;|&#9745;|
| Load Balancer |&#9745;|&#9745;| 

<!--
_color: black
-->

--- 
|  | *Plan projet prévu* | *Plan projet exécuté* |
|-----------|:----------:|:------------:|
| MariaDB |&#9745;|&#9745;|
| Application Insight |&#9745;|&#9745;|
| Script de montée en charge |&#9745;|&#9745;|
| TLS |&#9745;|&#9744;|
| Documentation Terraform |&#9745;|&#9745;|
| Méthodologie Scrum |&#9745;|&#9745;|

<!--
_color: black
-->

---
## 5 - Compréhension des outils et des logiciels
***Terraform*** = 
* outil organisé qui convient pour déployer pas à pas une infrastructure et des applications.
* construction d'un plan prédéfini des étapes qui vont se réaliser en parallèle avec des messages d'erreur détaillés et précis.
* permet de configurer et paramétrer toutes les étapes d'une infrastructure.
* compatible avec d'autres logiciels et plateformes
* un interpréteur qui reçoit du code et le transforme en différentes commandes.

<!--
_color: black
-->

---

***Ansible*** = 
* fichier père qui va appeler plusieurs fichiers fils pour chaque fonction voulue. 
* Il faut un fichier différent pour chaque étape.
* un programme qui permet d'automatiser des tâches.
* prend en entrée une liste d'actions dans l'ordre au format YAML (pas un résultat fini comme terraform)
* il exécute du code python en sortie = des possibilités infinies car l'utilisateur peut installer des collections (pleins de fonctions qu'Ansible va pouvoir exécuter).

<!--
_color: black
-->

---
## 6 - Difficultés  rencontrées
Nous avons rencontré plusieurs difficultés : communes et individuelles.

* Prioriser les différentes étapes du script en fonction de leurs pré-requis
* Rechercher et analyser de la documentation (Ansible mal rédigée, Ansible et Azure presque incompatibles, mauvaise adaptabilité et flexibilité du logiciel d'ansible, documentations pas à jour)
* Trier les informations, les gérer et les assembler

<!--
_color: black
-->

---
## 7 - Solutions trouvées 
Afin de palier aux difficultés, nous avons cherché des solutions, nous sommes remis en question et avons adoptés différents comportements :

* scrums quotidiens
* écoute active 
* communication permanente 
* des temps/moments dédiés
=> ont permis d'apprendre à travailler ensemble de manière optimale et convenable pour tous les membres du groupe. 

<!--
_color: black
-->
---
## 8 - Bonus

Example de nos courbes graphiques en temps réel
&nbsp;&nbsp;&nbsp;&nbsp;![width:1100px height:500px](https://user-images.githubusercontent.com/108002178/192768326-e169f53b-b6e8-422c-983c-d68fafe29c15.jpg)

<!--
_color: black
-->

---

&nbsp;&nbsp;&nbsp;&nbsp;![width:1100px height:600px](https://user-images.githubusercontent.com/108002178/192768327-7a2c27bd-5b2f-48ac-9b6e-af83723e7f95.jpg)

<!--
_color: black
-->
