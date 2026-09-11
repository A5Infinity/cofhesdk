# 05 — Mocks, périmètre et limites

`@cofhe/mock-contracts` reproduit localement des comportements utiles au développement sans offrir la confidentialité FHE réelle.
Le plugin Hardhat automatise le déploiement de ces doubles et les utilitaires associés.
Un test avec mock valide un flux applicatif, pas la sécurité cryptographique du coprocesseur.
Les environnements simulés doivent être clairement séparés des configurations destinées à un réseau réel.
Ce parcours couvre SDK, adaptateurs, permissions, React et outillage de simulation.
Il ne couvre pas l’implémentation cryptographique interne du coprocesseur ni son audit.
Le dépôt évolue rapidement ; les exports et migrations documentés doivent être relus avant intégration.
Aucune installation, compilation ou exécution n’a été effectuée ; `test/` et les tests de packages restent les références de validation.
