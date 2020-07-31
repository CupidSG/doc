Imprimantes
===========

Dans la fiche d'une imprimante, plusieurs informations sont disponibles:

-   Sur les caractéristiques générales de l'imprimante (le fabricant, le modèle, le type, le numéro de série...) ;
-   Sur la gestion de l'imprimante (le responsable technique, son statut, le lieu où elle se trouve...) ;
-   Sur les usagers de l'imprimante (connus ou non dans GLPI, groupe d'utilisateurs...) ;
-   Sur ses spécifications (le compteur de page initial, les types de ports...).

**Description du type de gestion :**

Il est possible de gérer les imprimantes de manière unitaire ou globale.

La gestion unitaire correspond à une gestion classique (une imprimante pour un ordinateur) alors que dans la gestion globale, l'imprimante devient un élément virtuel global qui sera connecté à plusieurs ordinateurs.

La gestion globale permet de limiter le nombre d'éléments à gérer dans le cas où ceux-ci ne constituent pas une donnée stratégique dans la gestion du parc informatique.

.. note::
	Il est possible d'utiliser les :doc:`gabarits avec les imprimantes <../generalites/gabarits>`.

Les différents onglets
----------------------

.. include:: onglets/composants.rst

Cartouches
~~~~~~~~~~

Dans cet onglet, il est possible de gérer les cartouches associées au modèle d'imprimante sélectionné.

Il se décompose en deux parties :

* Les cartouches utilisées, avec comme information les dates d'ajout et d'utilisation,
* Les cartouches usagées, avec comme information le modèle de cartouche, les dates d'ajout, d'utilisation et de fin de vie, le compteur de l'imprimante ainsi que le nombre de pages imprimées depuis le dernier changement de cartouche.

.. note::

   Pour la création ou la suppression de cartouche reportez-vous à :doc:`la gestion des cartouches <cartouches>`.

.. include:: onglets/connexions.rst

.. include:: onglets/ports-reseaux.rst

.. include:: onglets/gestion.rst

.. include:: ../onglets/contrats.rst

.. include:: ../onglets/documents.rst

.. include:: ../onglets/tickets.rst

.. include:: onglets/problemes.rst

.. include:: ../onglets/liens.rst

.. include:: ../onglets/notes.rst

.. include:: onglets/reservations.rst

.. include:: onglets/certificats.rst

.. include:: onglets/domains.rst

.. include:: onglets/appliances.rst

.. include:: ../onglets/historique.rst

.. include:: ../onglets/debug.rst

.. include:: ../onglets/all.rst


Les différentes actions
-----------------------

*   :doc:`Ajouter une imprimante <../../Les_différentes_actions/creer_un_nouvel_objet>`
*   :doc:`Visualiser une imprimante <../../Les_différentes_actions/visualiser_un_objet>`
*   :doc:`Modifier une imprimante <../../Les_différentes_actions/modifier_un_objet>`
*   :doc:`Supprimer une imprimante <../../Les_différentes_actions/supprimer_un_objet>`
*   :doc:`Associer un document à une imprimante <../../Les_différentes_actions/associer_un_document_a_un_objet>`
*   :doc:`Transférer une imprimante <../../Les_différentes_actions/transferer_un_objet>`
