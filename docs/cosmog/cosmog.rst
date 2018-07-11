Trading
=======

Do you have a specific Pokémon missing in your Pokédex? Desperate for a shiny? Then Cosmog is for you....

Using Cosmog, you can make requests for pokémon or make offers for existing requests. There is a trade channel per area.  

.. warning::

	Cosmog is for **requesting** Pokémon, not offering. If you have something to offer, find a request for that Pokémon.

Adding A New Trade Request
--------------------------

To add a new trade request use this command:

.. code-block:: bash

     !trade pokemon=<pokemon> form=<form> shiny=<yes/no> new=<yes/no>
	 
.. note::
	The **form** and **new** parameters are optional. The command will work without adding these. If left out, the new parameter will default to Yes. Only include form if requesting Unown letters or event mons like Party Hat Pikachu.

	
Examples: 

``!trade pokemon=Wailmer shiny=yes``
``!trade pokemon=Unown form=C shiny=no new=yes``
``!trade pokemon=Wailmer shiny=yes new=no``

Making An Offer For a Trade
---------------------------

If you find an open request for a Pokémon that you have and are willing to trade, you can start a negotiation with that player. To do so:

.. code-block:: bash

     !trade negotiate <ID>
	 
This will initiate a DM to both users advising the other that an offer has been made. It is then down to the two players to arrange this via DM. The trade status then changes to **In Discussion** but remians in the overview list.

.. note::
	Only **Open** requests can be negotiated. Once a trade is in negotiation, nobody else can make an offer for this trade.


After Negotation
----------------
	
There are two possible outcomes for a trade negotiation. Either the two players agree to meet and trade, or an agreement cannot be reached. 

Trade Agreed
~~~~~~~~~~~~

If the trade is agreed upon, the requesting player should type the following in DM with Cosmog:

.. code-block:: bash

     !complete <ID>
	
This will set the trade as completed and remove it from the overview list.
	 
Trade Not Agreed
~~~~~~~~~~~~~~~~
	 
If no agreement can be reached, the requesting player should type the following in DM with Cosmog:

.. code-block:: bash

     !decline <ID>
	
This will set the trade as open again, and new players can initiate a negotiation. 

Removing Requests
-----------------

If you happen to catch the mon that you created a request for, you can always remove the trade request by typing the following in DM with Cosmog:

.. code-block:: bash

     !remove <ID>
	
.. note::
	You cannot remove a request that is in discussion. If you no longer need this mon, you should decline the negotiation before removing, in order to let the other player know.
