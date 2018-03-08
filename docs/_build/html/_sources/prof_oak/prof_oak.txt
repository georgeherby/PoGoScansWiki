********
Prof Oak
********

.. contents:: :local:

IV Checker
##########

You can use Prof Oak to get IVs for your catches, using a few pieces of information.

Not Powered Up
--------------

This option is for catches or hatches that haven't been powered up. IC checking is easier for mons that have not been powered up as there are no half levels to consider:

::

	!groudon cp=2873 hp=128 stardust=4000 
	
Will return the following:

.. image:: not_poweredup_groudon.png

Powered Up
----------

If you have powered up your mon, add the poweredup parameter to your command:

::

	!venusaur cp=2283 hp=130 stardust=7000 poweredup=true
	
This will likely return more results, as includes half levels if possible

.. image:: powered_up_venusaur.png

Pokémon Stats
#############

These commands will provide you with all the notification you need for pokemon.

::

	!eevee
	
.. image:: eevee.png

Eggs
####

Get details for egg hatches such as rarity and CP range:

::

	!egg 2
	
Returns a list of all possible 2km eggs.

.. image:: egg_distance.png

.. note::

	Only 2, 5 or 10 can be used here.

::

	!egg Lapras
	
Tells you what distance egg the pokemon appears in, along with rarity type and possible CP range.

.. image:: egg_pokemon.png

Raid Bosses
###########

Get details for raid bosses and their counters

::

	!boss 4
	
Will returns a list of all level 4 bosses.

.. image:: boss_level.png

::

	!boss tyranitar
	
Provides details information about Tyranitar as a raid boss.

.. image:: boss_pokemon.png
