
# Installation des outils

* Installation de Vagrant : https://www.vagrantup.com/downloads.html
* Installation de VirtualBox : https://www.virtualbox.org/wiki/Downloads
* Un outil pour se connecter en SSH:
  * Putty : https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html
  * MobaXterm : https://mobaxterm.mobatek.net/download-home-edition.html

**Notes:**
> * Manipulation effectuée sous Windows.
> * Convient sur les PC portables Cap' (même avec "seulement" 8Go de RAM)
> * En cas de soucis de mot de passe administrateur sous Windows, lancer l'installation en effectuant un clic droit sur l'exécutable puis "Exécuter en tant qu'administrateur"


 1. Dans le menu Démarrer, cherchez "Windows PowerShell"

```bash
 mkdir vagrant_vms
 cd vagrant_vms
 vagrant init
```

 2. Modifier le fichier _Vagrantfile_ qui vient d'être créer.

***à compléter***


 3. Lancer la machine

```bash
 vagrant up         # l'enveloppe de la VM sera créée et démarrée sous VirtualBox
 vagrant ssh-config # garder le résultat
```
