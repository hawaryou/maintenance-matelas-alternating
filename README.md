# ENR09-V02 — Maintenance système compresseur matelas à air

Application web mobile inspirée du projet ENR08-V05 de maintenance des lits médicalisés. La checklist reprend la fiche ENR09-V02 fournie.

Fonctionnalités conservées :
- maintenance annuelle ou périodique ;
- lecture QR Code, Data Matrix, Code 128 et EAN-13 par caméra ou photo ;
- contrôle visuel et fonctionnel avec choix conforme / non conforme ;
- PDF de maintenance avec état global, signatures, observations, pièces changées et niveau d’obsolescence ;
- envoi du PDF par e-mail via Google Apps Script ;
- mode normal et tournée multi-équipements avec une seule signature client pour tous les certificats.

## Mode multi-équipements

1. Démarrer une tournée multi-équipements.
2. Renseigner et contrôler chaque système compresseur / matelas à air.
3. Enregistrer l’équipement pour passer au suivant.
4. Terminer la tournée et recueillir une seule signature client.
5. Générer un PDF regroupant tous les certificats, ou l’envoyer par e-mail.

Le mode normal produit un certificat par équipement.

## Déploiement

Publier les fichiers du dépôt sur GitHub Pages. Pour l’envoi e-mail, déployer `Code.gs` comme application Web Google Apps Script et vérifier le destinataire configuré avant mise en service.


## Aperçu, envoi et confidentialité

- Le bouton « Aperçu / Télécharger PDF » ouvre le document généré dans une fenêtre de prévisualisation.
- Le bouton « Aperçu puis envoyer » ouvre le même aperçu ; l'envoi ne démarre qu'après clic sur « Valider et envoyer par e-mail ».
- La notice « Confidentialité et données personnelles » est accessible depuis le pied de page, y compris sur mobile. Elle doit être complétée et validée par EuroMed avant usage réel.
- Le menu graphique « Menu » en haut à gauche renvoie vers le HUB EuroMed.

Attention : une notice dans l'application ne suffit pas à garantir la conformité RGPD. Vérifier notamment les durées de conservation, les rôles et responsabilités, la base légale, les droits des personnes, les sous-traitants et les mesures de sécurité.
