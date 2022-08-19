.. You should enable this project on travis-ci.org and coveralls.io to make
   these badges work. The necessary Travis and Coverage config files have been
   generated for you.

.. image:: https://travis-ci.org/''/ckanext-idgotheme.svg?branch=master
    :target: https://travis-ci.org/''/ckanext-idgotheme

.. image:: https://coveralls.io/repos/''/ckanext-idgotheme/badge.svg
  :target: https://coveralls.io/r/''/ckanext-idgotheme

.. image:: https://pypip.in/download/ckanext-idgotheme/badge.svg
    :target: https://pypi.python.org/pypi//ckanext-idgotheme/
    :alt: Downloads

.. image:: https://pypip.in/version/ckanext-idgotheme/badge.svg
    :target: https://pypi.python.org/pypi/ckanext-idgotheme/
    :alt: Latest Version

.. image:: https://pypip.in/py_versions/ckanext-idgotheme/badge.svg
    :target: https://pypi.python.org/pypi/ckanext-idgotheme/
    :alt: Supported Python versions

.. image:: https://pypip.in/status/ckanext-idgotheme/badge.svg
    :target: https://pypi.python.org/pypi/ckanext-idgotheme/
    :alt: Development Status

.. image:: https://pypip.in/license/ckanext-idgotheme/badge.svg
    :target: https://pypi.python.org/pypi/ckanext-idgotheme/
    :alt: License

=============
ckanext-idgotheme
=============

.. Put a description of your extension here:
   What does it do? What features does it have?
   Consider including some screenshots or embedding a video!


------------
Requirements
------------

For example, you might want to mention here which versions of CKAN this
extension works with.


------------
Installation
------------

.. Add any additional install steps to the list below.
   For example installing any non-Python dependencies or adding any required
   config settings.

To install ckanext-idgotheme:

1. Activate your CKAN virtual environment, for example::

     . /usr/lib/ckan/default/bin/activate

2. Install the ckanext-idgotheme Python package into your virtual environment::

     pip install ckanext-idgotheme

3. Add ``idgotheme`` to the ``ckan.plugins`` setting in your CKAN
   config file (by default the config file is located at
   ``/etc/ckan/default/production.ini``).

4. Restart CKAN. For example if you've deployed CKAN with Apache on Ubuntu::

     sudo service apache2 reload


---------------
Config Settings
---------------

Document any optional config settings here. For example::

    ckanext.idgotheme.name = IDGO
    ckanext.idgotheme.readthedocs = https://readthedocs.idgo
    ckanext.idgotheme.url_site_wp = https://publier.idgo
    ckanext.idgotheme.url_site_publier = https://publier.idgo
    ckanext.idgotheme.url_site_extracteur = https://extracteur.idgo
    ckanext.idgotheme.extent = -5.6 41 9.9 51.4


------------------------
Development Installation
------------------------

To install ckanext-idgotheme for development, activate your CKAN virtualenv and
do::

    git clone https://github.com/''/ckanext-idgotheme.git
    cd ckanext-idgotheme
    python setup.py develop
    pip install -r dev-requirements.txt


-----------------
Running the Tests
-----------------

To run the tests, do::

    nosetests --nologcapture --with-pylons=test.ini

To run the tests and produce a coverage report, first make sure you have
coverage installed in your virtualenv (``pip install coverage``) then run::

    nosetests --nologcapture --with-pylons=test.ini --with-coverage --cover-package=ckanext.idgotheme --cover-inclusive --cover-erase --cover-tests


---------------------------------
Registering ckanext-idgotheme on PyPI
---------------------------------

ckanext-idgotheme should be availabe on PyPI as
https://pypi.python.org/pypi/ckanext-idgotheme. If that link doesn't work, then
you can register the project on PyPI for the first time by following these
steps:

1. Create a source distribution of the project::

     python setup.py sdist

2. Register the project::

     python setup.py register

3. Upload the source distribution to PyPI::

     python setup.py sdist upload

4. Tag the first release of the project on GitHub with the version number from
   the ``setup.py`` file. For example if the version number in ``setup.py`` is
   0.0.1 then do::

       git tag 0.0.1
       git push --tags


----------------------------------------
Releasing a New Version of ckanext-idgotheme
----------------------------------------

ckanext-idgotheme is availabe on PyPI as https://pypi.python.org/pypi/ckanext-idgotheme.
To publish a new version to PyPI follow these steps:

1. Update the version number in the ``setup.py`` file.
   See `PEP 440 <http://legacy.python.org/dev/peps/pep-0440/#public-version-identifiers>`_
   for how to choose version numbers.

2. Create a source distribution of the new version::

     python setup.py sdist

3. Upload the source distribution to PyPI::

     python setup.py sdist upload

4. Tag the new release of the project on GitHub with the version number from
   the ``setup.py`` file. For example if the version number in ``setup.py`` is
   0.0.2 then do::

       git tag 0.0.2
       git push --tags
