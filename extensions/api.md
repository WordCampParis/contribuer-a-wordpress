# L’API des extensions

L’API des extensions repose majoritairement sur les fonctions liées aux crochets (« hooks » en anglais) de WordPress. La compréhension du fonctionnement des crochets de WordPress est fondamentale pour toute contributrice et tout contributeur du projet open source. Si ces crochets ont d’abord été pensés pour s’adresser prioritairement aux auteur·e·s d’extensions, les auteur·e·s de thèmes et plus récemment de blocs de l’éditeur moderne en ont également besoin pour leurs créations.

## Les crochets

Les crochets permettent à un morceau de code d’agir ou de réagir par rapport à un autre morceau de code. Ils constituent les fondamentaux de l’extension et de la personnalisation de WordPress par les extensions et les thèmes. WordPress lui-même les utilise pour son propre code.

Il existe deux types de crochet : les **actions** et les **filtres**.

### Les actions

Elles permettent d’intégrer l’exécution d’un morceau de code personnalisé à un moment précis du chargement du code de WordPress.

_Exemple_
WordPress utilise le crochet d’action `personal_options_update` pour générer une notification à l’ancienne adresse e-mail de l’utilisateur qui vient de modifier son adresse e-mail depuis sa page d’administration de profil. L’e-mail en question contient un lien pour valider ce changement d’adresse.

### Les filtres

Ils permettent à un morceau de code personnalisé de modifier la valeur de la variable auquel s’applique le filtre avant de renvoyer cette valeur au code de WordPress. WordPress poursuit alors le reste de son chargement en prenant en compte cette valeur modifiée.

_Exemple_
WordPress utilise le crochet de filtre `the_content` pour effectuer l’interprétation des blocs du contenu d'un article.

WordPress propose de nombreux crochets dans son code source. Ce qui permet aux extensions de modifier ou d’enrichir son comportement et aux thèmes de personnaliser l’apparence de la partie frontale du site. Extensions et thèmes peuvent eux aussi proposer leurs propres crochets d’action ou de filtre.

Référence : [Manuel de développement des extensions de WordPress](https://developer.wordpress.org/plugins/hooks/)
