Overview
========

A plugin to take the cdr and agent state information generated by OpenACD 
and publish in as protobufs in RabbitMQ.  This is meant to decouple OpenACD
from archiving and real-time reporting endpoints.

Building
========

    ./rebar get-deps compile

This will get required dependancies and package only what is absolutly 
needed for the plugin in './opacd_hop'.

Installing
==========

Place the entire 'oacd_hop' directory in OpenACD's plugins directory.  Then 
in OpenACD's shell:

    cpx:reload_plugins().