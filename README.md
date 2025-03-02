# VIRTUAL-LAB
# 🐧 Guide
# Télécharger et Installer VirtualBox sur Windows, macOS et Linux

Bienvenue dans ce guide détaillé sur la mise en place de ton premier laboratoire virtuel.

Je vais t'expliquer comment **télécharger** et **installer VirtualBox** un outil qui va te permetre de réaliser cette **première virtualisation** !

---

## 📚 Table des Matières

- [🔍 Prérequis Logiciels](#-prérequis-logiciels)
  - [🔧 Comment vérifier si wget ou curl est installé ?](#-comment-vérifier-si-wget-ou-curl-est-installé-)
  - [🚀 Installer wget ou curl sur votre Système](#-installer-wget-ou-curl-sur-votre-système)
    - [🪟 Pour Windows](#-pour-windows)
    - [🍏 Pour macOS](#-pour-macos)
    - [🐧 Pour Linux](#-pour-linux)
- [🌐 Télécharger VirtualBox depuis le Navigateur](#-télécharger-virtualbox-depuis-le-navigateur)
- [💻 Télécharger VirtualBox depuis le Terminal](#-télécharger-virtualbox-depuis-le-terminal)
  - [🪟 Pour Windows](#-pour-windows-terminal)
  - [🍏 Pour macOS](#-pour-macos-terminal)
  - [🐧 Pour Linux](#-pour-linux-terminal)
- [✅ Vérifier l'Installation](#-vérifier-linstallation)
- [📚 Ressources Utiles](#-ressources-utiles)
- [💻 Lancer ta première machine virtuelle (VM) sur VirtualBox](#-lancer-ta-première-machine-virtuelle-vm-sur-virtualbox)
    - [🪟 Pour Windows](#-pour-windows)
    - [🍏 Pour macOS](#-pour-macos)
    - [🐧 Pour Linux](#-pour-linux)
- [🆕 Créer une nouvelle VM](#-créer-une-nouvelle-vm)
  - [💿 Monter l'ISO depuis le sous-répertoire](#-monter-liso-depuis-le-sous-répertoire)
  - [🚀 Démarrer la VM](#-démarrer-la-vm)
- [📁 Référence aux sous-répertoires d'ISO](#-référence-aux-sous-répertoires-diso)

---


Linux est un noyau utilisé par de nombreuses distributions (distros), qui combinent le noyau avec des outils système, un gestionnaire de paquets et parfois une interface graphique (GUI). Chaque distribution a une philosophie, un public cible et une gestion des mises à jour spécifiques.

Si les mots noyau, gestionnaire de paquets ou encore GUI ne te parlent pas, je te conseille d'aller voir le dépôt GNU-LINUX qui t'expliquera ça en détail.

---

## 🔍 Prérequis Logiciels

Pour télécharger VirtualBox depuis le terminal, il vous faut :

- Soit `wget`, soit `curl`, deux outils permettant de récupérer des fichiers depuis le web.
- Un accès administrateur pour installer VirtualBox sur votre système.

### 🔧 Comment vérifier si `wget` ou `curl` est installé ?

Ouvrez un **terminal** (ou PowerShell sous Windows) et tapez :

`wget --version` ou `curl --version` 

Si l'une des commandes affiche une version, c'est tout bon ! Sinon, suivez les instructions ci-dessous pour installer ces outils.

### 🚀 Installer wget ou curl sur votre Système

### 🪟 Pour Windows

Vérifier si curl est installé (déjà présent sur Windows 10+ en PowerShell) :
`curl --version`
Installer wget (optionnel) :
Téléchargez l'exécutable depuis le site officiel :
👉 Télécharger wget pour Windows
Vérifier l'installation :
`wget --version`

### 🍏 Pour macOS

Installer 🍺 Homebrew (si non installé) :
🍺 Homebrew est un gestionnaire de paquets qui facilite l'installation de logiciels :
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
ou sinon directement depuis 🍺 [Site Officiel : Brew.sh](https://brew.sh)

Installer wget avec Homebrew :
```bash
brew install wget
```
Vérifier l'installation :
`wget --version`ou `curl --version`, curl est souvent déjà installé sur macOS

### 🐧 Pour Linux

Vérifier si wget ou curl est déjà présent :
`wget --version`ou `curl --version`

Installer wget ou curl selon votre distribution :
Pour Debian/Ubuntu :
```bash
sudo apt update
sudo apt install wget curl -y
```
Pour Fedora :
```bash
sudo dnf install wget curl -y
```
Pour Arch Linux :
```bash
sudo pacman -S wget curl
```
Vérifier l'installation :
`wget --version`ou `curl --version`

## 🌐 Télécharger VirtualBox depuis le Navigateur

Le moyen le plus simple pour télécharger VirtualBox est de visiter le site officiel :

🌍 [Page de téléchargement VirtualBox](https://www.virtualbox.org/wiki/Downloads)


Une fois téléchargé, lancez simplement le fichier pour démarrer l'installation.

## 💻 Télécharger VirtualBox depuis le Terminal

### 🪟 Pour Windows (Terminal)
Avec curl
```bash
curl.exe -o VirtualBox-7.0.8-Win.exe `
    https://download.virtualbox.org/virtualbox/7.0.8/VirtualBox-7.0.8-156879-Win.exe
```
Ou avec wget (si installé)
```bash
wget -O VirtualBox-7.0.8-Win.exe `
    https://download.virtualbox.org/virtualbox/7.0.8/VirtualBox-7.0.8-156879-Win.exe
```

Lancer l'installation
`.\VirtualBox-7.0.8-Win.exe`

### 🍏 Pour macOS (Terminal)
Télécharger l'image disque
```bash
curl -o VirtualBox-7.0.8-OSX.dmg \
    https://download.virtualbox.org/virtualbox/7.0.8/VirtualBox-7.0.8-156879-OSX.dmg
```

Ouvrir le fichier .dmg
`open VirtualBox-7.0.8-OSX.dmg`

### 🐧 Pour Linux (Terminal)
Pour Debian/Ubuntu
```bash
wget -O virtualbox-7.0.8.deb \
    https://download.virtualbox.org/virtualbox/7.0.8/virtualbox-7.0.8_ubuntu_jammy_amd64.deb
```
`sudo apt install ./virtualbox-7.0.8.deb`

Pour Fedora
```bash
wget -O virtualbox-7.0.8.rpm \
    https://download.virtualbox.org/virtualbox/7.0.8/VirtualBox-7.0-7.0.8_156879_fedora36-1.x86_64.rpm
```
`sudo dnf install ./virtualbox-7.0.8.rpm`

## ✅ Vérifier l'Installation


Windows : Recherchez Oracle VM VirtualBox dans le menu Démarrer 🔎.

macOS : Allez dans le dossier Applications 📁, lancez VirtualBox.

Linux : Exécutez la commande virtualbox dans un terminal 🖥️.



# 💻 Lancer ta première machine virtuelle (VM) sur VirtualBox

Une fois **VirtualBox** installé sur ton système d'exploitation (**Windows**, **macOS** ou **Linux**), suis ces étapes pour créer et lancer ta première **VM**. 

Les **images ISO** nécessaires pour tes systèmes d'exploitation préférés se trouvent dans les **sous-répertoires** de ce dépôt.

---

## 🪟 Pour Windows

1. **Ouvre VirtualBox** : 
   - Recherche "Oracle VM VirtualBox" dans le menu **Démarrer** et lance-le.

2. **Créer une nouvelle VM** : 
   - Clique sur **"New"**.

3. **Configurer la VM** :
   - **Nom** : Choisis un nom pour la VM (ex. : "Ubuntu VM").
   - **Type** : Sélectionne le type de système d'exploitation (ex. : Linux).
   - **Version** : Choisis la version exacte (ex. : Ubuntu 64-bit).

4. **Allouer la mémoire RAM** : 
   - Sélectionne la quantité de **RAM** (au moins **2 Go** pour un Linux léger).

5. **Créer un disque dur virtuel** :
   - Sélectionne **"Create a virtual hard disk now"**.
   - Choisis le type de disque **VDI (VirtualBox Disk Image)**.
   - Privilégie un disque **dynamique** (pour économiser de l'espace disque).
   - Défini la taille du disque (ex. : **20 Go**).

6. **Monter l'ISO** :
   - Dans les paramètres de la VM, va dans **"Storage"**.
   - Clique sur **"Empty"** sous **"Controller: IDE"**, puis sur l'icône du disque.
   - Sélectionne **"Choose a disk file"** et accède au fichier **ISO** situé dans le **sous-répertoire** correspondant de ce dépôt.

7. **Démarrer la VM** :
   - Clique sur **"Start"**.
   - Suis les instructions pour installer l'OS dans la VM.

---

## 🍏 Pour macOS

1. **Lance VirtualBox** :
   - Va dans le dossier **Applications** et ouvre **Oracle VM VirtualBox**.

2. **Créer une nouvelle VM** : 
   - Clique sur **"New"** et suis les mêmes étapes que sur Windows :
   - Donne un **nom** à ta VM.
   - Choisis le **type de système d'exploitation** (Linux, Windows, etc.).
   - Sélectionne la **version appropriée**.

3. **Configurer la RAM et le disque dur** :
   - Alloue la **RAM**.
   - Crée un disque dur virtuel (**VDI**, dynamique, **20 Go**).

4. **Monter l'image ISO** :
   - Ouvre les paramètres de la VM.
   - Va dans **"Storage"**.
   - Sélectionne **"Empty"** sous le **Controller IDE**.
   - Clique sur l'icône du disque et choisis **"Choose a disk file"** pour sélectionner l'ISO dans le **sous-répertoire** du dépôt.

5. **Démarrer la VM** :
   - Clique sur **"Start"**.
   - Installe l'OS à partir de l'image ISO montée.

---


### 🆕 **Créer une nouvelle VM**

1. **Clique sur "New"** pour démarrer la création d'une nouvelle VM.

2. **Configurer la VM** :

   - **Nom** : Donne un nom à ta VM (ex. : *"Ubuntu VM"*).
   - **Type de système** : Choisis le système d'exploitation (ex. : *Linux*).
   - **Version** : Sélectionne la version exacte (ex. : *Ubuntu 64-bit*).

3. **Allouer la mémoire RAM** :

   - Définis la quantité de **RAM** (au moins **2 Go** pour un Linux léger).

4. **Créer un disque dur virtuel** :

   - Sélectionne **"Create a virtual hard disk now"**.
   - Choisis le format **VDI (VirtualBox Disk Image)**.
   - Privilégie un **disque dynamique** pour économiser de l'espace.
   - Défini la **taille du disque** (ex. : **20 Go**).

### 💿 **Monter l'ISO depuis le sous-répertoire**

1. Va dans les paramètres de **"Storage"**.

2. Sélectionne **"Empty"** sous **"Controller: IDE"**.

3. Clique sur l'icône du disque, puis sur **"Choose a disk file"**.

4. Accède au fichier **ISO** dans le **sous-répertoire** du dépôt GitHub.


### 🚀 **Démarrer la VM**

1. Clique sur **"Start"** pour lancer la machine virtuelle.

2. Suis les étapes pour **installer le système d'exploitation** dans la VM.


### 📁 **Référence aux sous-répertoires d'ISO**

Pour téléchargé l'image **ISO** à monter dans **VirtualBox**, consulte les **sous-répertoires** dédiés de ce dépôt :

- `Kali-Linux`
- `Arch-Linux`
- `Debian`
- `Fedora`
- `Linux-Mint`
- `Manjaro`
- `OpenSUSE`
- `Ubuntu`

Chaque répertoire contient une **image ISO prête à l'emploi** pour ta **machine virtuelle** ! 🚀😊


## 📚 Ressources Utiles

🌍 [Site Officiel : VirtualBox.org](https://www.virtualbox.org/wiki/Downloads)

🍺 [Site Officiel : Brew.sh](https://brew.sh)


Bonne virtualisation ! 🥳
