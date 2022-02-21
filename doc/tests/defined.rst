``defined``
===========

``defined`` проверяет, определена ли переменная в текущем контексте. Это очень
полезно при использовании опции ``strict_variables``:

.. code-block:: twig

    {# defined работает с именами переменных #}
    {% if foo is defined %}
        ...
    {% endif %}

    {# и атрибутами в именах переменных #}
    {% if foo.bar is defined %}
        ...
    {% endif %}

    {% if foo['bar'] is defined %}
        ...
    {% endif %}

When using the ``defined`` test on an expression that uses variables in some
method calls, be sure that they are all defined first:

При использовании ``defined`` для проверки выражения, в котором используются переменные
в некоторых вызовах методов, убедитесь, что все они определены в первую очередь:
.. code-block:: twig

    {% if var is defined and foo.method(var) is defined %}
        ...
    {% endif %}
