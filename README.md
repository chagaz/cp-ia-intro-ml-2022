# Certificat Chef de Projet IA / Fondamentaux du Machine Learning (2022)

Ce répertoire contient les notebooks qui accompagnent le module « Fondamentaux du Machine Learning » du [Certificat Chef de Projet IA|https://executive-education.dauphine.psl.eu/formations/certificat/chef-projet-ia-big-data] 2021-2022.

## Librairies
Ces notebooks ont été créés avec Python 3.9.7 et les librairies suivantes :
* matplotlib 3.5.0
* numpy 1.21.2
* pandas 1.3.4
* scikit-learn 1.0.1

Pour utiliser les même librairies, utilisez le fichier `package_list.yml` :
* Avec Anaconda, suivez la section "Importing an environment" [du tutoriel](https://docs.anaconda.com/anaconda/navigator/tutorials/manage-environments/). 
* En ligne de commande, utilisez
```bash
   conda env create -f package_list.yml -n introml
   conda activate introml
```

## Contenus
* Cours 1 (mercredi 12/01 matin) : prise en main de `scikit-learn`
* Cours 2 (mercredi 12/01 après-midi) : sélection de modèle, régularisation
* Cours 3 (jeudi 13/01 matin) : arbres et modèles ensemblistes
* Cours 4 (jeudi 13/01 après-midi) : méthodes à noyaux
* Cours 5 (vendredi 14/01 matin) : réduction de dimension
* Cours 6 (vendredi 14/01 après-midi) : clustering

### Utilisation avancée (git et nbstripout)
Pour faciliter le contrôle de version avec de notebooks jupyter, vous pouvez utiliser [`nbstripout`](https://pypi.org/project/nbstripout/), qui nettoie votre notebook (en particulier en enlevant les cellules de sortie) : installez-le avec
```bash
conda install -c conda-forge nbstripout
```
puis, avant de faire un commit,
```bash
nbstripout <nom_du_notebook>.ipynb
```
vous pouvez utiliser `git diff <nom_du_notebook>.ipynb` avant votre comit pour vérifier les modifications.
