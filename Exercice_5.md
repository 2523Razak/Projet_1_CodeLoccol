````
# Création et gestion de dossiers scolaires : Exercice 5

Cet exercice montre comment **créer une structure de dossiers**, **ajouter du contenu**, **renommer et déplacer des fichiers**, puis **supprimer un dossier vide** dans le terminal.


## 1. Création de l’arborescence principale

**Description :**  
On crée un dossier `projet_scolaire` avec deux sous-dossiers : `maths` et `sciences`.

**Commandes exécutées :**
```bash
mkdir -p projet_scolaire/maths projet_scolaire/sciences
````

## 2. Ajout de contenu dans `maths`

**Description :**
Dans le dossier `maths`, on crée un fichier `equations.txt` et on y écrit une équation mathématique.

**Commandes exécutées :**

```bash
cd projet_scolaire/maths
echo "x^2 + y^2 = z^2" > equations.txt
```

## 3. Ajout de contenu dans `sciences`

**Description :**
Dans le dossier `sciences`, on crée un fichier `experiences.txt` et on y écrit une expérience simple.

**Commandes exécutées :**

```bash
cd ../sciences
echo "eau + huile = séparation" > experiences.txt
```

## 4. Renommer un fichier

**Description :**
On retourne dans le dossier `maths` et on renomme le fichier `equations.txt` en `geometrie.txt`.

**Commandes exécutées :**

```bash
cd ../maths
mv equations.txt geometrie.txt
```

## 5. Déplacer un fichier

**Description :**
On déplace le fichier `experiences.txt` du dossier `sciences` vers le dossier `maths`.

**Commandes exécutées :**

```bash
cd ../sciences
mv experiences.txt ../maths/
```

## 6. Supprimer un dossier vide

**Description :**
Après avoir déplacé tous les fichiers, on supprime le dossier `sciences` devenu vide.

**Commandes exécutées :**

```bash
cd ..
rmdir sciences
```

> Cet exercice permet de **créer, renommer et déplacer des fichiers**, ainsi que **supprimer un dossier vide**.
> Il aide à mieux comprendre la **gestion des projets par dossiers** dans le terminal.