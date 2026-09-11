# 03 — Permissions et déchiffrement

Le chiffrement protège la valeur, mais l’accès au résultat exige une politique distincte.
Le sous-module `permits` représente les autorisations nécessaires aux opérations de déchiffrement.
Une permission relie identité, portée et action autorisée ; elle ne doit pas devenir un jeton global réutilisable.
Le SDK expose ensuite les flux de déchiffrement des poignées autorisées.
L’application doit vérifier domaine, chaîne et contrat avant de demander une signature.
Une interface claire doit distinguer consentement de lecture et transaction modifiant l’état.
La révocation et la durée de validité appartiennent au modèle de menace de l’intégration.
La sécurité réelle dépend donc autant des permissions que de la primitive FHE.

Suite : [React et états asynchrones](04-react-integration.md).
