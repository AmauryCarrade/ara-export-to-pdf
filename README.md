# Export d’audits Ara en PDF

Ce dépôt contient deux _user styles_ permettant d’exporter en PDF un audit réalisé avec Ara,
l’outil web développé par la DINUM.

Les _user styles_ fonctionnent en modifiant les feuilles d’impression pour permettre l’export
en PDF des audits par le biais de l’impression en PDF. L’affichage web n’est pas altéré.

## Utilisation

Il y a deux styles à utiliser : un pour la première page (qui conserve toutes les en-têtes
de l’audit et les met en forme), et un pour les autres pages (qui retire toute en-tête afin
que le contenu puisse être ajouté à la suite du premier PDF).

1. Activez le style **Partie 1**, uniquement. Si le style **Partie 2** est actif,
   désactivez-le.
2. Exportez en PDF la première section (par exemple, l’onglet _Observations_ où
   vous aurez rédigé une introduction à l’audit), en utilisant la fenêtre d’impression
   puis _Imprimer en PDF_ (ou similaire).
3. En conservant ce style activé, activez le second style **Partie 2** : ce dernier
   supprimera les en-têtes des exports subséquents.
4. Exporter toutes les autres sections de la même manière, avec les deux styles appliqués.
5. Fusionnez les PDFs ainsi obtenus, dans le bon ordre.

---

_Attention : en fonction des navigateurs, il n’est pas garanti que le PDF exporté par impression soit accessible._
