# Présentation du `SSPCloud` et de `Git`

https://linogaliana.github.io/slides-gt-notebook/


## Objectif

- Découvrir `Git` à travers l'interface `RStudio`
- Découvrir l'interaction entre `Git`, `RStudio` et `Gitlab`
- Se familiariser avec quelques concepts de `Git`

## Méthode préconisée

On propose de travailler sur la même branche mais des fichiers
séparés. Cela constitue une initiation plus simple à `Git`
que l'utilisation de branches tout en évitant les conflits. 

## Fil conducteur

### Configuration

- Créer un compte Gitlab
- Se connecter au SSPCloud
- Créer un jeton à conserver quelque part (proposition: dans l'onglet `Mon Compte`)
- Chaque membre du groupe va sur la page d'accueil du projet
- Une des personnes doit forker le dépôt, les autres attendent
- La personne qui a fork ouvre les droits aux autres
- Retour sur la page d'accueil

### Récupération du dépôt

- Ouvrir un service RStudio sur SSPCloud
- Récupérer l'url pour être en mesure de cloner
- Cloner en utilisant le clique bouton de RStudio
- Découverte de l'onglet `Git`en haut à droite
- Passer en ligne de commande

```shell
git config --global credential.helper 'cache --timeout=200000'
```

### Premier commit

- Chacun crée un fichier `prenom-nom.md`
- Ecrire une phrase dedans
- Le fichier apparaît à droite avec statut `?`
- Cliquer sur la boite. Le statut doit changer pour devenir `A` --> `git add`
- Appuyer au dessus sur `commit`, une fenêtre s'ouvre (l'autoriser si le navigateur bloque).
Observer le changement
- Valider en mettant un message à droite et en cliquant sur `Commit` --> premier commit

### Interaction avec le dépot

- Appuyer sur la fleche verte (`push`)
- Il est nécessaire de s'authentifier une fois pour confirmer l'identité de notre
dépôt local


A ce stade:

- Personne la plus rapide: message qui indique un push réussi
- Autres: `push` refusé. C'est normal, il faut être à jour avec le dépôt pour
pouvoir pousser ses modifications. 

On va donc récupérer en local les dernières modifications

- Appuyer sur la fleche bleue (`pull`) pour récupérer les modifications
- Tenter à nouveau le `push` (flèche verte)
- Refaire ça si vous êtes plus de deux
