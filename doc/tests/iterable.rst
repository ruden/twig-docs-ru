``iterable``
============

``iterable`` проверяет, является ли переменная массивом или обходимым объектом:

.. code-block:: twig

    {# evaluates to true if the foo variable is iterable #}
    {% if users is iterable %}
        {% for user in users %}
            Привет {{ user }}!
        {% endfor %}
    {% else %}
        {# users is probably a string #}
        Привет {{ users }}!
    {% endif %}
