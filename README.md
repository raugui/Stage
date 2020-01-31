# Stage chez Huggi

On ma demandé d'effectuer deux petits projets parmis les autres tâches réalisées.
Par soucis de confidentialité du code, voici uniquement les demandes en détails. 
Celles-ci ont étaient réalisées et terminées.

# Demande de devis pour un utilisateur

La demande 

Permettre à un utilisateur de faire un panier, une fois le panier effectué il aura le choix entre effectuer un devis (sans se connecter) ou alors valider la commande. (Il devra se connecter/créer un compte)
Le fournisseur pourra consulter le devis dans son panneau d’administration "mes commandes".
Note : 
Utilisateur : Personne qui n’a pas d’identifiant client.

Idée en détail 

Utilisateur :

-	Permettre à un utilisateur d’ajouter des articles à un panier.
-	Permettre à un utilisateur d’accéder au panier.
-	Permettre à un utilisateur d’effectuer un devis à partir de son panier :
o	Seulement pour certains fournisseurs.
o	Seulement pour certains articles du fournisseur.
-	Lorsque le devis est effectué, l’utilisateur ET le fournisseur reçoivent le devis par mail en pièce jointe au format PDF.
-	Si l’utilisateur se connecte/s’inscrit, son panier (non connecté) sera transféré dans son panier lié à son compte. Les articles ne pouvant être ajouté au panier (restriction de fin de collaboration fournisseur par exemple) ne seront pas ajoutés et donc retirés du panier.

Fournisseur :
-	Le fournisseur lorsqu’il sera dans son interface de commandes, il aura la possibilité de voir le devis de l’utilisateur.

Action 

Lorsque l’utilisateur ajoute des articles à son panier, puis le consulte, il aura deux choix qui s’offrent à lui :
-	Passer commande :
o	On lui demandera de se connecter ou de s’inscrire.
-	Demander un devis :
o	On lui demandera d’indiquer les informations suivantes dans un formulaire :
	Nom
	Prénom
	E-mail
	Adresse
	Nom société 
	Numéro de téléphone (facultatif)
 Message personnel
o	Lorsque les informations seront validées, il pourra faire la demande de devis. 

# Permettre aux utilisateurs d'émettre un avis et un commentaire sur un article, ainsi que d'émettre un avis sur un commentaire.

Permettre à un utilisateur d’émettre un avis et un commentaire sur un article précédemment commandé.
Permettre à un utilisateur connecté de voir les commentaires et de les trouver « utile » ou « inutile » en fonction de leurs utilités.
Le top commentaire sera jugé en fonction des « utiles » « inutiles » et le meilleur sera sélectionné automatiquement et mis en évidence.
Permettre au fournisseur de décider s’il veut ou non afficher les commentaires sur ses articles.
Permettre à l’administrateur d’administrer les commentaires. (Attente d’acceptation de l’administrateur pour être visible)

Idée en détail

Utilisateur :

-	Lorsqu’un client aura effectué une commande, quelques semaines plus tard il recevra un mail avec un lien pour lui permettre d’ajouter un commentaire et un avis sur les articles commandé.

Administrateur :

-	Il pourra gérer les commentaires dans un espace dédié.

Fournisseur :

-	Décide si les commentaires apparaissent sur ses articles.

Action 

Utilisateur :
-	Lorsque le client aura cliqué sur le lien, il arrivera sur une fenêtre. Sur cette fenêtre il y’aura ses articles commandés ainsi qu’un espace commentaire et un espace avis (étoiles, note de 1à5). Il aura juste à valider son choix pour chaque article. S’il n’émet pas d’avis, l’avis sera par défaut à une note de 3/5. Le client n’est pas obligé de rédiger un commentaire. Celui-ci peut être nul.
-	Lorsque le client aura effectué un commentaire/avis sur un article, il passera en attente de validation. 
-	Le client aura la possibilité d’émettre un avis sur un commentaire (utile ou inutile) d’un article. 

Administrateur :
-	L’administrateur possède un espace de gestion des commentaires. Celui-ci pourra consulter les commentaires émis, il pourra voir les informations suivantes :
o	Nom du client
o	Nom de l’article
o	Image de l’article
o	Note émise du client
o	Commentaire du client
o	Date d’émission
o	Le fournisseur de l’article
-	Il pourra ainsi valider ou non le commentaire. S’il le valide, le commentaire apparaitra sur la fiche article du produit.

Fournisseur :

-	Les fournisseurs peuvent décider ou non si les commentaires apparaissent sur les articles. (demande à l’administrateur)

Système :

-	Le système calculera automatiquement le meilleur commentaire par article, et il l’affichera en top commentaire (en haut de la liste des commentaires) et sera mis en évidence. Il sera calculé par les avis des utilisateurs sur les commentaires.
-	Les commentaires seront triés par date d’émission.

