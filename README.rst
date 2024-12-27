==============
ApolloPyClient
==============


.. image:: https://img.shields.io/pypi/v/ApolloPyClient.svg
        :target: https://pypi.python.org/pypi/ApolloPyClient

.. image:: https://img.shields.io/travis/gcj-bit/ApolloPyClient.svg
        :target: https://travis-ci.com/gcj-bit/ApolloPyClient

.. image:: https://readthedocs.org/projects/ApolloPyClient/badge/?version=latest
        :target: https://ApolloPyClient.readthedocs.io/en/latest/?version=latest
        :alt: Documentation Status




A Python SDK that is easy to integrate with the Apollo configuration management syste.



Usage
--------
```python
    client = ApolloClient(
        app_id=os.environ.get('APOLLO_APP_ID'),
        config_service_url=os.environ.get('APOLLO_CONFIG_URL'),
        cluster=os.environ.get('APOLLO_CLUSTER'),
        secret=os.environ.get('APOLLO_SECRET'),
        env=os.environ.get('APOLLO_ENV'),
        namespaces=['application', 'test', 'testjson.json', 'testyaml.yaml'],
        ignore_ssl_verify=True,
    )
    print(client.all())
    # sleep for 100000 seconds, you can view log to get the config
    time.sleep(100000)

```
