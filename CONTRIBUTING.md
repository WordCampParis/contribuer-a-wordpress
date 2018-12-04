# Comment contribuer ?

Merci d'envisager de contribuer à notre projet de documentation (en français) de la manière de contribuer à WordPress. Vous êtes tou·te·s les bienvenu·e·s pour nous aider dans la rédaction de cette documentation. Ce projet accompagne la [démarche participative](https://2019.paris.wordcamp.org/2018/11/06/premier-atelier-preparatoire-journee-contribution/) de préparation de la première **Journée de Contribution** du [WordCamp Paris](https://2019.paris.wordcamp.org) qui se déroulera le 24 avril 2019. Pour participer concrètement cette démarche, vous avez simplement besoin d'un compte sur GitHub.com et sur WordPress.org. Si toutefois vous ne disposez pas de l'un ou l'autre, voici les deux liens d'inscription sur ces deux sites :

- https://github.com/join
- https://login.wordpress.org/register?locale=fr_FR

## Principe

> La meilleure manière d'apprendre à contribuer, c'est de contribuer !

C'est le principe que nous avons retenu pour la rédaction de cette documentation et c'est une des raisons pour lesquelles nous avons choisi de l'écrire sur GitHub.com. En effet, la contribution au noyau de WordPress (ou à certains thèmes et extensions matures) repose sur :

- l'utilisation d'un [système de gestion du code source](https://fr.wikipedia.org/wiki/Gestion_de_versions) centralisé (ex: Subversion) ou décentralisé (ex: Git).
- un outil de rapport et de suivi d'anomalies (la plupart des projets open source de WordPress utilise le logiciel [Trac](https://trac.edgewall.org/))

En utilisant GitHub.com nous réunissons ces deux ingrédients en un seul et même "lieu" tout en profitant de la fonctionnalité de clonage de Git pour vous permettre de gagner en autonomie et en souplesse et nous faire gagner en efficacité quant à l'organisation de notre collaboration.

Par ailleurs, nous pensons que c'est également un bon moyen de se familiariser avec la gestion des [anomalies ou demandes d'évolutions](https://github.com/WordCampParis/contribuer-a-wordpress/issues) ("ticket" pour WordPress.org, "issue" pour GitHub.com) et leur organisation au sein de [jalons](https://github.com/WordCampParis/contribuer-a-wordpress/milestones) ("Milestones" pour les deux).

## Rédiger en ligne

Un autre avantage de l'utilisation de GitHub.com, c'est que vous pouvez commencer à contribuer en ligne sans équipement logiciel particulier. Pour vous le démontrer, nous vous proposons de faire votre première contribution en utilisant les différentes interfaces de GitHub.com.

### La tâche à réaliser

![Issue](https://dl.dropboxusercontent.com/s/fyq9i01xg6k1nps/00-issue.png)

Si vous affichez la [liste des "issues"](https://github.com/WordCampParis/contribuer-a-wordpress/issues) de notre dépôt GitHub, vous en trouverez une qui est étiquetée *bonne première anomalie* et qui s'intitule "S'ajouter en tant que contributeur au projet". En cliquant sur son lien vous afficherez la page capturée ci-dessus. Notez dés à présent que la référence de cette tâche est `#4`.

L'objectif de cette tâche est simple : il s'agit de modifier le fichier [CONTRIBUTORS.md](./CONTRIBUTORS.md) afin qu'il intègre vos noms d'utilisateur·rice sur GitHub.com et WordPress.org.

### Cloner le dépôt dans vos dépôts GitHub.

![Fork](https://dl.dropboxusercontent.com/s/e0rrc54lydqdesd/01-fork.png)

En haut à droite comme le montre la flèche bleue, vous trouverez le bouton "Fork". Cliquez dessus et attendez quelques instants, le temps que GitHub se charge de cloner ce dépôt dans vos dépôts.

![Forking...](https://dl.dropboxusercontent.com/s/udemwf6ylr25shc/02-my-fork.png)

L'écran ci-dessus apparaîtra pendant le processus de clonage et vous pouvez d'ores et déjà constater à l'aide de la flèche bleue que vous êtes désormais dans votre zone personnelle sur GitHub (mon nom d'utilisateur est `imath`).

![Forked](https://dl.dropboxusercontent.com/s/nr9aw7lnrbgwa2o/03-open-contributors.png)

Dés que vous verrez apparaître l'écran ci-dessus, cliquez sur le fichier `CONTRIBUTORS.md` de la liste pour l'afficher.

###Modifier le fichier listant les contributeur·rice·s

![Open file](https://dl.dropboxusercontent.com/s/6ojug7wlpw86xno/04-edit-contributors.png)

Ce fichier contient notamment un tableau qui informe sur les noms d'utilisateur·rice des contributeurs de notre projet. Comme le montre la flèche bleue, cliquez alors sur l'icône en forme de crayon pour basculer dans le mode de modification de ce fichier.

![Copy row](https://dl.dropboxusercontent.com/s/lj8o4l548rpem9o/05-copy-contributor.png)

Pour mettre en forme les fichiers, GitHub utilise la syntaxe [MarkDown](https://guides.github.com/features/mastering-markdown/). Pas d'inquiétude concernant cette syntaxe à ce moment de la partie, une bonne manière de progressivement maîtriser un nouveau language est d'utiliser le bon vieux copier/coller ! Sélectionnez donc une des lignes du tableau, dans notre exemple celle de @audrasjb, et copiez là avant d'insérer une nouvelle ligne (retour chariot).

![Paste contributor](https://dl.dropboxusercontent.com/s/k86wtotoco64vxd/06-paste-contributor.png)

Collez alors le contenu de votre presse-papier avant de remplacer les éléments insérés par vos données personnelles. Il s'agit de remplacer ce qui est entre crochets par vos noms d'utilisateur·rice et ce qui est entre parenthèses par les URL de vos profils d'utilisateur·rice, et ce sur chacun des sites : d'abord GitHub.com, puis WordPress.org. Une fois que c'est fait, vous pouvez vérifier le résultat en cliquant sur l'onglet "Preview changes" de l'interface.

###Valider les modifications (commit)

![Prepare commit](https://dl.dropboxusercontent.com/s/4sy31yyp105jcsw/07-commit-contributors.png)

Sous la fenêtre de prévisualisation, vous trouverez le formulaire de validation de votre modification ou de "[commit](https://fr.wikipedia.org/wiki/Commit)". Dans le premier champ : indiquez succintement en quoi consiste votre modification, par exemple "Ajout de mes noms d'utilisateur" et **veillez à activer le bouton radio de création d'une nouvelle branche** en spécifiant le nom de cette branche pour l'identifier plus facilement par la suite (ex: "ajout/profil-nomutilisateur").

> PS : la branche "master" est la version par défaut du contenu de votre dépôt, elle doit être considérée comme la version la plus aboutie de vos travaux de rédaction. En utilisant une nouvelle branche pour "tester" une modification : cela vous permet de ne pas altérer votre version la plus aboutie jusqu'à ce que vous soyez certain que vos modifications puissent sereinement être fusionnées dans la branche "master" (NB: vous pouvez aussi décider de les abandonner en supprimant la nouvelle branche).

Une fois, que votre "commit" est prêt, cliquez sur le bouton vert s'intitulant "Propose file change".

![No self PR](https://dl.dropboxusercontent.com/s/hzokpeupl8w5asb/08-noselfpr-contributors.png)

Vous atteignez alors un écran qui vous propose de faire une "Pull Request" (qu'on pourrait traduire par une demande de modification) sur la version "master" de votre dépôt. Or, vous souhaitez faire cette demande sur le dépôt que vous avez cloné (ou "forké"), c'est à dire celui de [WordCampParis](https://github.com/WordCampParis/contribuer-a-wordpress). Pour ce faire, il suffit d'interrompre le processus en revenant sur la page d'accueil de votre dépôt en cliquant sur l'onglet `Code` comme le montre la flèche bleue.

### Faire une "Pull Request" (demande de changement) sur le dépôt forké

![Compare](https://dl.dropboxusercontent.com/s/1tsrb3mhlhof7yd/09-compare-upstream-contributors.png)

Une fois revenu·e sur la page de votre "fork", vous remarquerez la présence d'une zone à fond jaune dans laquelle un bouton vert intitulé "Compare & pull request" vous invite à comparer et faire une demande de changement. Cliquez dessus.

![Pull Request](https://dl.dropboxusercontent.com/s/x5rn278c5i35060/10-pr-upstream-contributors.png)

Cette fois-ci, la demande de modification concerne bien le dépôt forké depuis WordCampParis. Pour référencer ce changement dans la tâche décrite plus tôt, il s'agit de saisir le caractère `#` suivi du numéro de la tâche (ou anomalie). GitHub nous assiste en nous proposant une liste déroulante pour la retrouver plus facilement : activez la numéro 4, comme le montre la capture ci-dessus. Une fois que vous êtes satisfait·e de votre "Pull Request", cliquez sur le bouton vert s'intitulant "Create pull request". Vous n'avez plus qu'à patienter jusqu'à ce qu'un validateur ou "committer" du dépôt de WordCampParis réagisse à votre demande.

### Suivre l'avancée de ses "Pull Requests"

![Follow PRs](https://dl.dropboxusercontent.com/s/vl2lt0p4lttsmx6/11-follow-pr-contributors.png)

Comme le montre la flèche bleue, vous pouvez à tout moment consulter les demandes de modification sur les différents dépôts auquels vous avez contribués depuis le menu "Pull requests" de la barre de navigation supérieure de GitHub.com.

### Résoudre des conflits

Lorsqu'on travaille à plusieurs sur un même document, il est fréquent que nos demandes de modification génèrent des conflits car la version du contenu auquel elle se rapportait peut avoir évoluer avec le temps.

![Merge Conflicts](https://dl.dropboxusercontent.com/s/ocv4dwoykwqyshu/12-merge-conflicts.png)

Lorsque c'est le cas, vous remarquerez que votre "Pull Request" affiche un cadre vous informant qu'il existe des conflits à résoudre, comme illustré dans la capture d'écran ci-dessus. Cliquez alors sur le bouton sur la droite de ce cadre et qui s'intitule "Resolve conflicts".

![View conflicts](https://dl.dropboxusercontent.com/s/8vlahrvlfl14cug/13-view-merge-conflicts.png)

Vous pourrez alors mettre à jour le (ou les) fichier(s) concerné(s) votre "Pull Request" grâce à l'interface qui s'affiche. Comme montré ci-dessus, l'ajout de vos noms d'utilisateur sous la mention `<<<<<<< ajout/profils-imath` (c'est à dire le nom de votre branche) n'est pas intervenu alors que la version la plus aboutie de la documentation a intégré un autre utilisateur comme le montre ce qui est affiché au dessus de la mention `<<<<<<< master`.

![Resolve merge conflicts](https://dl.dropboxusercontent.com/s/si8d77gx82cfca4/14-resolve-merge-conflicts.png)

Il s'agit donc de déplacer votre rangée de tableau sous celle de @anybodesign et de supprimer les marqueurs de branches conflictuelles qui vous permettaient de comprendre la difficulté. Une fois que c'est fait, cliquez sur le bouton "Mark as resolved" pointé par la flèche bleue.

![Merge](https://dl.dropboxusercontent.com/s/9jcrht3u3s6hqtx/15-merge.png)

Lorsque tous les conflits sont résolus, vous verrez apparaître le bouton vert "Commit merge" pour vous permettre de valider cette fusion. Cliquez dessus et patienter quelques instants.

![Conflics solved](https://dl.dropboxusercontent.com/s/djum1nxqwnsl7jc/16-merge-pr-upstream.png)

Un bandeau sur fond bleu vous confirmera que les conflits ont été résolus et votre demande de modification sera à jour par rapport à la branche "master" du dépôt de WordCampParis. Un de ses committers pourra donc poursuivre son étude de votre demande de modification et pourquoi pas la valider !

![Tada](https://dl.dropboxusercontent.com/s/hwcw94054119zk5/17-merged.png)

Bravo ! Votre demande de modification a été fusionnée dans la branche "master" du dépôt de WordCampParis, ou autrement dit : votre "PR" a été "mergée" ! Vous pouvez tranquillement supprimer la branche qui a servit à votre demande de modification en cliquant sur le bouton "Delete branch".

![Issue updated](https://dl.dropboxusercontent.com/s/fs2ay0xhho0fypx/18-issue-updated.png)

Comme vous aviez référencé la tâche numéro 4 dans votre demande de modification, vous pourrez constater que le descriptif de cette tâche s'est enrichit d'une information concernant cette fusion.

###Maintenir son "fork" à jour

Si vous affichez la page d'accueil de votre "fork", vous constaterez que sa branche "master" n'est plus identique à celle de WordCampParis : c'est normal, vu qu'on vient de lui ajouter vos noms d'utilisateur·rice !

![Behind](https://dl.dropboxusercontent.com/s/emsu2bztqgzzhfr/19-sync-fork-compare.png)

La première flèche bleue vous montre la mention qui vous indique ce "retard", en cliquant sur le lien de comparaison pointé par la deuxième, vous pouvez démarrer le processus de synchronisation de votre "fork".

![Sync start](https://dl.dropboxusercontent.com/s/9mzkfwhvjdoq8vp/20-sync-fork-compare-view.png)

S'"il n'y a rien à comparer" lors de cette première étape, c'est que vous comparez dans le mauvais sens. Pour comparer dans le bon sens vous allez commencer par redéfinir la liste déroulante de base sur votre fork, comme illustré ci-dessous.

![Base fork](https://dl.dropboxusercontent.com/s/v8cn2jilx5nrh7d/21-sync-fork-compare-view-prbranch.png)

Du coup, en faisant cette opération, vous allez comparer exactement la même chose !

![Across](https://dl.dropboxusercontent.com/s/4z75377p4ot9q5g/22-sync-fork-compare-across-forks.png)

Il s'agit donc comme le montre la flèche bleue d'étendre la comparaison à tous les forks disponibles.

![Head fork](https://dl.dropboxusercontent.com/s/ftu2c3d5qhuwdp8/23-sync-fork-compare-set-upstream.png)

Vous pouvez désormais définir la liste déroulante "head fork" sur celui de WordCampParis afin de faire apparaître les "commits" qu'il manque à votre fork.

![Compare master/upstream](https://dl.dropboxusercontent.com/s/np1f17wn6zxpy6z/24-sync-fork-pull-request.png)

En plus de la liste des commits, vous trouverez une nouvelle zone à fond jaune dans laquelle le bouton qui s'intitule "Create pull request" vous permettra de modifier votre branche "master" pour qu'elle soit synchronisée avec celle de WordCampParis. Cliquez sur ce bouton !

![Pull request to sync](https://dl.dropboxusercontent.com/s/tssd5lr3rfcvf7p/25-sync-fork-commit-pr.png)

Vous ouvrez l'écran de création de "Pull Request", cette fois-ci c'est normal que ce soit votre fork qui soit l'objet de cette demande de modification. Validez cette demande en cliquant sur le bouton "Create pull request".

![Confirm merge](https://dl.dropboxusercontent.com/s/4bsi5nc68uw0cke/26-sync-fork-merge-pr.png)

Il ne vous reste plus qu'à confirmer la fusion des deux branches en cliquant sur le bouton "Merge pull request".

![Tada](https://dl.dropboxusercontent.com/s/wa4ho0rpz6xnzvh/27-sync-fork-merged-pr.png)

Bravo ! Votre fork est bien synchronisé avec le dépôt de WordCampParis, vous pouvez créer d'autres modifications dans une nouvelle branche comme vu plus tôt avec l'exemple de l'insertion de vos noms d'utilisateurs dans le fichier `CONTRIBUTORS.md`.

