Regroupement
============

.. warning::
 Cette opération est irréversible !

Réaliser un regroupement
------------------------

* Si le logiciel n'existe pas dans l'entité mère, créer un logiciel dont le nom est strictement identique au nom du logiciel dans les entités filles ;
* Ouvrir la fiche du logiciel de l'entité mère ;
* Activer la récursivité (sous-entités à Oui en haut à droite), un nouvel onglet "Regroupement" apparaît après l'onglet "Historique" ;
* Ouvrir cet onglet, une liste indique les logiciels des entités filles ayant le même nom ;
* Sélectionner les lignes souhaitées et valider le regroupement via les actions massives.

Effets du regroupement
----------------------

* Les licences sont attachées au logiciel de l'entité mère, mais restent dans les sous-entités d'origine ;
* Les versions sont fusionnées (plus de doublon dans l'entité mère);
* Les anciens logiciels sont déplacés dans la corbeille ;

.. note::
 Lors de l'utilisation d'un outil d'inventaire tiers, ne pas oublier :

 * de vider la corbeille à la fin du regroupement (sinon la synchronisation restaurera le logiciel en cas de nouvelle version) ;
 * d'affecter le même fabricant au nouveau logiciel (la synchronisation vérifiant le nom du fabricant, un nouveau logiciel serait créé).