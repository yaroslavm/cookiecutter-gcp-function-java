{% set is_open_source = cookiecutter.open_source_license != 'Not open source' -%}
{% for _ in cookiecutter.project_name %}={% endfor %}
{{ cookiecutter.project_name }}
{% for _ in cookiecutter.project_name %}={% endfor %}

{{ cookiecutter.project_short_description }}

{% if is_open_source %}
* Free software: {{ cookiecutter.open_source_license }}
{% endif %}

Features
--------

* TODO

Credits
-------

This package was created with Cookiecutter_ and the `yaroslavm/cookiecutter-gcp-function`_ project template.

.. _Cookiecutter: https://github.com/audreyr/cookiecutter
.. _`yaroslavm/cookiecutter-gcp-function-java`: https://github.com/yaroslavm/cookiecutter-gcp-function-java
