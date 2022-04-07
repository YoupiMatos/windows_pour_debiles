# Installation de Windows pour débiles

Ceci est un petit guide pour installer Windows si vous n'avez aucune idée de ce que vous faites. Avec des images!

## Ce qu'il vous faut

- Une connexion internet
- L'accès à un ordinateur sous Windows 7 ou plus
- Une clef USB d'au moins 8 Go
- Une machine 64 bits capable de booter en UEFI (Machine sur laquelle vous voulez installer Windows)

## Ce que vous aurez à la fin

- Windows 10 Education
- Office 365 (facultatif)
- Des paramètres de vie privée raisonnables

___

## Télécharger windows

1. Ouvrez https://tb.rg-adguard.net/
2. Choisissez Windows (Final)
3. Choisissez la dernière version (build 19044.1288 au moment de l'écriture de ce guide)
4. Choissez "Windows 10" pour l'édition
5. Choisissez votre langue (Ça sera Français pour ce guide)
6. Choisissez le fichier ISO en x64.
7. Cliquez sur  "Download"
8. Le téléchargement devrait venir de `https://software-download.microsoft.com`
9. Sauvegardez le fichier

![image](https://i.imgur.com/IbxvAfv.png)

## Télécharger Rufus

1. Allez sur https://rufus.ie
2. Téléchargez la dernière version portable

![image](https://i.imgur.com/YL6Etlq.png)

## Graver l'ISO sur votre clef USB

1. Coonnectez votre clef USB
2. Lancez Rufus
3. Choisissez votre clef
4. Cliquez sur "SÉLECTION" et choisissez l'ISO que vous avez téléchargé
5. Cliquez sur "DÉMARRER"
6. Attendez que ça finisse

![image](https://i.imgur.com/xrgKsLR.png)

## Ajouter ei.cfg

1. Ouvrer le bloc-note
2. Collez ça dedans :
```
[Channel]
Retail
```
1. Sauvegardez le fichier sous `ei.cfg` dans lme dossier `Sources` (il devrait déjà exister) sur votre clef usb.
2. Éteignez l'ordinateur cible

## Précautions

Je vous recommande d'enlever tous les autres disques autre que celui sur lequel vous comptez installer Windows.

## Démarrer sur la clef USB

C'est là que je peux pas vraiment vous aider. Votre PC vous dis sûrement quelque chose comme `F10 Boot menu` sur l'écran de lancement. Essayez de matraquer cette touche et de choisir votre clef usb en tant que périphérique de démarrage. Vous aurez peut être besoin de désactiver l'option "Secure Boot" pour que ça marche. Pour de l'aide sur ces choses, consultez le manuel de votre carte mère ou internet.

## Installer Windows

1. Choisissez votre langue, le format horaire et de clavier, et cliquez sur `Suivant`.

![image](https://i.imgur.com/3XUpVg2.png)

2. Cliquez sur `Installer maintenant`
3. Si on vous demande une clef de produit, cliquez sur `Je n'ai pas de clef produit (Product Key)`
4. Choisissez `Windows 10 Education` pour l'installation, et cliquez sur `Suivant`

![image](https://i.imgur.com/8z9Wf0c.png)

5. Acceptez les termes du contrat de licence et cliquez sur `Suivant`
6. Choisissez `Personnalisé`

![image](https://i.imgur.com/G6Cz4i4.png)

1. Si vous ne comptez pas gardez vos donnez, supprimez toutes les partitions. Sinon supprimez seulement les partitions dont vous n'avez pas besoin (l'ancienne installation, etc...)
2. Choisissez `Espace non alloué` et cliquez sur suivant. Choisir un espace non alloué fera que l'installeur créera automatiquement les partitions dont il a besoin.

![image](https://i.imgur.com/Du3EGUS.png)

9. Attendez que ça finisse. L'ordinateur va redémarrer pendant l'installation, c'est normal.

![image](https://i.imgur.com/qdPAtyn.png)

## OOBE

1. Choisissez votre région & votre disposition de clavier
2. Quand vous aurez l'écran se connecter avec Microsoft, choisissez `Joindre le domaine à la place` pour ne pas avoir à vous connecter

![image](https://i.imgur.com/YcyVek5.png)

3. Choisissez votre. Si vous ne voulez pas configurer de questions en cas de perte de mot de passe, n'en mettez pas, vous pourrez en mettre un plus tard.
4. Choisissez non à toutes les options de vie privée et cliquez sur `Accepter`

![image](https://i.imgur.com/98ndB5m.png)

5. Dites non à Cortana quand on vous le demande
6. Vous arriverez bientôt sur votre bureau

![image](https://i.imgur.com/WacHVzW.png)

## Office (facultatif)

Cette étape est facultative. Vous pouvez l'ignorer si vous ne comptez pas utiliser Office.

1. Ouvrez https://tb.rg-adguard.net/
2. Choisissez `Microsoft Office` comme type
3. Choisissez `Microsoft Office 365` comme version
4. Choisissez `Office 365 Professional Plus` comme édition
5. Choisissez votre langue (Ça sera Français ici)
6. Choisissez le seul fichier disponible et cliquez sur `download`
7. Sauvegardez le fichier. Il devrait venir de `officecdn.microsoft.com.edgesuite.net` (Edge essaiera de vous empêcher de le télécharger. Vous pouvez cliquer sur conserver dans les trois petits points pour le télécharger quand même)

![image](https://i.imgur.com/g9Kyy3t.png)

1. Ouvrez le fichier téléchargé pour le monter
2. Lancez `Setup.exe`

![image](https://i.imgur.com/6GAKgoS.png)

10. Laissez le finir, et fermez la fenêtre

![image](https://i.imgur.com/j3MMqgo.png)

## Activation

1. Ouvrez le menu Sécurité Windows et sélectionnez Protection contre les virus et les menaces
2. Choisissez `Gérer les paramètres` dans Paramètres de protection contre les virus et les menaces
3. Désactivez Protection en temps réel, Protection dans le cloud et Envoi automatique d'un échantillon. C'est seulement temporaire.

![image](https://i.imgur.com/d2gjBG1.png)

4. Téléchargez [7-zip](https://www.7-zip.org) (J'imagine que vous pouvez le faire tout seul)
5. Ouvrez ça : [official KMS_VL_ALL paste](https://pastebin.com/cpdmr6HZ)
6. Téléchargez et décompressez la version AIO
7. Lancez le fichier CMD téléchargé en tant qu'administrateur

![image](https://i.imgur.com/fOyhMRO.png)

8. Appuyez sur `2` et attendez qu'il s'active

![image](https://i.imgur.com/O8UBgqv.png)

9. Appuyez sur `0` pour quitter
10. Vous pouvez maintenant supprimer tout ce que vous avez téléchargé, et réactiver les paramètres de sécurité

Votre Windows et Office devraient être activés maintenant:

![image](https://i.imgur.com/b5lPnb5.png)

## Vie privée

1. Téléchargez [Privatezilla](https://github.com/builtbybel/privatezilla#download)
2. Décompressez et lancez `Privatezilla.exe`
3. Je recommande d'utiliser les paramètres par défaut et de cocher la catégorie `Cortana` pour éviter de casser des choses
4. Cliquez sur `Apply selected` 

![image](https://i.imgur.com/fqR7kYr.png)

___

Vous devriez maintenant avoir une installation de Windows 10 basique, activée et raisonnablement respecteuse de vitre vie privée.

___

Ce guide à été traduit à partir de [Windows_For_Retards](https://rentry.co/windows_for_retards).