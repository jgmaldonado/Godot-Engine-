:github_url: hide

.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the VisualShaderNodeCompare.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_VisualShaderNodeCompare:

VisualShaderNodeCompare
=======================

**Inherits:** :ref:`VisualShaderNode<class_VisualShaderNode>` **<** :ref:`Resource<class_Resource>` **<** :ref:`Reference<class_Reference>` **<** :ref:`Object<class_Object>`

A comparison function for common types within the visual shader graph.

Description
-----------

Compares ``a`` and ``b`` of :ref:`type<class_VisualShaderNodeCompare_property_type>` by :ref:`function<class_VisualShaderNodeCompare_property_function>`. Returns a boolean scalar. Translates to ``if`` instruction in shader code.

Properties
----------

+--------------------------------------------------------------------+--------------------------------------------------------------------+-------+
| :ref:`Condition<enum_VisualShaderNodeCompare_Condition>`           | :ref:`condition<class_VisualShaderNodeCompare_property_condition>` | ``0`` |
+--------------------------------------------------------------------+--------------------------------------------------------------------+-------+
| :ref:`Function<enum_VisualShaderNodeCompare_Function>`             | :ref:`function<class_VisualShaderNodeCompare_property_function>`   | ``0`` |
+--------------------------------------------------------------------+--------------------------------------------------------------------+-------+
| :ref:`ComparisonType<enum_VisualShaderNodeCompare_ComparisonType>` | :ref:`type<class_VisualShaderNodeCompare_property_type>`           | ``0`` |
+--------------------------------------------------------------------+--------------------------------------------------------------------+-------+

Enumerations
------------

.. _enum_VisualShaderNodeCompare_ComparisonType:

.. _class_VisualShaderNodeCompare_constant_CTYPE_SCALAR:

.. _class_VisualShaderNodeCompare_constant_CTYPE_SCALAR_INT:

.. _class_VisualShaderNodeCompare_constant_CTYPE_VECTOR:

.. _class_VisualShaderNodeCompare_constant_CTYPE_BOOLEAN:

.. _class_VisualShaderNodeCompare_constant_CTYPE_TRANSFORM:

enum **ComparisonType**:

- **CTYPE_SCALAR** = **0** --- A floating-point scalar.

- **CTYPE_SCALAR_INT** = **1** --- An integer scalar.

- **CTYPE_VECTOR** = **2** --- A 3D vector type.

- **CTYPE_BOOLEAN** = **3** --- A boolean type.

- **CTYPE_TRANSFORM** = **4** --- A transform (``mat4``) type.

----

.. _enum_VisualShaderNodeCompare_Function:

.. _class_VisualShaderNodeCompare_constant_FUNC_EQUAL:

.. _class_VisualShaderNodeCompare_constant_FUNC_NOT_EQUAL:

.. _class_VisualShaderNodeCompare_constant_FUNC_GREATER_THAN:

.. _class_VisualShaderNodeCompare_constant_FUNC_GREATER_THAN_EQUAL:

.. _class_VisualShaderNodeCompare_constant_FUNC_LESS_THAN:

.. _class_VisualShaderNodeCompare_constant_FUNC_LESS_THAN_EQUAL:

enum **Function**:

- **FUNC_EQUAL** = **0** --- Comparison for equality (``a == b``).

- **FUNC_NOT_EQUAL** = **1** --- Comparison for inequality (``a != b``).

- **FUNC_GREATER_THAN** = **2** --- Comparison for greater than (``a > b``). Cannot be used if :ref:`type<class_VisualShaderNodeCompare_property_type>` set to :ref:`CTYPE_BOOLEAN<class_VisualShaderNodeCompare_constant_CTYPE_BOOLEAN>` or :ref:`CTYPE_TRANSFORM<class_VisualShaderNodeCompare_constant_CTYPE_TRANSFORM>`.

- **FUNC_GREATER_THAN_EQUAL** = **3** --- Comparison for greater than or equal (``a >= b``). Cannot be used if :ref:`type<class_VisualShaderNodeCompare_property_type>` set to :ref:`CTYPE_BOOLEAN<class_VisualShaderNodeCompare_constant_CTYPE_BOOLEAN>` or :ref:`CTYPE_TRANSFORM<class_VisualShaderNodeCompare_constant_CTYPE_TRANSFORM>`.

- **FUNC_LESS_THAN** = **4** --- Comparison for less than (``a < b``). Cannot be used if :ref:`type<class_VisualShaderNodeCompare_property_type>` set to :ref:`CTYPE_BOOLEAN<class_VisualShaderNodeCompare_constant_CTYPE_BOOLEAN>` or :ref:`CTYPE_TRANSFORM<class_VisualShaderNodeCompare_constant_CTYPE_TRANSFORM>`.

- **FUNC_LESS_THAN_EQUAL** = **5** --- Comparison for less than or equal (``a <= b``). Cannot be used if :ref:`type<class_VisualShaderNodeCompare_property_type>` set to :ref:`CTYPE_BOOLEAN<class_VisualShaderNodeCompare_constant_CTYPE_BOOLEAN>` or :ref:`CTYPE_TRANSFORM<class_VisualShaderNodeCompare_constant_CTYPE_TRANSFORM>`.

----

.. _enum_VisualShaderNodeCompare_Condition:

.. _class_VisualShaderNodeCompare_constant_COND_ALL:

.. _class_VisualShaderNodeCompare_constant_COND_ANY:

enum **Condition**:

- **COND_ALL** = **0** --- The result will be true if all of component in vector satisfy the comparison condition.

- **COND_ANY** = **1** --- The result will be true if any of component in vector satisfy the comparison condition.

Property Descriptions
---------------------

.. _class_VisualShaderNodeCompare_property_condition:

- :ref:`Condition<enum_VisualShaderNodeCompare_Condition>` **condition**

+-----------+----------------------+
| *Default* | ``0``                |
+-----------+----------------------+
| *Setter*  | set_condition(value) |
+-----------+----------------------+
| *Getter*  | get_condition()      |
+-----------+----------------------+

Extra condition which is applied if :ref:`type<class_VisualShaderNodeCompare_property_type>` is set to :ref:`CTYPE_VECTOR<class_VisualShaderNodeCompare_constant_CTYPE_VECTOR>`.

----

.. _class_VisualShaderNodeCompare_property_function:

- :ref:`Function<enum_VisualShaderNodeCompare_Function>` **function**

+-----------+---------------------+
| *Default* | ``0``               |
+-----------+---------------------+
| *Setter*  | set_function(value) |
+-----------+---------------------+
| *Getter*  | get_function()      |
+-----------+---------------------+

A comparison function. See :ref:`Function<enum_VisualShaderNodeCompare_Function>` for options.

----

.. _class_VisualShaderNodeCompare_property_type:

- :ref:`ComparisonType<enum_VisualShaderNodeCompare_ComparisonType>` **type**

+-----------+----------------------------+
| *Default* | ``0``                      |
+-----------+----------------------------+
| *Setter*  | set_comparison_type(value) |
+-----------+----------------------------+
| *Getter*  | get_comparison_type()      |
+-----------+----------------------------+

The type to be used in the comparison. See :ref:`ComparisonType<enum_VisualShaderNodeCompare_ComparisonType>` for options.
