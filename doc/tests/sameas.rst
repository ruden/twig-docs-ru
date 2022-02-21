``same as``
===========

``same as`` проверяет, совпадает ли переменная с другой переменной.
Это эквивалентно ``===`` в PHP:

.. code-block:: twig

    {% if foo.attribute is same as(false) %}
        атрибут foo действительно является 'false' PHP значением
    {% endif %}
