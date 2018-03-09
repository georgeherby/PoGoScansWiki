************************
Amending Existing Alerts
************************

.. contents:: :local:

Updating IV/CP/Level/Distance
#############################

.. note::

	You can either update 1 alert, or update multiple alerts at once

Change Minimum IV
-----------------

::

	!iv <ALERT_ID_REQUIRED> <NEW_IV_REQUIRED>  

For example ``!iv 3121 80``, to update a single alert.

::

	!iv <ALERT_ID_REQUIRED> <NEW_IV_REQUIRED>,<ALERT_ID_OPTIONAL> <NEW_IV_OPTIONAL> 

For example ``!iv 3121 80,3222 90,3333 60`` to update multiple alerts.


.. note::

	You can have as many ``<ALERT_ID_OPTIONAL> <NEW_IV_OPTIONAL>`` as you like separated by a comma, but make sure there is no space between commas.

Change Minimum CP
-----------------

::

	!cp <ALERT_ID_REQUIRED> <NEW_CP_REQUIRED>  

For example ``!cp 3121 1800``, to update a single alert.

::

	!cp <ALERT_ID_REQUIRED> <NEW_CP_REQUIRED>,<ALERT_ID_OPTIONAL> <NEW_CP_OPTIONAL> 

For example ``!cp 3121 2000,3222 1500,3333 2900`` to update multiple alerts.


.. note::

	You can have as many ``<ALERT_ID_REQUIRED> <NEW_CP_REQUIRED>`` as you like separated by a comma, but make sure there is no space between commas.

Change Minimum Level
--------------------

::

	!level <ALERT_ID_REQUIRED> <NEW_LEVEL_REQUIRED>  

For example ``!level 3121 30``, to update a single alert.

::

	!level <ALERT_ID_REQUIRED> <NEW_LEVEL_REQUIRED>,<ALERT_ID_OPTIONAL> <NEW_LEVEL_OPTIONAL>  

For example ``!level 3121 25,3222 30,3333 30`` to update multiple alerts.


.. note::

	You can have as many ``<ALERT_ID_OPTIONAL> <NEW_LEVEL_OPTIONAL>`` as you like separated by a comma, but make sure there is no space between commas.

Change Distance
---------------	

.. warning ::

	This command can only be used with location based alerts

::

	!distance <ALERT_ID_REQUIRED> <NEW_DISTANCE_REQUIRED>  

For example ``!distance 3121 2.5``, to update a single alert.

::

	!distance <ALERT_ID_REQUIRED> <NEW_DISTANCE_REQUIRED>,<ALERT_ID_OPTIONAL> <NEW_DISTANCE_REQUIRED>  

For example ``!distance 3121 2.5,3222 5,3333 0.5`` to update multiple alerts.

.. note::

	You can have as many ``<ALERT_ID_OPTIONAL> <NEW_DISTANCE_REQUIRED>`` as you like separated by a comma, but make sure there is no space between commas.


Updating Exclusions
###################

.. note::

	* This can only be done for one alert at a time. 
	* You can only exclude pokemon when the alert pokemon is set to ``all``, a generation or a rarity type.
	* You can only exclude areas when the alert area is set to ``all``
	* You can only exclude forms when the alert pokemon is set to ``all``, a generation, a rarity type or a pokemon that has forms, such as Unown.
	
.. warning::

	Area exclusion is only possible for channel based alerts.

Adding New Exclusion
--------------------

To append pokemon exclusions:

::

	!excludemon append id=1234 pokemon=rattata,common  

To append area exclusions:

::

	!excludearea append id=1234 area=Caversham,Earley  
	
To append form exclusions:

::

	!excludeform append id=1234 form=Normal,Sunny 

Replacing Existing Exclusions
-----------------------------

To replace pokemon exclusions:

::

	!excludemon replace id=1234 pokemon=pidgey 

To replace area exclusions:

::

	!excludearea replace id=1234 area=Kennington,Bicester  
	
To replace form exclusions:

::

	!excludeform replace id=1234 form=K,L,P

Deleting Exclusions
-------------------

To delete pokemon exclusions:

::

	!excludemon delete id=1234 pokemon=meditite

To delete area exclusions:

::

	!excludearea delete id=1234 area=Marlow
	
To delete form exclusions:

::

	!excludeform delete id=1234 form=Rainy

.. note::

	You can also delete all exclusions for pokemon or areas by using "all" for the final parameter, ie ``!excludemon delete id=1234 pokemon=all``, ``!excludearea delete id=1234 area=all`` or ``!excludeform delete id=1234 form=all``
	