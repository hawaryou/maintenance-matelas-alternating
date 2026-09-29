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
