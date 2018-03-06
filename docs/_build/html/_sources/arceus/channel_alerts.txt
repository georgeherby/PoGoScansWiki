*************************
Setting Up Channel Alerts
*************************

.. contents:: :local:

Adding A New Alert
##################

.. warning::

	Channel alerting is unavailable in London. Please see :doc:`here </arceus/intro>` for the reason why.
	
If you want to set up alerts for Pokémon spawns, initiate a conversation with Arceus by typing into bot-commands:

::

    !arceus
	
This will get Arceus to send you a message. Use this DM window to send all commands. 

The command to add a new alert is:

::

	!alert pokemon=<name> channel=<channel> area=<area> iv=<iv> cp=<cp> level=<level> excludemon=<monexclusions> excludearea=<areaexclusions>
	
* ``<name>`` - Compulsory. Here you can specify a single Pokémon by name, or use a built in group:

	* ``all`` refers to all Pokémon
	* ``gen1``, ``gen2``, ``gen3`` refers to all Pokémon in a generation.
	* ``ultra common``, ``common``, ``uncommon``, ``rare``, ``ultra rare`` refers to rarity tiers of Pokémon as decided by the admins. To see what’s in each tier, send Arceus the command ``!rarity <tier-name>`` – e.g. ``!rarity ultra rare``
	
* ``<channel>`` - Compulsory. The channel for which you want alerting. 

.. note::

	To see the list of available channels, type ``!channels`` in the **bot-commands** channel in discord!
	
* ``<area>`` - Compulsory. The area for which you want alerting. This can be a single area, or use ``all`` to get alerts for all areas in a channel.

.. note::

	The areas are those in () in the spawn posts in discord. A list of areas in each channel can be found in the **readme** on discord.
	
.. warning::

	There is no validation of the ``<area>`` parameter, so if you misspell the area name, your alert will not work.
	
* ``<iv>``, ``<cp>``, ``<level>`` - Optional. Whole numbers specifying min IV (as a percentage), CP, level. 

.. note::

	You cannot specify all 3 of these in a single filter; between 0 and 2 of them is fine.
	
* ``<monexclusions>`` - Optional. If you’ve chosen a group for ``<name>``, you can exclude individual Pokémon, Generations or Rarity Types by providing a comma-separated list here.

.. note::

	You can list Pokémon exclusions by name, or dex number.
	
* ``<areaexclusions>`` - Optional. If you’ve chosen ``all`` for the ``<area>``, you can exclude certain areas from generating an alert by providing a comma-separated list here.
	
.. warning::

	* Though you may omit optional parameters, you must **stick to the order** of parameters as outlined above.
	* Check there are **no spaces around any = sign**, and that you include only one space between separate parameters.
	
Example Commands
----------------

::

	!alert pokemon=dratini channel=Brighton area=Patcham iv=90

Creates an alert for all dratini In Patcham with an IV over 90%	
	
::

	!alert pokemon=ultra rare channel=Reading area=All iv=80 cp=2000 excludemon=Blastoise excludearea=Henley
	
Creates an alert for all ultra rare pokémon in Reading that have an IV over 80% **and** a CP over 2000, excluding Blastoise and any spawns in Henley.
	
::
	
	!alert pokemon=all channel=Oxford area=All iv=100 excludemon=gen1,ultra common excludearea=Bicester
	
Creates an alert for all 100% IV pokémon in Oxford excluding ultra commons and any gen1 pokémon. Do not send alert if in Bicester.

Removing, Muting Or Unmuting Alerts
###################################

By ID
-----

First run :doc:`show </arceus/show>` command above and note the alert id for the record you
want to remove.

Once you have the alert id, use this command to remove, mute or unmute the alert

::

    !alert remove 32        ------ 32 being the ID you want to remove
    !alert mute 32          ------ 32 being the ID you want to mute
    !alert unmute 32        ------ 32 being the ID you want to unmute

All alerts
----------

::

    !alert remove all       ------ This will remove all raid alerts
    !alert mute all         ------ This will mute all raid alerts
    !alert unmute all       ------ This will unmute all raid alerts
	
By Location
-----------

You can remove, mute or unmute all alerts for a channel or an area within a channel:

::

    !alert remove channel=MidSussex
    !alert remove channel=MidSussex area=Hassocks
	
::

    !alert mute channel=Reading
    !alert mute channel=Reading area=Caversham
	
::

    !alert unmute channel=Slough
    !alert unmute channel=Slough area=Britwell

.. note::

	If removing by area, channel is still required.