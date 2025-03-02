# 🐧 **VIRTUAL-LAB - Crée ton premier laboratoire virtuel !**  

## 🧭 **Découvre comment virtualiser facilement des distributions Linux**  

Bienvenue dans ce guide détaillé sur la création de ton **premier laboratoire virtuel** avec **VirtualBox** !  

Je vais t'expliquer pas à pas comment **télécharger**, **installer** et **utiliser VirtualBox** pour explorer en toute sécurité différentes **distributions Linux**. 

---

## 📚 **Table des Matières**

- [🧠 Qu'est-ce qu'un laboratoire virtuel ?](#-qu'est-ce-qu'un-laboratoire-virtuel-)
- [🔍 Prérequis Logiciels](#-prérequis-logiciels)
  - [🔧 Vérifier si wget ou curl est installé](#-vérifier-si-wget-ou-curl-est-installé)
  - [🚀 Installer wget ou curl sur ton système](#-installer-wget-ou-curl-sur-ton-système)
    - [🪟 Pour Windows](#-pour-windows)
    - [🍏 Pour macOS](#-pour-macos)
    - [🐧 Pour Linux](#-pour-linux)
- [🌐 Télécharger VirtualBox depuis le Navigateur](#-télécharger-virtualbox-depuis-le-navigateur)
- [💻 Télécharger VirtualBox depuis le Terminal](#-télécharger-virtualbox-depuis-le-terminal)
- [💡 Lancer ta première machine virtuelle (VM)](#-lancer-ta-première-machine-virtuelle-vm)
- [🧪 Expérimente avec ton labo virtuel](#-expérimente-avec-ton-labo-virtuel)
- [📚 Ressources Utiles](#-ressources-utiles)

---

## 🧠 **Qu'est-ce qu'un laboratoire virtuel ?**  

Un **laboratoire virtuel** est un environnement isolé sur ton ordinateur où tu peux :

- 🧪 **Tester des systèmes d'exploitation**, notamment des distributions Linux.  
- 🛠️ **Expérimenter en toute sécurité** sans risquer de casser ton système principal.  
- 🎓 **Apprendre et s'entraîner** avec des outils informatiques dans un cadre contrôlé.  

Pour créer ce labo virtuel, on utilise un logiciel de **virtualisation** tel que **VirtualBox**.  
Il te permet de faire tourner un **ordinateur virtuel (VM)** à l'intérieur de ton propre système d'exploitation.  

> 💡 Si des termes comme **noyau**, **distribution**, **interface graphique** ou **gestionnaire de paquets** te semblent flous, je te conseille d'aller faire un tour sur le dépôt [GNU-LINUX](https://github.com/ton-compte/GNU-LINUX) pour en apprendre plus ! 😉

---

## 🔍 **Prérequis Logiciels**

Avant de télécharger **VirtualBox**, assure-toi d'avoir :  

- Un **terminal** fonctionnel (ou **PowerShell** sous Windows).  
- Soit `wget`, soit `curl` pour télécharger des fichiers depuis le web.  
- Un **accès administrateur** pour installer les logiciels nécessaires.

---

### 🔧 **Vérifier si `wget` ou `curl` est installé**  

Ouvre un **terminal** et tape :  

```bash
wget --version
```
ou
```bash
curl --version
```
Curl est généralement déjà installé sur Windows et macOS. Pour Linux c'est wget qui domine.

Si une version s'affiche, c'est tout bon ! Si tu veux voir comment installer celui qui te manque, je te conseille d'aller voir mon autre dépôt WGET-CURL.



## 🌐 Télécharger VirtualBox depuis le Navigateur

Le moyen le plus simple pour télécharger VirtualBox est de visiter le site officiel :

🌍 Page de téléchargement VirtualBox

## 💻 Télécharger VirtualBox depuis le Terminal

### 🪟 Pour Windows
curl.exe -o VirtualBox-7.0.8-Win.exe `
https://download.virtualbox.org/virtualbox/7.0.8/VirtualBox-7.0.8-156879-Win.exe
### 🍏 Pour macOS
curl -o VirtualBox-7.0.8-OSX.dmg \
https://download.virtualbox.org/virtualbox/7.0.8/VirtualBox-7.0.8-156879-OSX.dmg
### 🐧 Pour Linux
```bash
wget -O virtualbox-7.0.8.deb \
https://download.virtualbox.org/virtualbox/7.0.8/virtualbox-7.0.8_ubuntu_jammy_amd64.deb

sudo apt install ./virtualbox-7.0.8.deb
```
## 💡 Lancer ta première machine virtuelle (VM)

Ouvre VirtualBox et clique sur "New".
Configure ta VM :
Nom : "Ubuntu VM"
Type : Linux
Version : Ubuntu 64-bit
Alloue la RAM : 2 Go minimum
Crée un disque dur virtuel (VDI, 20 Go, dynamique).
Monte l'image ISO depuis le dépôt GNU-LINUX.
Démarre la VM et suis les instructions pour installer l'OS.

## 🧪 Expérimente avec ton labo virtuel !

🎲 Maintenant que ta machine virtuelle est prête, il est temps de tester, expérimenter et apprendre !

👉 Si tu veux en savoir plus sur les différentes distributions Linux, consulte le dépôt GNU-LINUX.

# 📚 Ressources Utiles

- 🌍 [VirtualBox - Télécharger](https://www.virtualbox.org/wiki/Downloads)  
- 🍺 [Homebrew (macOS)](https://brew.sh)  
- 📁 [GNU-LINUX - Détails sur les distributions](https://github.com/ton-compte/GNU-LINUX)  

___
✨ Bonne virtualisation et bon apprentissage ! 🚀😊
