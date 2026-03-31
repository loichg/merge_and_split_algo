# Merge and Split : Coopération Équitable dans les Réseaux Sans Fil

Ce projet implémente l'algorithme **Merge and Split** appliqué à la formation de coalitions d'émetteurs à antenne unique dans les réseaux sans fil. L'objectif est de permettre aux utilisateurs de s'auto-organiser pour maximiser leur utilité tout en minimisant les coûts liés à la coopération.

## Présentation du Projet
Dans un système de transmission **TDMA**, les émetteurs forment des coalitions disjointes pour optimiser la capacité totale du réseau. L'algorithme étudie l'équilibre entre :
* **L'Utilité :** La capacité de transmission atteinte par une coalition.
* **Le Coût :** L'énergie consommée pour l'échange d'informations entre membres d'une même coalition, qui augmente avec la distance et la taille du groupe.

## Fonctionnalités
* **Algorithme de Coalition :** Simulation des règles de fusion (*Merge*) et de division (*Split*) selon des critères de gain d'utilité.
* **Stabilité :** Recherche de structures de coalitions stables ($\mathbb{D}_{hp}$-stable ou $\mathbb{D}_{c}$-stable).
* **Analyse de l'Équité :** Intégration du **Jain Index** pour évaluer la répartition des ressources entre les utilisateurs.
* **Modélisation de la Mobilité :** Observation dynamique de l'évolution des coalitions lors du déplacement d'un utilisateur dans le réseau.

## Paramètres du Système
La simulation repose sur plusieurs paramètres configurables :
* **Mt / Mr** : Nombre de transmetteurs et de récepteurs.
* **$\alpha$** : Exposant d'affaiblissement de propagation (entre 2 et 6).
* **$\tilde{P}$** : Contrainte de puissance par slot de connexion.
* **Modèle de canal** : Prise en compte de la distance et de l'affaiblissement du signal.

## Installation et Utilisation
Le projet est développé en **Python** (Jupyter Notebook).

### Prérequis
* Python 3.x
* Bibliothèques : `numpy`, `matplotlib`, `scipy`

### Lancement
1. Clonez le dépôt :
   ```bash
   git clone [https://github.com/votre-utilisateur/votre-depot.git](https://github.com/votre-utilisateur/votre-depot.git)

2. Installez les dépendances :
   ```bash
   pip install numpy matplotlib scipy
3. Exécutez le notebook principal pour générer les simulations et les visualisations.

## Résultats

Le projet permet de générer :
- Une cartographie des coalitions (utilisateurs regroupés par couleurs).
- Des graphiques d'évolution de l'utilité individuelle.
- Une animation (mobilite.gif) montrant la reconfiguration en temps réel du réseau.

## Auteurs
Projet réalisé par Loïc Huang, Thomas Aubertier et Pascal Pham dans le cadre du cursus MAIN3 à Polytech Sorbonne.
