:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/modules/visual_script/doc_classes/VisualScriptLocalVarSet.xml.

.. _class_VisualScriptLocalVarSet:

VisualScriptLocalVarSet
=======================

**Inherits:** :ref:`VisualScriptNode<class_VisualScriptNode>` **<** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

Changes a local variable's value.

Description
-----------

Changes a local variable's value to the given input. The new value is also provided on an output Data port.

\ **Input Ports:**\ 

- Sequence

- Data (variant): ``set``\ 

\ **Output Ports:**\ 

- Sequence

- Data (variant): ``get``

Properties
----------

+-----------------------------------------------------+------------------------------------------------------------------+------------------+
| :ref:`Variant.Type<enum_@GlobalScope_Variant.Type>` | :ref:`type<class_VisualScriptLocalVarSet_property_type>`         | ``0``            |
+-----------------------------------------------------+------------------------------------------------------------------+------------------+
| :ref:`StringName<class_StringName>`                 | :ref:`var_name<class_VisualScriptLocalVarSet_property_var_name>` | ``&"new_local"`` |
+-----------------------------------------------------+------------------------------------------------------------------+------------------+

Property Descriptions
---------------------

.. _class_VisualScriptLocalVarSet_property_type:

- :ref:`Variant.Type<enum_@GlobalScope_Variant.Type>` **type**

+-----------+---------------------+
| *Default* | ``0``               |
+-----------+---------------------+
| *Setter*  | set_var_type(value) |
+-----------+---------------------+
| *Getter*  | get_var_type()      |
+-----------+---------------------+

The local variable's type.

----

.. _class_VisualScriptLocalVarSet_property_var_name:

- :ref:`StringName<class_StringName>` **var_name**

+-----------+---------------------+
| *Default* | ``&"new_local"``    |
+-----------+---------------------+
| *Setter*  | set_var_name(value) |
+-----------+---------------------+
| *Getter*  | get_var_name()      |
+-----------+---------------------+

The local variable's name.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
