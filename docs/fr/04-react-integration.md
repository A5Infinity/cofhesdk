# 04 — React et états asynchrones

`@cofhe/react` fournit des hooks et composants au-dessus du SDK principal.
L’interface doit représenter séparément initialisation, chiffrement, soumission et déchiffrement.
Ces étapes peuvent dépendre d’un portefeuille, d’un réseau et d’un bloc récemment finalisé.
Une boucle d’attente bornée évite qu’un écran reste indéfiniment dans un faux état de progression.
Les erreurs cryptographiques ne doivent pas être absorbées comme de simples erreurs d’affichage.
Un changement de compte ou de chaîne invalide le contexte courant et doit déclencher une réévaluation.
Les composants React simplifient l’usage, mais ne remplacent pas la gestion explicite de ces transitions.
La couche UI fait donc partie du périmètre de sûreté d’une application confidentielle.

Suite : [mocks, limites et validation](05-mocks-limites.md).
