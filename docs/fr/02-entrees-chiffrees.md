# 02 — Le cycle des entrées chiffrées

`@cofhe/sdk` récupère les clés FHE nécessaires au chiffrement des entrées.
Le chargement est différé jusqu’à l’exécution de `client.encryptInputs(...).execute()`.
L’initialisation du module TFHE suit la même stratégie paresseuse.
Cette décision réduit le coût initial pour les parcours qui n’ont pas encore besoin de chiffrer.
Les adaptateurs web et Node isolent les différences d’environnement d’exécution.
Les types d’entrée chiffrée rendent la largeur attendue explicite dans l’API.
Une application doit éviter de journaliser la valeur claire avant son chiffrement.
Elle doit aussi traiter comme sensibles les données temporaires et erreurs de sérialisation.

Suite : [permissions et déchiffrement](03-permissions-dechiffrement.md).
