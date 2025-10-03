````
# Gestion de fichiers personnels et dossiers : Exercice 6

Cet exercice montre comment **créer un dossier à votre nom**, **ajouter et déplacer des fichiers**, **renommer**, **afficher les fichiers cachés** et **supprimer un fichier**.

## 1. Création d’un dossier personnel

**Description :**  
On crée un dossier portant votre nom (à la place de "votrenom") et on entre dedans.

**Commandes exécutées :**
```bash
mkdir votrenom
cd votrenom
````

## 2. Création de fichiers

**Description :**
On crée trois fichiers :

* `banque.txt` pour les informations bancaires,
* `sante.txt` pour les informations médicales,
* `.mdp` pour un fichier caché.

**Commandes exécutées :**

```bash
touch banque.txt sante.txt .mdp
```

## 3. Ajout de contenu

**Description :**
On ajoute du texte à l’intérieur des fichiers `banque.txt` et `sante.txt`.

**Commandes exécutées :**

```bash
echo "Relevé bancaire janvier" > banque.txt
echo "Vaccination complète" > sante.txt
```

## 4. Vérification des fichiers cachés

**Description :**
On liste tous les fichiers, y compris les fichiers cachés, pour vérifier la présence de `.mdp`.

**Commandes exécutées :**

```bash
ls -a
```

## 5. Renommer un fichier

**Description :**
On renomme le fichier `sante.txt` en `medical.txt`.

**Commandes exécutées :**

```bash
mv sante.txt medical.txt
```

## 6. Organisation dans un sous-dossier

**Description :**
On crée un dossier `documents` et on y déplace les fichiers `banque.txt` et `medical.txt`.

**Commandes exécutées :**

```bash
mkdir documents
mv banque.txt medical.txt documents/
```

## 7. Suppression d’un fichier caché

**Description :**
On supprime le fichier caché `.mdp`.

**Commandes exécutées :**

```bash
rm .mdp
```

> Cet exercice permet de comprendre comment **créer, renommer, déplacer et supprimer des fichiers**, ainsi que **gérer les fichiers cachés** dans le terminal.