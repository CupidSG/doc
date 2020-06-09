Ports réseau
~~~~~~~~~~~~~

Dans cet onglet, il est possible de matérialiser le ou les port(s) réseau associé(s) à un matériel. 

Un port réseau permet de modéliser la sortie d'une interface réseau sur un matériel donné. Chaque port est caractérisé par un numéro et un nom.

Sur ce port, il est possible d'ajouter un ou plusieurs réseaux virtuels (VLAN), ces derniers peuvent être définis par un nom, un commentaire et un numéro de VLAN (TAG ID).

Pour chaque matériel, il est possible à tout moment d'ajouter un ou plusieurs ports grâce au système de modification massive.

Sur chaque port réseau, on peut associer un ou plusieurs [nom réseau](08_Module_Configuration/02_Intitulés/06_Intitulés_Internet.rst "Un nom réseau correspond à l'identification unique d'une machine du point de vue d'Internet.").
On peut ajouter plusieurs noms réseau en allant dans l'onglet "Nom réseau".

* Lorsqu'il n'y a qu'un seul nom réseau, il s'affichera dans le formulaire du port réseau et il sera possible de le modifier directement. On peut également modifier le nom réseau au travers de son formulaire propre (avec ses onglets) en cliquant sur le titre juste au dessus de la partie du formulaire qui le concerne.
* Lorsqu'il y a plusieurs noms réseau, il n'est plus possible de modifier le nom réseau dans le formulaire du port réseau. On doit systématiquement utiliser l'onglet.

Les ports réseau peuvent être de différents types. Il y a des ports physiques (Ethernet, Wifi ...), :ref:`virtuels <Port réseau virtuel>` (boucle locale, alias, aggrégats ...), point à point (ligne commutée) ...

L'onglet des ports réseau représente l'ensemble de ports disponibles sur l'équipement dans un tableau. Dans l'en-tête du tableau, à côté du nombre total de port, il y a un lien permettant de choisir les options
d'affichage des ports réseaux. Il est ainsi possible d'afficher ou de masquer des informations telles que les informations réseau (tout ce qui concerne Internet), les caractéristiques intrinsèques du port (ie. dépendant de son type), les adresses MAC, les VLANs ...

.. note::

   * GLPI permet de représenter fidèlement des connexions réseau très complexes avec des alias ports Wifi et/ou Ethernet associés à des VLAN regroupés dans aggrégats (voir ci-dessous).
   * Pour un port réseau d'un type d'objet ordinateurs, le champ MAC avec la liste déroulante permet de sélectionner l'adresse MAC des composants de type carte réseau.

* :doc:`Ports réseau de type Ethernet <onglets/ethernet-ports-reseau>`
* :doc:`Ports réseau de type Wifi <onglets/wifi-ports-reseau>`
* :doc:`Ports réseau de type boucle locale <onglets/bouclelocale-ports-reseau>`
* :doc:`Ports réseau de type Alias de port réseau <onglets/alias-ports-reseau>`
* :doc:`Ports réseau de type Aggrégats de ports réseau <onglets/alias-ports-reseau>`