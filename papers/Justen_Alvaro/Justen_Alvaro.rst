:author: Álvaro Justen
:email: alvarojusten@gmail.com
:institution: Fundação Getúlio Vargas (Rio de Janeiro, Brazil)

:author: Flávio Amieiro
:email: flavioamieiro@gmail.com
:institution: Fundação Getúlio Vargas (Rio de Janeiro, Brazil)

--------------------------------
pyquality: analyzing Python code
--------------------------------

.. class:: abstract

    ``pyquality`` is a tool to measure Python code quality with a focus on
    *rich reports* that take into account the *history of the code*.

    Still in an early development stage, ``pyquality`` analyses the conformity
    to PEP8 standards throughout a project's history and generates a full
    report including a video showing the evolution of the code, focusing on its
    quality.

    We aim to make it easy to include new analysis and reports, and also
    support different version control systems (only Git is supported for now).

.. class:: keywords

    code quality, python, software development, free software


Installation
------------

To install a stable version, install it directly from `PyPI
<http://pypi.python.org/>`_ using ``pip``:

.. code-block:: bash

    pip install pyquality

You can also clone pyquality's repository and install our ``develop`` branch:

.. code-block:: bash

    git clone git@github.com:NAMD/pyquality.git
    cd pyquality
    python setup.py install


Using it
--------

Once you've installed `pyquality`, a command called `pyquality` will be
available in your system/virtualenv. To create a report based on a existing Git
repository, just execute:

.. code-block:: bash

    pyquality /path/to/Git/repository

If do you want to create a report based on a remote Git repository, just
replace the path with the URL, for example, to run `pyquality` against its own
repository, execute:

.. code-block:: bash

        pyquality git@github.com:NAMD/pyquality.py
