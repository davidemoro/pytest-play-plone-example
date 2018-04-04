``pytest-play`` basic example that shows how to automate a Plone login using
parametrized tests based on pure json scenarios. It is just a hello world
test for demonstrative purpose.

Prerequisites:

* geckodriver (https://github.com/mozilla/geckodriver/releases)

How to run the tests::

  $ virtualenv --no-site-packages --python $(which python3.6) python
  $ source python/bin/activate
  $ pip install -r requirements.txt
  $ pytest --variables env-ALPHA.yml --splinter-webdriver firefox --splinter-screenshot-dir /tmp -x

See:

* https://github.com/tierratelematics/pytest-play/pull/51
* https://www.plone-demo.info
* https://www.plone.org
