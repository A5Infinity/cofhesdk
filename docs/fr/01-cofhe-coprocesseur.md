# 01 — CoFHE comme couche de confidentialité

CoFHE permet à une application EVM de manipuler des valeurs chiffrées via un coprocesseur FHE.
Le contrat travaille avec des poignées plutôt qu’avec les données en clair.
Le SDK client prépare les entrées chiffrées et coordonne leur utilisation côté application.
Cette architecture conserve l’ergonomie EVM tout en déportant les opérations cryptographiques spécialisées.
Le dépôt regroupe le SDK principal, les liaisons React, les mocks et l’intégration Hardhat.
Chaque couche répond à une phase différente : chiffrement, autorisation, interface et développement.
La confidentialité n’est pas équivalente à l’anonymat : métadonnées et appels restent à examiner.
L’intégrateur doit identifier précisément quelles données sont chiffrées et lesquelles restent publiques.

Suite : [le cycle des entrées chiffrées](02-entrees-chiffrees.md).
