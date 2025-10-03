````
# Gestion de dossiers et fichiers : Exercice 2

Cet exercice montre comment **créer des dossiers et des fichiers**, ajouter du contenu et vérifier les fichiers dans le terminal.

## 1. Création du dossier `conteneur` et sous-dossiers

** Description : **  
On commence par créer un dossier principal `conteneur` et trois sous-dossiers pour organiser différents types d'objets.

**Commandes exécutées :**
```bash
cd ~
mkdir conteneur
cd conteneur
mkdir voitures ustensiles electronique
````

## 2. Création d'un fichier dans `voitures` et ajout de contenu

**Description :**
On crée un fichier `mes_voitures.txt` et on y écrit le nom de plusieurs voitures.

**Commandes exécutées :**

```bash
cd voitures
echo "benz" > mes_voitures.txt
echo "toyota" >> mes_voitures.txt
echo "honda" >> mes_voitures.txt
```

## 3. Création d'un fichier dans `ustensiles` et ajout de contenu

**Description :**
On crée un fichier `cuisine.txt` et on y écrit différents ustensiles de cuisine.

**Commandes exécutées :**

```bash
cd ../ustensiles
echo "cuillere" > cuisine.txt
echo "marmite" >> cuisine.txt
echo "couteau" >> cuisine.txt
```
## 4. Vérification du contenu du fichier

**Description :**
On lit le fichier pour voir ce qu'il contient.

**Commandes exécutées :**

```bash
cat cuisine.txt
```

## 5. Vérification du contenu du dossier `conteneur`

**Description :**
On retourne dans le dossier `conteneur` et on liste tout le contenu.

**Commandes exécutées :**

```bash
cd ..
ls -l
```

> Cet exercice permet de comprendre comment **créer des fichiers, écrire dedans, et naviguer dans les dossiers** avec le terminal.

```
