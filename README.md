# Travail-Pratique-Machine-Learning
## Optimisation d'hyperparamètre distribuée implémentation via Optuna/Ray tune

## 1. Description du projet

Ce projet consiste à expérimenter différentes méthodes d’optimisation d’hyperparamètres en Machine Learning sur le dataset MNIST. Il utilise Ray Tune et Optuna pour comparer les performances et les temps d’exécution de plusieurs approches.

## 2. Prérequis

- Python 3.10 ou une version compatible avec les dépendances.
- Jupyter Notebook.
- Les bibliothèques Ray Tune, Optuna, NumPy et Matplotlib.

## 3. Installation

Cloner le dépôt :

```bash
git clone https://github.com/belvaazidama-lgtm/Travail-Pratique-Machine-Learning.git
cd Travail-Pratique-Machine-Learning
```

Créer un environnement virtuel sous Windows :

```bash
python -m venv .venv
.venv\Scripts\activate
```

Installer les dépendances :

```bash
pip install jupyter "ray[tune]" optuna numpy matplotlib
```

## 4. Utilisation

Lancer Jupyter Notebook :

```bash
jupyter notebook
```

Ouvrir les notebooks du dossier `scripts/` :

- `Ray_Tune.ipynb` : expérimentations avec Ray Tune.
- `Ray_Tune_avec_OptunaSearch.ipynb` : intégration d’OptunaSearch dans Ray Tune.
- `optuna_mnist.ipynb` : optimisation avec Optuna.

Exécuter les cellules dans l’ordre.

## 5. Stack technique et architecture

**Technologies :** Python, Ray Tune, Optuna, Jupyter Notebook, NumPy et Matplotlib.

**Structure du projet :**

```text
Travail-Pratique-Machine-Learning/
├── README.md
└── scripts/
    ├── Ray_Tune.ipynb
    ├── Ray_Tune_avec_OptunaSearch.ipynb
    ├── optuna_mnist.ipynb
    └── placeholder
```

## 6. Résultats

Les expériences ont été réalisées avec 8 essais par méthode, 10 époques et 3 graines aléatoires.

- Meilleure accuracy moyenne : recherche aléatoire, avec **98,09 %**.
- Écart avec PBT : **0,09 point de pourcentage**.
- Méthode la plus rapide : **ASHA, avec 267 secondes**.
- Essais en erreur : **0**.

La différence de précision entre la recherche aléatoire et PBT reste faible par rapport à la variabilité observée entre les graines.

## 7. Contribution

Les contributions sont les bienvenues. Toute personne souhaitant améliorer le projet peut proposer des corrections, signaler un problème ou ajouter des expérimentations, en veillant à documenter les modifications.

## 8. FAQ et dépannage

**Problème : Optuna n’est pas installé.**

```bash
pip install optuna
```

**Problème : Jupyter Notebook n’est pas reconnu.**

```bash
pip install jupyter
```

**Problème : les dépendances ne s’installent pas.**

Vérifier la version de Python, l’activation de l’environnement virtuel et la connexion Internet.
