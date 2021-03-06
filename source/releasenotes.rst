Release Notes
=============

1.3.1
_____

*Release date 01 Nov 2016*

**Bug Fix**

* #66 - Do not allow incidents for disabled events


1.3.0
_____

*Release date 25 Mar 2016*

**New Features**

*  Modify JIRA ticket for existing incident

* Bulk toggle of incidents

* Bulk JIRA assignment of incidents

* minor bugfixes

1.1.0
_____

*Release date 2 Sep 2015*

**New Features**

* JIRA support

* Reports based on time range

* Sorting of incidents based on time and count

* migrates to Travis' container build system

1.0.0
-----

*Release date 21 Jun 2015*

**New Features**

* event suppression

* better application layout and installation script

* integration of listener within the engine

* use gevent for asynchronous processing of incidents

* supports Django 1.8 (with new migrations)


**Bugfixes**

many..


0.11.0
------

**New Features**

* get detailed list of incidents from most alerted elements

* search incidents based on elements

* view username for acknowledged and closed incidents

**Bugfixes**

* retry rabbitmq connection without crashing

* better handling of messages (including retries) if DB connection drops

* cleaner connection handler for rabbitmq_read

* close connection after writing a message

* increase default log rotation on 100MB

* changes EventSearchForm to show updated team listings

* removes obsolete dispatcher module

* removes boolean comparison for NoneType in get_report_all_incidents



0.10.0
------

* LDAP authentication support.

* Auto-refreshing dashboards.

* Search elements/hosts.

* Generate report for most alerted elements/hosts.

* Pagination for event code display.

* Show plugin server's name along with plugin names.

* Lots of bug-fixes.

0.9.3
-----

* Fixes bug where team list was not getting updated when adding users.

* Adds more validation to JSON strings accepted while adding incidents.

0.9.2
-----
* Fixes a critical template bug that didn't allow adding plugin servers on fresh installation.

* Couple of minor bug fixes.

0.9.1
-----

* Updated the helper scripts in bin directory.

0.9.0
-----

* Added RabbitMQ support.

* Added bulk event creation feature (Tools -> Add events in bulk).

* Added ability to export events in CSV.

* UI will not allow creating events with duplicate summaries in the same category within user's team.

* Updated Django==1.6.5, Twisted==13.2.0, zope.interface==4.1.0

* Launched the `integration_tools`_ repository to help integrate with 3rd party tools.

* Lots of unittests, minor bug fixes, removal of cruft, etc.

.. _integration_tools: https://github.com/CitoEngine/integration_tools

0.8.0
-----

* Initial release
