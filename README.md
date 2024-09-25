Rapport de KAGONE Yasmine Oulia:


Ce laboratoire nous a permit d'apprendre à utiliser l'outil de travail GitHub. Cet outil permet la gestion
de projet et la collaboration en équipe. Il permet a plusieurs personnes d'une même équipe de travailler sur
le même projet. Lors d'un projet d'équipe, le travail peut être subdivisé en plusieurs parties attribuées
au différents membres de l'équipe. Chacun des membres peut travailler sur sa partie individuellement et la
partager à ses coéquipiers à travers GitHub, consulter la partie des autres et finaliser le projet en rassemblant 
les différentes parties. Cet outil permet de stocker toutes les parties d'un projet au même endroit et de 
mieux organiser celui-ci.

Dans la partie 1, nous avons créer un repository qui représente le lieu de gestion de notre projet. Dans ce
repository nous avons créer un nouveau dossier, dans lequel nous avons ajouter un  fichier texte. Nous avons 
ensuite fait un commit où nos changements ont été mentionné, puis nous avons synchronisé le repository distant
avec sa version locale. Nous avons créé une nouvelle branche afin que notre coéquipier puisse travailler sur 
celle-ci. Par la suite, nous avons cloner le repository de notre coéquipier , puis sur la branche qui a été 
créé pour nous, nous avons créé un nouveau dossier auquel on a aussi ajouté un texte. Nous avons ensuite
modifié le premier dossier en ajoutant un texte dans celui qui s'y trouvais déjà. Puis, nous avons fait un commit et 
synchronisé le repository distant avec sa version locale. Enfin, après vérification, nous avons fait un merge 
pour inclure les modifications de notre coéquipier dans la branche principale.

Dans la partie 2, nous avons créé localement un repository dans notre machine avec la même structure que celle de la
partie 1. Nous avons ensuite rendu le projet accessible à notre coéquipier sur GitHub. Par la suite, nous 
avons injecté une erreur dans le premier dossier, ajouté un deuxième texte au deuxième dossier, puis utiliser
les issues pour signaler cette erreur injectée. Parlant des issues, ceux ci doivent être clair et concis. La 
description des problèmes doit y être détaillée. Nous avons aussi appris comment rectifier les erreurs 
mentionnées dans les issues. Pour cela, nous sommes passé par deux méthodes, nous avons utilisé 
<<git revert 'numéro du commit problématique'>> qui permet de supprimer les actions du commit mentionné. Nous
avons aussi utiliser <<git reset --hard 'numéro du dernier commit correct'>> qui supprime toutes les actions 
des commits précédents le commit mentionné. Le problème avec la commande git reset est qu'elle est suivit de 
la commande <<git push --force origin Nom_de_la_branche>>, qui supprime l'historique des commits précédents, 
nous perdons alors le suivis de tout ce qui a été fait. Par ailleurs, le problème avec le git revert est que 
dans un cas plus général, si les actions du commit sélectionné sont supprimées, cela peut affecter le fonctionnement 
des actions des commits suivants si ils sont reliés.

En sommes, nous retenons que l'utilisation de GitHub doit être méthodiques. Nous devons nous assurer de pas avoir fait d'erreurs 
avant de déployer les changements sur le répertoire distant. Il est aussi important de toujours faire des commits à chaque changement
afin d'avoir une bonne gestion et un bon suivi de notre travail.

Listes des commandes utilisées:

    Git clone : permet de copier notre repository distant et le coller sur notre machine locale
    Cd : permet de naviguer dans un répertoire
    Mkdir : permet de créer un répertoire
    Cd.. : retour en arrière d’un répertoire
    echo 'text à écrire' >> Nom_du_text.txt : permet d'écrire une chaine de caractère dans un fichier texte
    Git add --a : pour utiliser tous les fichiers prêts à être envoyer sur le répertoire distant GitHub
    Git commit -m : permet de commenter la modification qu’on vient de faire à l’intérieur de l’environnement de travail
    Git push origin : déployer les changements sur le répertoire distant
    Git branch : pour voir les branches locales sur la machine locale
    Git branch -r : pour ajouter les branches distantes
    Git checkout – b nom_de_la_branche : permet de créer une nouvelle branche locale et de permuter sur celle-ci
    Git checkout nom_branche : pour changer de branche vers nom_branche
    Git pull origin nom_branche: permet de mettre les changements venant d’un répertoire distant sur un repository local
    Git merge : permet de fusionner des modifications d'une branche dans une autre
    Git log : permet d'afficher l’historique des commits
    Git reset -- hard : permet de réinitialiser l'état du repository à un commit spécifique
    Git revert : permet de supprimer les actions d'un repository spécifique
    Git init : initialisation d’un répertoire locale git
    Git push --force origin :utiliser après le git reset pour forcer l'envoi des modifications locales vers le repository distant

