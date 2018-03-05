Nests
=====

The nests channel in discord contains all known nests with information gathered by yourselves. Shaymin is used to collate and display all this information.

Nest Types
----------

#. Large Spawn Area
#. Single Spawn Point
#. Multiple in One Point
#. Unknown 

Adding A New Nest
-----------------

To add a new nest use this command:

.. code-block:: bash

    !nest "channel" "Nest Name" "pokemon" <nest_type>
	
Example: ``!nest "Worthing" "Denton Garden" "Weedle" 1``

.. note::

	Before adding a new nest, please double check that the location does not already exist. If it does, use the below instead.

Updating A Nest After Migration
-------------------------------
	
Nests migrate every two weeks. When a migration has happened, We clear the pokemon from the nests. The information that needs repopulating with the new pokemon.	
	
To update a nest with no pokemon assigned to it:

.. code-block:: bash

    !update <nest_id> "pokemon Name"

Example: !update 1432 "Weedle"