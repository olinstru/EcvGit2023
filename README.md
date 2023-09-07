Bonjour à tous,

Voici l'exercice à réaliser.
Pour la notation je regarderais l'arbre git et je vérifierais qu'il correspond bien à ce qui est demandé.
Normalement, vous avez un projet git qui a été créé en PUBLIC ! Attention, s'il n'est pas public, je ne pourrais pas vous noter !

Voici donc l'exercice :

# 1 - Mise en place (10 pts)
## Initialisation
- Effectuez un clone de ce projet (celui que vous êtes en train de lire) dans un dossier vide où vous avez accès sur votre machine : "git clone https://github.com/GuillaumeMuret/EcvGit2023.git"
- Renommez le remote actuel suite au clone : "git remote rename origin github-gmuret"
- Ajouter votre remote comme indiqué sur la page de votre nouveau projet GitHub "git remote add origin git@github.com:<VOTRE_NOM_UTILISATEUR_GITHUB>/EcvGit2023.git" (si vous vous êtes trompés sur l'url, il vous faudra supprimer origin "git remote rm origin" et refaire la commande d'ajout)
- Pousser la branche "master" sur le remote origin : "git push -u origin HEAD"
- (vous venez de réaliser ce qu'on appelle un fork)
- Créer une nouvelle branche "feature/test-toto"
- Créer un nouveau fichier nommé "toto.txt" avec le contenu "toto" sur la première ligne
- Ajouter le fichier "toto.txt" à l'index Git de la branche "feature/test-toto"
- Effectuer un commit avec le message "set toto"
- Pousser la branche "feature/test-toto"
- Revenez sur "master"
- Créer une nouvelle branche "feature/test-titi"
- Créer un nouveau fichier nommé "titi.txt" avec le contenu "titi" sur la première ligne
- Ajouter le fichier "titi.txt" à l'index Git de la branche "feature/test-titi"
- Effectuer un commit avec le message "set titi"
- Pousser la branche "feature/test-titi"
- Revenir sur "master"
- Créer une nouvelle branche "feature/test-tata"
- Créer un nouveau fichier nommé "toto.txt" (ATTENTION LE FICHIER S'APPELLE BIEN "toto.txt") avec le contenu "tata" sur la première ligne
- Ajouter le fichier "toto.txt" à la branche "feature/test-toto"
- Effectuer un commit avec le message "set tata"
- Pousser la branche "feature/test-tata"

# 2 - Actions sur les branches (10 pts)
- Placer vous sur la branche "feature/test-toto"
- Effectuer une fusion de "feature/test-titi" sur "feature/test-toto"
- Garder le message de commit par défaut de la fusion ("Merge branch ..."). RAPPEL : pour quitter l'éditeur de texte vi il vous suffit de taper "ESC", entrer ces trois caractères ":wq" puis appuyer sur "ENTRER". Pour quitter l'éditeur de texte nano il vous suffit de taper "CTRL + O" pour écrire (sauvegarder) et "CTRL + X" pour quitter.
- Pousser le résultat de cette fusion
- Effectuer une fusion de "feature/test-tata" sur "feature/test-toto"
- Le résultat à l'intérieur du fichier en conflit doit être "tonton"
- Une fois le conflit résolu, ajouter le fichier en conflit à l'index Git permettant de valider la fin de la fusion
- Effectuer un commit avec le message "merge with conflict feature/test-titi into feature/test-toto"
- Modifier le fichier "tata.txt" avec le contenu "Hakuna Matata" sur la première ligne
- Ajouter cette modification à l'index Git puis effectuer un commit avec le message "quelle phrase magnifique !"
- Pousser ce commit
- Supprimer le fichier "tata.txt"
- Ajouter cette suppression à l'index Git puis effectuer un commit avec le message "quel chant fantastique !"
- Effectuer un revert de l'action précédente ("git revert SHA1_DU_COMMIT_QUE_JE_VEUX_REVERT" pour trouver le "SHA1_DU_COMMIT_QUE_JE_VEUX_REVERT" il suffit de réaliser la commande "git log", les sha1 sont écrits juste après le mot commit)
