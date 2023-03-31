> Quelles étapes (steps) sont réalisées par cette action ?

Récupération du dépôt, installation des dépendances, linting et tests.

> Une étape est définie au minimum par 2 éléments, lesquels sont-ils et à quoi servent-ils ?

Un nom et un élément à run (uses, run)

> La première étape contient le mot-clé ‘with’, a quoi sert-il ?

Passer une valeur à l'action.

> Sur l’onglet Summary d’une analyse de code, SonarCloud fournit 4 indicateurs. Quels sont-ils et quelles sont leurs utilités ?

* Reliability : bug suceptible de provoquer des erreurs
* Maintainability : code difficile à maintenir
* Security : vulnérabilités
* Security review : portion de code contenant potentiellement des problèmes de sécurités à confirmer ou infirmer par un humain.


> À quoi sert l’indicateur Quality Gate ?

A s'assurer que le code soit prêt pour la production (Passed).


> Quelle est la différence entre les sections New code et Overall Code
dans l’onglet Summary ?

* New code : nouveau code
* Overall code : nouveau code + ancien code

> Y a-t-il des Code Smells ? Si oui, combien et pour quelle(s) raisons(s)
?

Oui, des paramètres de méthode inutilisés et des méthodes ayant exactement la même implémentation.

> Y a-t-il des Security Hotspots ? Si oui, combien et pour quelle(s)
raison(s) ?

Oui, l'image Docker utilise `root` comme utilisateur par défaut : c'est une mauvaise pratique et un risque de sécurité.