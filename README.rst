``pytest-play`` basic example that shows how to automate a Plone login using
parametrized tests based on pure json scenarios. It is just a hello world
test for demonstrative purpose.

Prerequisites:

* geckodriver (https://github.com/mozilla/geckodriver/releases)

How to run the tests::

  $ virtualenv --no-site-packages --python $(which python3.6) python
  $ source python/bin/activate
  $ pip install -r https://raw.githubusercontent.com/davidemoro/cookiecutter-qa/master/%7B%7Bcookiecutter.project_slug%7D%7D/requirements.txt
  $ pytest --variables env-ALPHA.yml --splinter-webdriver firefox --splinter-screenshot-dir /tmp -x

In addition a bzt/Taurus ``index.yml`` file is provided too (suitable for a BlazeMeter cloud run with ``bzt index.yml``).

See:

* https://www.plone-demo.info
* https://www.plone.org

``pytest-play`` is shipped by default by a more opinionated cookiecutter scaffolding tool with many options (selenium grid ready,
Jenkins integration, etc). Have a look at:

* https://github.com/davidemoro/cookiecutter-qa
