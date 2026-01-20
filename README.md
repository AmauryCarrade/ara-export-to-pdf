# Export d’audits Ara en PDF

Ce dépôt contient deux _user styles_ permettant d’exporter en PDF un audit réalisé avec Ara,
l’outil web développé par la DINUM.

Les _user styles_ fonctionnent en modifiant les feuilles d’impression pour permettre l’export
en PDF des audits par le biais de l’impression en PDF. L’affichage web n’est pas altéré.

## Installation

Vous devez au préalable avoir une extension de gestion de styles utilisateur installée sur votre navigateur (par exemple, Stylus, disponible sur [Firefox](https://addons.mozilla.org/firefox/addon/styl-us/) et [Chrome](https://chromewebstore.google.com/detail/stylus/clngdbkpkpeebahjckkjfobafhncgmne)).

Ensuite, cliquez sur ces liens pour installer les styles : **[Partie 1](https://github.com/AmauryCarrade/ara-export-to-pdf/raw/refs/heads/main/ara-export-to-pdf-partie-1.user.css)** – **[Partie 2](https://github.com/AmauryCarrade/ara-export-to-pdf/raw/refs/heads/main/ara-export-to-pdf-partie-2.user.css)**.

Ils seront mis à jour automatiquement en cas d’évolution, si l’extension utilisée le supporte.

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

### Fusionner des PDFs

Pour fusionner des PDFs, vous pouvez :
- utiliser un service web, tel que [Adobe Acrobat (web)](https://www.adobe.com/acrobat/online/merge-pdf.html), [iLovePDF](https://www.ilovepdf.com/merge_pdf), ou [Smallpdf](https://smallpdf.com/merge-pdf) ;
- utiliser PDFtk en GUI (Windows, Linux, macOS) ou en ligne de commande : `pdftk partie1.pdf partie2.pdf ... cat output audit.pdf` ;
- sous macOS, utiliser Aperçu (par copier-coller des pages d’un PDF à l’autre).

---

_**Attention** : en fonction des navigateurs, il n’est pas garanti que le PDF exporté par impression soit pleinement accessible._
