Workflow outgoing_msg in ChannelMessage
=========================================================

ChannelMessage States
-------------------------------------

* created
* dispatched
* delivered
* error

ChannelMessage Transitions
----------------------------------------
#. send_to_dispatcher
#. dispatch_error
#. deliver

The Workflow
------------

.. figure::  /images/workflows/outgoing_msg.png

   Workflow outgoing_msg
