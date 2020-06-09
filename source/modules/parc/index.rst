Module Parc
===========

Le module Parc de GLPI est destiné à la gestion des matériels et logiciels composants le parc informatique de l'organisation.


La gestion de l'inventaire dans GLPI
------------------------------------

GLPI, nativement, est un outil statique. Il permet de lister les équipements et logiciels mais une intervention humaine est nécessaire pour saisir les informations et les mettre à jour.

Cependant, automatiser la remontée d'informations est possible en couplant GLPI avec un outil tiers spécialisé. Ainsi GLPI propose l'utilisation de 2 plugins existants :

* Le plugin `Fusion Inventory <https://github.com/fusioninventory/fusioninventory-for-glpi/>`_ disponible sur Github.

   Il transforme GLPI en serveur d'inventaire (les agents discutent directement avec GLPI)

   Vous pouvez également consulter le `site officiel de FusionInventory <http://www.fusioninventory.org>`_.

* Le plugin `ocsinventoryng <https://github.com/pluginsGLPI/ocsinventoryng>`_ disponible sur Github.

   Il permet de synchroniser la base GLPI avec un l'outil d'inventaire `OCS Inventory NG <http://www.ocsinventory-ng.org>`_ (les agents des équipements du parc discutent avec le serveur OCS Inventory NG).

Objets disponibles
-----------------

Chaque objet implémenté dans GLPI bénéficie d'une "fiche". Cette fiche regroupe toutes les informations relatives à l'objet séparées en différents onglets.

.. toctree::
   :maxdepth: 1

   ordinateurs
   moniteurs
   logiciels
   licenses
   materiels-reseaux
   peripheriques
   imprimantes
   cartouches
   consommables
   telephones
   global

.. todo::

   Référencé dans la doc originale, mais non présent :

   * **[Gestion du protocole Internet (IP)](../glpi/inventory_ip.html)**\
      Le protocole IP est matérialisé sous plusieurs formes : adresses
      IP, réseaux IP, mais aussi des FQDN
