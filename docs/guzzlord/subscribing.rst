***********
Subscribing
***********

.. contents:: :local:

Why Should I Subscribe?
#######################

There are many reasons why subscribing is possibly the best thing you could ever do :) Not only do you get the warm fuzzy feeling from knowing that your support is keeping this service running, 
but you also get ALL of the following goodies!!

* Access to the scan channels to see what is spawning in the areas you want to know about  
* Access to the map  
* Access to :doc:`Arceus </arceus/intro>`, our pokemon alert bot (for pokemon subscribers). This can be customised to alert you for pokemon based on location, IV, CP, Level and more.
* Access to :doc:`Dialga </dialga/intro>`, our raid alert bot. This can be customised to alert you to raids in your chosen area or at specific gyms.

Cost of Subscription
####################

We have implemented a new subscription model, so you can choose to sign up to what you want to get:

* Raids - £1 per 30 days
* Raids and Quests - £2 per 30 days
* Raid, Quests & Pokemon - £3 per 30 days

You can subscribe for whatever length of time you want; there is no maximum subscription but we would advise against subscribing too far into the future, due to the nature of our service. 
Niantic could enforce changes that would result in the potential closure of our service without much notice, and refunds will not be processed should this happen.

.. warning::

	Guzzlord will only read whole pound amounts, so if you pay £2.50, your subscription will only be for £2 worth.

How To Subscribe
################

Make Payment
============

Firstly, work out how much you want to pay by seeing how long an amount will get you using:

::

	!calculate amount

For example ``!calculate 5`` 

Make a payment via `PayPal <http://bit.ly/PoGoScans>`_. Make note of the transaction ID for the payment.

.. note::

	Payment can only be made in GBP, and must have a value of at least £1. Anything less will be rejected by Guzzlord. Also, payments cannot be processed until marked as 'Complete' in PayPal.

Apply Payment
=============

Go to the bot-commands channel and type:

::

    !subscribe
	
In DM with Guzzlord, type:
 
::

    !transaction <ID> <SubType>

where <ID> is the transaction ID you noted in step 1 and <SubType> is one of ``raids``, ``quests`` or ``pokemon``. If the transaction ID is correct and found on `PayPal <http://bit.ly/2igVOxV>`_, you will receive a response with your new subscription expiry date.

.. image:: subscribe_response.PNG

.. note::

	Please remember, if you are subscribing again after expiring, your map credentials will have changed and alerts will have been muted. If extending your subscription, your credentials will remain unchanged.
	
.. warning::

	ONLY CHOOSE 1 SUB TYPE! IF YOU WANT ALL TYPES, PICK POKEMON. THE TIERS WILL ALWAYS INCLUDE THE LOWER TIER!
 
Get Map Credentials
===================

Type:

::

    !map
	
In DM with Guzzlord to get the URL of the map, and your credentials for logging onto the map. If desired you can also change your password (see :ref:`changing password <passwordchange>`)

Expiration
==========

You will be sent a reminder 3 days before your subscription expires and again once it does. Should your subscription expire, the following will happen:

* Your map credentials will be deleted
* Your bot rights will be revoked
* Your active alerts will be muted
* You will no longer be able to see the scan channels
* You will no longer be able to see the subscriber only channels.

Your alerts will not be deleted until you leave the server in case you decide to re-subscribe.

You can always check your expiry date by typing:

::

	!expiry
	
What If I Do Not Have PayPal?
=============================

Unfortunately we only accept PayPal as a form of payment for subscription. We have found that 99% of people do have and are happy to use PayPal and we cannot process any other form of payment.
If you cannot use PayPal at all, our only suggestion is to liaise with a fellow PoGo player or friend that does use PayPal, and ask them to do it for you if you pay them.

There is no issue our side with this, and anybody can use the transaction ID generated, as long as it has not already been used.

.. _passwordchange:
	
Useful Commands 
###############

All commands must be done in DM with Guzzlord.

::

    !change_password newpassword
	
If you want to change your map password to something shorter or more memorable.

.. warning::

    Passwords are stored in the DB as plain text. Please do not use a password that you use elsewhere.
