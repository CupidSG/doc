Alias de port réseau
====================

Un alias de port réseau est un port virtuel qui peut spécialiser un port physique.

Sous Linux, chaque :term:`VLAN`, lorsqu'il est transmis « :term:`taggé <VLAN Taggé>` », est associé à un alias de port (``eth2.50`` pour représenter le VLAN ``50`` sur le port ``eth2``).

Un alias de port comporte son port d'origine (celui sur lequel il s'appuie) et une adresse MAC.

.. warning::

   Lorsque l'on change le port d'origine, l'adresse MAC du nouveau port d'origine est affecté à l'alias de port.