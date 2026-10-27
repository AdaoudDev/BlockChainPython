# Projet BlockChain en python

Dans le cadre du projet de blockchain en python, je développe une blockchain python permettant à des machines de se connecter en tant que node/valideurs, des clients à créer des comptes, faire des transactions à l'aide d'un client front-end

## Utilisation IA
L'IA est utilisée pour rédiger du code, et faire le design du frontend, mais toute décision system design ou de technologies/concepts sont prises par moi après des recherches indépendantes.

### Concept
L'idée du projet est de faire une blockchain pour la vente d'objets informatiques de seconde main, basée sur les numéros de séries avec des valideurs centraux qui font rentrer les objets sur le marché

## Le concept utilisée : PoA
Le mécanisme choisi est le Proof of Authority, où des valideurs de confiance font rentrer les objets dans le réseau.

## Faiblesse du concept
La faiblesse de ce concept est le fait que l'infiltration/infection d'une des autorités fait que des objets non valides soient validés et infiltrent le réseau. 

## Solution apportée
Pour sécuriser ceci, on va faire qu'il faut 2-3 entités qui valident des transactions, et que si plusieurs transactions sont validés par une entité qui ne devaient pas être validés, on peut remettre en cause son accès et le suspendre temporairement.

## Valideurs
### Choix des valideurs
Le comité annuel choisi des valideurs toutes les nouvelles entités à ajouter. (Vu que c'est une démo, nous allons faire que c'est une variable d'envrionnement).

### L'incitation d'être valideur
Les valideurs sont rémunérés par des frais de transaction facturés envers les individus entrant sur le réseau, et par transaction passé (frais) pour la puisssance de compute qu'il provisionnent

### Détection de valideurs inauthentiques
Lorsqu'un valideur valide des objets qui se font rejetés par d'autres valideurs en boucle, un niveau de suspicion est ajouté à ce dernier, et la confiance est mise en pause et l'information propagée sur le réseau afin de mitiger les dégats