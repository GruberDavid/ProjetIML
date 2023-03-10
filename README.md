# ProjetIML

Groupe : David GRUBER, Arthur MONTFORT et Daniel LEDOUSSAL

## Installation
Pour pouvoir utiliser le projet il faut :
* Installer Unity (2021.3 ou plus récent)
* Installer Python (3.8.13 ou plus récent)
* Installer le package Unity `com.unity.ml-agents`
* Installer le package Python `mlagents`
    * Pour se faire, suivre le guide d'installation ML-Agents [ici](https://github.com/Unity-Technologies/ml-agents/blob/develop/docs/Installation.md)


## Description de l'objectif
L'objectif est de permettre à un kart de rouler sur des circuits personnalisés de différentes difficultés.  
Le projet est réalisé en utilisant différents assets du template Kart Microgame d'Unity.  
Le Machine Learning est fait grâce aux packages Unity et Python ML-Agents.

## Description haut niveau
Notre objectif est d’implémenter et modifier le système de kart mis à disposition dans le template Kart Microgame d’Unity pour le faire fonctionner dans des circuits personnalisés de plus en plus complexes. Un de nos objectifs était de notamment le faire prendre des tremplins servant de raccourcis. 

Pour cela nous avons utilisé une IA qui se base sur un modèle d’apprentissage par renforcement (reinforcement learning), donc un agent dans un environnement qui reçoit des récompenses et est pénalisé en fonction de son comportement.

Dans notre cas, notre modèle reçoit une récompense quand : 
* Il passe les différents checkpoints qui sont dispersés sur tout le circuit.
* Il navigue correctement dans le circuit (pas de collision).
* Il passe par un tremplin.  

Il est pénalisé en cas de collision avec les murs du circuit.

## Défis
Nous avons donc rencontré les défis suivants : 
* Difficulté à modifier le modèle pour lui faire prendre les tremplins
* Difficulté à choisir les bon paramètre pour un fonctionnement optimisé de l’IA

Au final, le kart arrive globalement à finir chaque circuit créé mais ne prend jamais les tremplins.  
Résultat en vidéo pour chaque circuit : 
* [Result Track 1](https://youtu.be/Mw1KA922Lmk) 
* [Result Track 2 ](https://youtu.be/8WLiXgky46k) 
* [Result Track 3 ](https://youtu.be/D9Xis6VI0Z0) 

## Travail futur
On peut potentiellement imaginer utiliser cette IA sur des karts plus complexes, ou alors dans des circuits plus complexes. 

On peut aussi potentiellement essayer d’utiliser ce genre de modèle dans un environnement réel, afin de guider par IA un vrai Kart.

## Conclusion
Le projet nous a apporté les connaissances et capacités suivantes : 
* Perfectionnement de nos connaissances dans le machine learning, plus spécifiquement dans le domaine du renforcement learning (Analyse et Modification d’un modèle déjà existant).
* Prise en main des outils de machine learning dans l'environnement de développement Unity. 
* Développement des capacités à analyser et comprendre un système robotique dans un environnement virtuel. (Dans notre cas, le kart dans le moteur Unity).
* Amélioration de nos capacités à utiliser les outils collaboratifs (GIT et Github).
* Amélioration de nos capacités à travailler en équipe.


