pytest-play example (Plone login with parametrized tests based on pure json scenarios)::

  $ virtualenv --no-site-packages --python $(which python3.6) python
  $ source python/bin/activate
  $ pip install -r requirements.txt
  $ pytest --variables env-ALPHA.yml --splinter-webdriver firefox --splinter-screenshot-dir /tmp -x
