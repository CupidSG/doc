Ordinateurs
===========

Le terme **Ordinateur** dans GLPI est générique. Pour intégrer cette catégorie d'objet, un équipement doit posséder au minimum un processeur, un système d'exploitation et des logiciels installés.

Plusieurs équipements rentrent donc dans cette catégorie:

* Ordinateur avec unité centrale
* Ordinateur portable
* Serveur
* Smartphone
* Tablette

Dans la fiche d'un ordinateur, on trouve un certain nombre d'informations concernant le système d'exploitation (nom, version, service pack, numéro de série, product ID), les caractéristiques générales (fabricant, modèle, type, numéro de série), les informations de gestion (responsable technique, statut, localisation) et les usagers du poste (connus ou non dans GLPI).



D'autres champs sont informatifs, comme `Réseau` (type de connexion au poste), et la `source de la mise à jour` qui est un intitulé indiquant d'où proviennent les mises à jour d'un poste (oui/non, Windows update, yum, apt, etc).

.. note::

   * Dans le cas d'une utilisation de GLPI couplé avec un outil d'inventaire, différentes informations sur l'importation sont également disponibles.
   * Il est possible d'utiliser les :doc:`gabarits avec les ordinateurs <../generalites/gabarits>`.

Les différents onglets
----------------------

Ordinateur
~~~~~~~~~~

Premier onglet de l'objet, celui ci regroupe des informations généralistes comme:

* Le nom de l'objet dans GLPI, son fabricant et son modèle ;
* Son type, le lieu physique et son statut dans au sein du parc ;
* Son affectation auprès des membres de l'organisation ainsi que des groupes/utilisateurs de la plateforme.

D'autres champs viennent compléter cet onglet notamment pour l'identification technique de l'objet: 

* Numéro de série
* Numéro d'inventaire
* UUID

.. image:: images/computers-assets.png
        :alt: Fiche Ordinateur
        :align: center


.. include:: onglets/impact-analysis.rst

Systèmes d'exploitation
~~~~~~~~~~~~~~~~~~~~~~~

Dans cet onglet il est possible d'affecter un système d'exploitation à l'ordinateur.

.. note::
  * Les systèmes d'exploitations sont des intitulés dans GLPI, il est donc possible de les créer au préalable. 
  * En cas d'utilisation d'un outil d'inventaire tiers, ces informations peuvent être automatiquement importées et mises à jour !

.. image:: images/os-computers-assets.png
        :alt: Système d'exploitation d'un ordinateur
        :align: center

.. include:: onglets/composants.rst


Volumes
~~~~~~~

Dans cet onglet, sont gérés les volumes de l'ordinateur. Un volume lié à un ordinateur est caractérisé par son nom, la partition physique, son point de montage, son système de fichiers ainsi que sa taille. Il est également possible de définir la taille restant libre sur le volume.

.. note::
   En cas d'utilisation d'un outil d'inventaire tiers, ces informations peuvent être automatiquement importées et mises à jour.

.. image:: images/volumes-computers-assets.png
        :alt: Volumes liés à l'objet ordinateur
        :align: center

Logiciels (et licences)
~~~~~~~~~~~~~~~~~~~~~~~

Cet onglet permet d'associer à un ordinateur les logiciels et les licences existants déjà dans GLPI. Ceux-ci sont triés par catégorie et sont caractérisés par leur nom, leur version ainsi que le statut de cette dernière.

Si une licence est associée à l'utilisation de ce logiciel sur cet ordinateur, l'information sera également présentée.

.. note::

    * La liste déroulante énumère les logiciels disponibles dans l'entité.
    * En cas d'utilisation d'un outil d'inventaire tiers, les logiciels peuvent être automatiquement importés dans GLPI, associés à l'ordinateur et mettre à jour la liste à chaque actualisation de l'inventaire !

.. image:: images/softwares-computers-assets.png
        :alt: Logiciels et Licences installés sur un ordinateur
        :align: center

.. include:: onglets/connexions.rst

.. include:: onglets/ports-reseaux.rst

.. include:: onglets/gestion.rst

.. include:: ../onglets/contrats.rst

.. include:: ../onglets/documents.rst

Virtualisation
~~~~~~~~~~~~~~

Dans cet onglet, on retrouve tous les systèmes de virtualisation (machines virtuelles, containers, jails, ...) associés à un hôte (host) ou l'hôte sur lequel un système de virtualisation est installé. Les informations disponibles varient d'un système à l'autre, en fonction des information qu'il est effectivement possible d'obtenir.

pour une machine virtuelle par exemple, on trouvera son nom, son système de virtualisation, son modèle de virtualisation, l'état de la machine virtuelle, la mémoire allouée ainsi que le nom de la machine physique (hôte) et le nombre de processeurs logiques.

GLPI réalise actuellement la liaison entre un hôte et une machine virtuelle en se basant sur l'identifiant unique (uuid). Dans certains cas, il arrive que l'uuid soit différent au sein de la machine physique et virtuelle, la liaison est alors impossible.

Le seul moyen d'associer manuellement une machine virtuelle à une machine physique est d'attribuer à la machine virtuelle déclarée sur l'hôte et à la machine virtuelle dans GLPI un uuid identique.

.. note::

   En cas d'utilisation d'un outil d'inventaire tiers, ces informations peuvent être automatiquement importées et mises à jour.

.. include:: ../onglets/tickets.rst

.. include:: onglets/problemes.rst

.. include:: ../onglets/liens.rst

.. include:: ../onglets/notes.rst

-   **[Onglet "Réservations"](Les_différents_onglets/Onglet_Réservations.rst)**
     Gestion des réservations pour un objet d'inventaire

.. include:: ../onglets/historique.rst

.. include:: ../onglets/debug.rst

.. include:: ../onglets/all.rst

Les différentes actions
-----------------------

Outre les :doc:`actions communes <../generalites/actions>` ; certaines actions sont spécifiques aux ordinateurs :

* **Installer un logiciel avec licence sur un ordinateur**
    Depuis l'onglet *Logiciels*, ajouter une licence en choisissant le nom du logiciel suivi du nom de la licence.
    Depuis les actions de masse du tableau récapitulatif, choisissez **Installer**.

    .. warning::

       Un logiciel ne peut être installé que si sa licence possède une version d'achat et/ou d'utilisation.
