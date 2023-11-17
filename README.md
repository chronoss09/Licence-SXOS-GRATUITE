# LICENCE SXOS GRATUITE ![NS](https://img.shields.io/badge/-Nintendo%20Switch-e4000f?style=flat&logo=Nintendo%20Switch)

Avec les dernières avancés, il n'est plus nécessaire de faire un spoof de licence SXOS, il est maintenant possible de générer une licence valide depuis l'empreinte digital de votre propre console (__fingerprint__). Il suffit juste du boot.dat du SXOS ainsi que du request-licence.dat générée par votre console.

## Générer une licence valice depuis sa propre console :

  * Télécharger le dernier boot.dat en date [SXOS_beta_v3.1.0](https://www.mediafire.com/file/z8td5k923wsqs9w/SXOS_beta_v3.1.0.zip/file) (fw 11.0.1 max pour le moment)
  * __TX SX Licence Generator - by Reacher17__ téléchargeable à l'adresse suivante : [Licence Generator](https://www.mediafire.com/file/bmhexo5koxtqf9i/Generator_License_SX_License_Hack.rar/file)  
  * Extraire les 2 archives "_Licence Generator_ et le "_boot.dat_" quelque part sur votre PC
  * Mettre le fichier _boot.dat_ à la racine de la carte SD de votre console
  * Inséré votre carte SD à votre console puis injecter le fichier "_payload.bin_ contenu dans l'archive avec [TegraRcmGUI](https://github.com/eliboa/TegraRcmGUI/releases)
  * Sur le menu SX, appuyer sur "_Custom CFW_"
  * Un message vous dira que la _licence.dat_ est introubale et il va crée un fichier "__request-licence.dat__ 
  * Placer ce fichier dans le même dossier où se trouve le script sur mon votre PC 
  * Lancer le script et attendre quelque seconde
  * Un fichier __licence.dat__ est crée
  * Placer les 2 fichiers (__boot.dat__ & __licence.dat__) à la racince de votre carte SD
  * Démarrer votre console
  * Sur le menu SX, appuyer sur "_Boot custom FW_"
  * Bingo, vous voila sous SXOS
  * Enjoy !!!

N.B : Il faut avoir [Python 3](https://www.python.org/downloads/) installé sur votre PC pour exécuter le script.


## Custom Licence avec menu modifié :  
![capture](https://gbatemp.net/attachments/e0c-5inxeaabuyo-jpg.260555/)
Même principe que le script Licence Generator mais celui-ci te donne la possibilité de créer soit même un menu SX à ton goût.

  * Télécharger le script [SX License Hack](https://www.mediafire.com/file/5pl3kkgezvwb3tb/SX_License_Hack.rar/file)
  * Faite la procédure cité plus haut pour obtenir le fichier _request-licence.dat_
  * Télécharger un thème de votre choix via ce lien : [Custom Menu SXOS CFW v2](https://gbatemp.net/threads/custom-sxos-cfw.588020/#post-9463428)
  * Placer les fichiers du thème ainsi que le fichier _request-licence.dat_ dans le même dossier que le script puis exécuter le.
  * Placer les 2 fichiers (__boot.dat__ & __licence.dat__) à la racince de votre carte SD
  * Démarrer votre console
  * Vous voila avec un menu SX modifié à votre goût
      * Attention à la 4e icônes avant de customisé votre boot.dat, si vous n'en voulez pas, supprimer le fichier _holder.bmp_ contenu dans le dossier _theme_
  * Appuyer sur "_Boot custom FW_" pour lancé votre SXOS cfw
  * Bingo, vous voila sous le custom SXOS cfw
  * Enjoy !!!

  
## Homebrew SX qui fonctionne :  
  * _SX Dumper_
  * _SX Save Managers_
  * _SX Installer (Tinfoil)_

## Tuto Vidéo :
  * Tuto vidéo (en Français) par Deejay87: _[SXOS-FREE-LICENCE--SETUP--EMUNAND--CHOIDUJOURNX](https://odysee.com/@deejay87:4/SXOS-FREE-LICENCE--SETUP--EMUNAND--CHOIDUJOURNX:8)_
  * Lancé SXOS sous le firmware 11.0.1 (tuto en Anglais) par Sthetix : [HOW TO RUN THE SXOS ON FIRMWARE 11.0.1](https://www.sthetix.info/how-to-run-the-sxos-on-firmware-11-0-1/)
    
Plus d'infos : 
  * sur Discord : _[Modconsoles](https://discord.gg/yCrp3p5c)_
  * sur Gbatemps : _[Hack SXOS](https://gbatemp.net/threads/hack-sxos.582831/)_
  * Tuto vidéo par _[Deejay87](https://odysee.com/@deejay87:4/SXOS-FREE-LICENCE--SETUP--EMUNAND--CHOIDUJOURNX:8)_

## Tout d'abord, je remercie profondement Reacher17 qui n'a pas baissé les bras depuis qu'il avait commencé à travailler sur le reverse engineering du cfw SX. B&nder pour l'aide apporté au Script, moi même pour la licence fourni pour les testes, mrdude pour la mise à jour du script et le patch des homebrews SX ainsi que Zoria, Shadow, Darkstorm, Hexkyz, Red-J et MurasakiNX.


## English by Mrdude

Here's the guide with the graphics and new hacks, with this everything will work the same as on original sxos 3.10
======================================================================================

**SXOS currently only supports Switch firmware up to 11.0.0** - any newer firmware will fail, you can downgrade using AtmosphereNX and then create an emunand running 11.0.0 firmware for use with SXOS.

Download this file before you continue : [Hack Script and SXOS-GFX.zip](https://www.mediafire.com/file/95t3hu33ktx5aah/Hack_Script_and_SXOS-GFX.zip/file)

1: Copy an untouched clean [SXOS_beta_v3.1.0](https://www.mediafire.com/file/z8td5k923wsqs9w/SXOS_beta_v3.1.0.zip/file) boot.dat to your sd card root directory and Use SXOS payload to launch it.  
2: Launch SXOS - and if you don't have __license-request.dat__ - this will be created on the root of your micro sd card.  
3: Copy _license-request.dat_ from your switch to the extracted folder you download from this post.  
4: Copy a clean _SXOS 3.10 boot.dat_ to the folder and rename it to boot.dat.orig (this will keep it from being modified).  
5: Click __SXOS-GFX.exe__ - this will create a new folder called out that will contain some bin files which a created from the themes folder (you can remove this be clicking on SXOS-GFX.exe again)  
6: If you have python 3.9 installed - run __SX_License_Hack.py__ and boot.dat and _license.dat_ should be created.  
7: Copy the newly created boot.dat and license.dat to the root of your micro sd card.   
8: Use SXOS payload to launch. 

**note - SXOS extra hekate icon can be modded at line 310 (BL.write(b'argon/payloads/hekate.bin') to launch any payload you want, just change the path to the payload you with to launch, line 314 contains the name for that icon - once again change this to what you want.**

Also autoboot code was commented out - you can re-enable this again in the script if you want to show the SXOS options during boot - or just press the volume + button to bring up the options menu. 
