Setting Up Location Alerts
==========================

The command to add a new alert is:

::

	!alert pokemon=<name> distance=<distance> iv=<iv> cp=<cp> level=<level> excludemon=<exclusions>
	
* ``<name>`` - Compulsory. Here you can specify a single Pokémon by name, or use a built in group:

	* ``all`` refers to all Pokémon
	* ``gen1``, ``gen2``, ``gen3`` refers to all Pokémon in a generation.
	* ``ultra common``, ``common``, ``uncommon``, ``rare``, ``ultra rare`` refers to rarity tiers of Pokémon as decided by the admins. To see what’s in each tier, send Arceus the command ``!rarity <tier-name>`` – e.g. ``!rarity ultra rare.``
	
* ``<distance>`` - Compulsory. A decimal number specifying max distance from active location, interpreted in km. 

.. note::

	Don’t type km; just the number will do!
	
* ``<iv>``, ``<cp>``, ``<level>`` - Optional. Whole numbers specifying min IV (as a percentage), CP, level. 

.. note::

	You cannot specify all 3 of these in a single filter; between 0 and 2 of them is fine.
	
* ``<exclusions>`` - Optional. If you’ve chosen a group for ``<name>``, you can exclude individual Pokémon, Generations or Rarity Types by providing a comma-separated list here.

.. note::

	You can list Pokémon by name, or dex number.
	
warning::

	* Though you may omit optional parameters, you must **stick to the order** of parameters as outlined above.
	* Check there are **no spaces around any = sign**, and that you include only one space between separate parameters.
	
Example Commands
----------------

::

	!alert pokemon=dratini distance=1.5 iv=90

Creates an alert for all dratini within 1.5km with an IV over 90%	
	
::

	!alert pokemon=ultra rare distance=2 iv=80 cp=2000 excludemon=Blastoise
	
Creates an alert for all ultra rare pokémon within 2km that have an IV over 80% **and** a CP over 2000, exclusing Blastoise
	
::
	
	!alert pokemon=all distance=5 iv=100 excludemon=gen1,ultra common
	
Creates an alert for all 100% IV pokémon within 5km excluding ultra commons and anything gen1 pokémon