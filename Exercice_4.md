````
# Exercice 4

Cet exercice montre comment **créer un fichier caché**, **organiser des dossiers**, **renommer** et **déplacer** des fichiers dans le terminal.

## 1. Création d’un fichier caché et affichage des fichiers

**Description :**  
On crée un fichier caché nommé `.configuration` dans le répertoire personnel.  
Ensuite, on affiche tous les fichiers, y compris les fichiers cachés.

**Commandes exécutées :**
```bash
cd ~
touch .configuration
ls -a
````

## 2. Création d’une arborescence en une seule commande

**Description :**
On crée un dossier `creations` contenant un sous-dossier `crayons`.

**Commandes exécutées :**

```bash
mkdir -p creations/crayons
```

## 3. Création, renommage et déplacement de fichiers

**Description :**
Dans `crayons`, on crée un fichier `couleurs.txt` puis on le renomme en `colors.txt`.
Ensuite, on crée un fichier `gomme.txt` dans `creations` et on le déplace dans le dossier `crayons`.

**Commandes exécutées :**

```bash
cd creations/crayons
touch couleurs.txt
mv couleurs.txt colors.txt

cd ..
touch gomme.txt
mv gomme.txt crayons/
```

## 4. Retour au répertoire personnel

**Description :**
On revient dans le dossier personnel (home).

**Commandes exécutées :**

```bash
cd ~
```

> Cet exercice permet d’apprendre à **créer, renommer et déplacer des fichiers**, ainsi qu’à **gérer des fichiers cachés** dans le terminal.