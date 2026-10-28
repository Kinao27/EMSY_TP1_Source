# TP1 - Installation Linux sur une VM - V0.4

## Groupe 

1. Yazan (YAD) 		- Noé (NAM) 
2. Siméon (SAR) 	- Gaëtan (GFR)
3. Tristan (TCK) 	- Nicolas (NTN)
4. Matéo (MCN) 		- Thomas (TBT)
5. Noah (NRN) 		- Guillaume (GFE)
6. Benjamin (BSC) 	- Valentin (VBC)
7. Gabriel (GOM) 	- Nikola (NDC)

## But 

Cette manipulation a pour but d'installer une distribution linux [Sparky Linux](https://sparkylinux.org/) dans une machine virtuelle VMware 
Workstation Player, à l’aide d’une image disque (ISO).

## Materiels à disposition 

- VMware Workstation Player - V17
- Image disque (ISO) : sparkylinux-6.4-x86_64-minimalcli.iso

## Création d’une machine virtuelle 

**A.** Lancez VMware Workstation Player (logiciel)  

**B.** Sélectionnez **Create a New Virtual Machine** 

**C-A.** Placez le fichier `.iso` dans une repertoire connu : 

`C:\SAR\VM\ISO`

**C-B.** Indiquez le chemin d’accès de l’image iso comme indiqué sous l’image ci-dessous :

![install image disk](/Images_1/Install_ISO.jpg) 

**D-A.** Choisissez un nom d'OS : `Linux - Debian 11.x` 

![OS name choice](Images/OS_Choice.jpg) 

**D-B.** Nommez la machine virtuelle : `SparkyLinux-SAR` 

**E.** Creez un disque virtuel -> capcité : **20GB** 

> Remarque 1 : Cocher **store virtual disk a single file**

![Virtual disk](/Images_1/VirtualDisk.jpg) 

> Remarque 2 : Ci-dessous, la configuration de la VM 

![Virtual disk](/Images_1/VM_Config.jpg) 

**F.** Lancez la machine virtuelle : **Play virtual machine** 

## Lancement de l'image ISO (Linux - Live CD) 

**G.** Lancement du live CD : 

<<<<<<< HEAD
<img width="639" height="533" alt="Lancement" src="https://github.com/user-attachments/assets/8ac52812-9387-434d-bfe2-95b2ece6f881" />

Shell Linux : 

<img width="798" height="653" alt="Shell" src="https://github.com/user-attachments/assets/0d541573-cc46-4704-9f9e-1646c0e59098" />
=======
![Launch](/Images/Lancement.jpg)

Shell Linux : 

![Shell_Linux](/Images/Shell.jpg)
>>>>>>> ff31364 (Ajout du rapport TP1 SAR-GFR)

> **ATTENTION** : par défaut, le clavier est configuré est **Clavier Americain**

Q1. disposition du clavier américain ?

<<<<<<< HEAD
<img width="720" height="279" alt="American" src="https://github.com/user-attachments/assets/a0cde3b2-bac6-4a64-8261-fdd2cd344b94" />

Q2. disposition du clavier suisse-romand ?

<img width="531" height="183" alt="Suisse" src="https://github.com/user-attachments/assets/98153eb1-74cb-4486-b776-172ab888c11a" />

Q3. disposition du le clavier français ? 

<img width="530" height="171" alt="Francais" src="https://github.com/user-attachments/assets/7f05a2bd-9fa9-49c3-8892-64c8d7825265" />

**H.** Déplacez-vous à la **racine du système** en utilisant la commande suivante : `cd` 

Q4. <img width="148" height="69" alt="Racine" src="https://github.com/user-attachments/assets/521a35c8-043f-4e04-9993-adc9d0736744" />

**I.** Affichez le contenu de la racine avec la commande : `ls –l`	

<img width="716" height="404" alt="ls-l" src="https://github.com/user-attachments/assets/b38123d1-c0d0-42a7-b1d0-dabf5f196a6e" />

Q5. Que signifie l'option `-l` avec la commande `ls` 

Le -l signifie « long listing format » (affichage détaillé).

Au lieu d'afficher uniquement les noms des fichiers, ls -l affiche plusieurs informations :

<img width="438" height="164" alt="Infos" src="https://github.com/user-attachments/assets/fa2d2365-27fc-4d8f-90a7-5c9a57272ef9" />

Q6. Décrypter la ligne où se trouve le répertoire **home**    

<img width="381" height="20" alt="Home" src="https://github.com/user-attachments/assets/df38e28b-179b-4dff-9248-c5efb83581db" />

·d → home est un répertoire (dossier).
·rwx → le propriétaire (root) a les droits :
	·r = lecture
	·w = écriture
	·x = accès au répertoire
·r-x → le groupe (root) peut lire et accéder au répertoire, mais pas écrire.
·r-x → les autres utilisateurs peuvent lire et accéder au répertoire, mais pas écrire.
·1 → nombre de liens.
·root → propriétaire du répertoire.
·root → groupe propriétaire.
·60 → taille indiquée pour le répertoire.
·Sep 17 14:02 → dernière modification.
·home → nom du répertoire.
=======
![QWERTY](/Images/American.jpg)

Q2. disposition du clavier suisse-romand ?

![QWERTZ](/Images/Suisse.jpg)

Q3. disposition du le clavier français ? 

![AZERTY](/Images/Francais.jpg)

**H.** Déplacez-vous à la **racine du système** en utilisant la commande suivante : `cd` 

Q4. ![Root](/Images/Racine.jpg)

**I.** Affichez le contenu de la racine avec la commande : `ls –l`	

![ls-l](/Images/ls-l.jpg)

Q5. Que signifie l'option `-l` avec la commande `ls` 

- Le -l signifie « long listing format » (affichage détaillé).

Au lieu d'afficher uniquement les noms des fichiers, ls -l affiche plusieurs informations :

![-l](/Images/Infos.jpg)

Q6. Décrypter la ligne où se trouve le répertoire **home**    

![Home](/Images/Home.jpg)

- d → home est un répertoire (dossier).
- rwx → le propriétaire (root) a les droits :
	- r = lecture
	- w = écriture
	- x = accès au répertoire
- r-x → le groupe (root) peut lire et accéder au répertoire, mais pas écrire.
- r-x → les autres utilisateurs peuvent lire et accéder au répertoire, mais pas écrire.
- 1 → nombre de liens.
- root → propriétaire du répertoire.
- root → groupe propriétaire.
- 60 → taille indiquée pour le répertoire.
- Sep 17 14:02 → dernière modification.
- home → nom du répertoire.
>>>>>>> ff31364 (Ajout du rapport TP1 SAR-GFR)

**J.** Créez un répertoire de travail nommé « EMSY_SAR-GFR» 

Q7. dans quel dossier racine allez-vous le placer (justifiez votre réponse) 

Le choix logique est /home. Justification :
- /home est le répertoire standard réservé aux données et fichiers personnels/utilisateurs dans l'arborescence Linux
- Ça évite de mélanger les fichiers de travail avec les fichiers du système.

Q8. Quelle commande allez-vous utiliser pour faire ceci ?  

- sudo mkdir /home/EMSY_SAR-GFR

**K.** Dans ce répertoire, créez un fichier texte que vous nommerez `TESTSLO_XXX_XXX` et éditez celui en écrivant un texte, exemple : "TP linux by XXX et XXX".
	   Utiliser la commande `vi`

- sudo vi TESTSLO_SAR-GFR

Q9. Pouvez-vous éditez un fichier uniquement avec la commande `vi` 

- vi fonctionne très bien pour ça, mais ce n'est pas l'unique méthode, nano est une autre possibilité.

Q10. Si vous éteignez la machine virtuelle et que vous la rallumez, est-ce que le répertoire créé ci-dessus existe toujours (justifiez votre réponse) ? 

- Non, je suis sur le Live CD (le système démarre depuis l'ISO,en RAM).
- Rien n'est encore installé sur le disque virtuel, donc toute les modifications sont temporaires (stockées en RAM)

**L.** Tapez la commande `ls -l /dev/sda` 

![ls-l/dev/sda](/Images/sda.jpg) 

Q11. Que signifie **sda** ? 

- s = SCSI (périphérique de stockage géré par le pilote générique sd du noyau Linux)
- d = disk
- a = c'est le premier disque détecté par le système

Q12. Quelle différence y a-t-il entre le répertoire de la question Q6 et celui du point L (justifiez votre réponse) ?

- /home est un vrai répertoire : il contient d'autres fichiers/dossiers, sert à organiser l'arborescence du système de fichiers.
- /dev/sda n'est pas un répertoire, c'est un fichier spécial de périphérique (device file).
- /dev/sda est une interface qui permet au système et aux programmes d'interagir directement
 avec le disque dur physique/virtuel au niveau bas

## Installation de SparkyLinux sur la VM

**M.** Installez SparkyLinux

![Installer](/Images/SparkyDL.jpg)


Q13. Quelle est la taille de disque minimum recommandée pour installer la distribution Sparky en mode cli 

- La taille de disque minimum est 10-12Go. Notre disque de 20Go est suffisant.

Q14. A quoi sert la partition swap ? Est-ce que ce principe existe-t-il sur les OS Microsoft Windows ? 

- le swap c'est l'extension de la RAM sur le disque, utilisé quand elle est pleine.

Q15. Quel format pourriez-vous utiliser pour la 3ème partition afin qu’elle soit également accessible depuis un OS Microsoft ? 

- FAT32 ou exFAT (compatibles Linux/Windows/Mac)

Q16. Durant l’installation, on vous demande deux noms d’utilisateur. A quoi correspondent-ils ? 

- Mot de passe root (admin) + nom d'utilisateur standard avec son mot de passe (droits limités).

**N.** Une fois l’installation de Linux terminée, prenez une capture d’écran du démarrage de votre système (GRUB)

![GRUB](/Images/GRUB.jpg)
 

**O.** Trouvez la ou les lignes de commande permettant de changer le clavier et procédez à la configuiration 

- sudo dpkg-reconfigure keyboard-configuration

![clavier](/Images/clavier.jpg)

**P.** Tapez la commande : `nano -version`

![nano](/Images/nano.jpg)

Q17. A quoi sert `nano` ? 

- nano est un éditeur de texte en ligne de commande, plus simple que vi (pas de modes séparés, on tape directement). Raccourcis affichés en bas de l'écran (Ctrl+O sauver, Ctrl+X quitter).

**Q.** Testez si l’application `git` est installée sur votre distribution, si ce n’est pas le cas installez un client git. 

Q18. Comment savoir si `git` est déjà installé ? 

- avec la commande git --version, si Git n'est pas installé, un message indiquant que la commande n'a pas été trouvée s'affichera.

dpkg -l git sudo

Q19. Si le client `git` n'est pas installé, quelle(s) commande(s) utilisez-vous pour l’installer ? 

- sudo apt update
- sudo apt install -y git

Q20. Que veut dire `apt` ? 

- Advanced Packaging Tool, c'est le logiciel de gestion de paquets central utilisé par les distributions linux.

Q21. Est-ce que cette commande (`apt`) peut être utilisée sur toutes les distributions Linux (justifiez votre réponse)? 

- non, elle est spécifique aux distributions basées sur Debian.

**R.** Créez un sous-répertoire « EMSY_TP1_XXX-YYY » dans le répertoire de votre utilisateur. 
       
**Attention** : Ici on veut que l’utilisateur (vous) ait les droits de lecture, d’écriture et d’exécution.

- mkdir -m 755 EMSY_TP1_SAR-GFR

Q22. Quel est le répertoire utilisateur ?  

- /home/sar

Q23. Quelles sont les commandes pour changer les droits d'utilisateurs (lecture - écriture - execution) ?  

- cd ~ (pour se positionner dans le répertoire utilisateur).
- mkdir -m 755 EMSY_TP1_SAR-GFR (pour créer le sous-répertoire de travail en lui attribuant explicitement les droits de lecture, d'écriture et d'exécution pour l'utilisateur, soit les permissions 755).

**S.** Dans ce répertoire, tapez la commande : `git clone https://github.com/votreDepot/EMSY_TP1_Source`

***Remarque*** : Il faut au préalable que vous ayez mis en place à cette adresse un fork du dépôt fourni lors de ce TP.

Q24. Qu’observez-vous dans ce répertoire ?

![REP](/Images/REP.jpg)

**T.** Editez le fichier source `.c` avec l’éditeur de texte « nano ». -> Réalisez un petit programme en C (par exemple de type « Hello world »).

![Hello](/Images/Hello.jpg)

**U.**	Vérifiez si le compilateur `gcc` est bien installé. Notez la version du logiciel

- Version de GCC : 10.2.1

![gcc](/Images/gcc.jpg)

**U-A.** Tapez les commandes suivantes :
```Shell 
gcc -Wall -o fichier.o -c fichier.c 
gcc -o fichier fichier.o 
```
Remarque : « fichier » est à remplacer par le nom de votre choix

![gcc](/Images/U-A.jpg)

Q25. Quels sont les fichiers qui ont été générés 

- EMSY_TP1.o : Le fichier objet (résultant de la compilation avec l'option -c).

- EMSY_TP1 : Le fichier exécutable (résultant de l'étape d'édition de liens).

![gcc](/Images/U-A_2.jpg)


**V.** Entrez la commande suivante : `./fichier`

![./EMSY_TP1](/Images/V.jpg)

Q26. Que se passe-t-il ?

- Le programme s'exécute et affiche le message Hello World! directement dans le terminal.

...A compléter...

## Tips 

> Tip 1 : sortir de la VM -> appuyer simultanément sur `Ctrl` et `Alt` 

> Tip 2 :  
> Pour arrêter un Linux proprement : 	`shutdown`  
> Pour forcer l’arrêt d’un système :	`halt` ou `poweroff`  
> Seul un administrateur peut exécuter ces commandes !

> Tip 3 : [commande vi avec ses options](https://www.linuxtricks.fr/wiki/guide-de-sur-vi-utilisation-de-vi)

> Tip 4 : [éditer un fichier type markdown (.md)](https://ashki23.github.io/markdown-latex.html)

