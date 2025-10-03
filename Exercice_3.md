
````
# Création d'une arborescence avec des sous-dossiers : Exercice 3

Cet exercice montre comment **créer une structure de dossiers complète en une seule commande**, puis comment ajouter des fichiers et du contenu à l’intérieur.

## 1. Création de l’arborescence principale

**Description :**  
On crée un dossier `actualites` avec un sous-dossier `politique` à l’intérieur.  
Grâce à l’option `-p`, tous les dossiers nécessaires sont créés en une seule commande.

**Commandes exécutées :**
```bash
mkdir -p actualites/politique
````

## 2. Création du dossier `elections` dans `politique`

**Description :**
On entre dans le dossier `politique`, puis on crée un sous-dossier appelé `elections`.

**Commandes exécutées :**

```bash
cd actualites/politique
mkdir elections
```

## 3. Création du fichier `candidats.txt` et ajout de contenu

**Description :**
On entre dans le dossier `elections` et on ajoute les noms des candidats dans le fichier `candidats.txt`.

**Commandes exécutées :**

```bash
cd elections
echo "Issoufou" > candidats.txt
echo "Hama" >> candidats.txt
echo "Seini" >> candidats.txt
```

## 4. Remonter de deux niveaux

**Description :**
On retourne au dossier principal `actualites`.

**Commandes exécutées :**

```bash
cd ../..
```

## 5. Création du dossier `buzz`

**Description :**
Dans le même niveau que `actualites`, on crée un nouveau dossier appelé `buzz`.

**Commandes exécutées :**

```bash
mkdir buzz
```

> L'exercice 3 nous apprend comment **créer rapidement une hiérarchie de dossiers**, **insérer des fichiers** et **naviguer dans les répertoires** du terminal.

```