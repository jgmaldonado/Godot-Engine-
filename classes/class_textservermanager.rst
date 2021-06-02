:github_url: hide

.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the TextServerManager.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_TextServerManager:

TextServerManager
=================

**Inherits:** :ref:`Object<class_Object>`

Manager for the font and complex text layout servers.

Description
-----------

``TextServerManager`` is the API backend for loading, enumeration and switching :ref:`TextServer<class_TextServer>`\ s.

Note: Switching text server at runtime is possible, but will invalidate all fonts and text buffers. Make sure to unload all controls, fonts, and themes before doing so.

Methods
-------

+-------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`TextServer<class_TextServer>` | :ref:`find_interface<class_TextServerManager_method_find_interface>` **(** :ref:`String<class_String>` name **)** |const|            |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`TextServer<class_TextServer>` | :ref:`get_interface<class_TextServerManager_method_get_interface>` **(** :ref:`int<class_int>` index **)** |const|                   |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`               | :ref:`get_interface_count<class_TextServerManager_method_get_interface_count>` **(** **)** |const|                                   |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`               | :ref:`get_interface_features<class_TextServerManager_method_get_interface_features>` **(** :ref:`int<class_int>` index **)** |const| |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`String<class_String>`         | :ref:`get_interface_name<class_TextServerManager_method_get_interface_name>` **(** :ref:`int<class_int>` index **)** |const|         |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Array<class_Array>`           | :ref:`get_interfaces<class_TextServerManager_method_get_interfaces>` **(** **)** |const|                                             |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`TextServer<class_TextServer>` | :ref:`get_primary_interface<class_TextServerManager_method_get_primary_interface>` **(** **)** |const|                               |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`             | :ref:`set_primary_interface<class_TextServerManager_method_set_primary_interface>` **(** :ref:`int<class_int>` index **)**           |
+-------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------+

Method Descriptions
-------------------

.. _class_TextServerManager_method_find_interface:

- :ref:`TextServer<class_TextServer>` **find_interface** **(** :ref:`String<class_String>` name **)** |const|

Finds an interface by its name.

----

.. _class_TextServerManager_method_get_interface:

- :ref:`TextServer<class_TextServer>` **get_interface** **(** :ref:`int<class_int>` index **)** |const|

Returns the interface registered at a given index.

----

.. _class_TextServerManager_method_get_interface_count:

- :ref:`int<class_int>` **get_interface_count** **(** **)** |const|

Returns the number of interfaces currently registered.

----

.. _class_TextServerManager_method_get_interface_features:

- :ref:`int<class_int>` **get_interface_features** **(** :ref:`int<class_int>` index **)** |const|

Returns text server supported features (binary OR).

----

.. _class_TextServerManager_method_get_interface_name:

- :ref:`String<class_String>` **get_interface_name** **(** :ref:`int<class_int>` index **)** |const|

Returns the interface name registered at a given index.

----

.. _class_TextServerManager_method_get_interfaces:

- :ref:`Array<class_Array>` **get_interfaces** **(** **)** |const|

Returns a list of available interfaces the index and name of each interface.

----

.. _class_TextServerManager_method_get_primary_interface:

- :ref:`TextServer<class_TextServer>` **get_primary_interface** **(** **)** |const|

Returns the primary :ref:`TextServer<class_TextServer>` interface.

----

.. _class_TextServerManager_method_set_primary_interface:

- :ref:`bool<class_bool>` **set_primary_interface** **(** :ref:`int<class_int>` index **)**

Sets (and initializes it if required) interface registered at a given index as the primary. Invalidates all references to the fonts and text buffers.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`