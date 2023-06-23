<h1 align="center">Configuration</h1>

# Importing

```python
from tweeterpy import config
```

> ### Example - Config Usage

```python
from tweeterpy import TweeterPy
from tweeterpy import config

config.PROXY = {"http":"127.0.0.1","https":"127.0.0.1"}
config.TIMEOUT = 10

twitter = TweeterPy()

print(twitter.get_user_id('elonmusk'))

```

## Retries Limit

```python
# Maximun number of retries for each request
config.MAX_RETRIES = 3
```

## Request Timeout

```python
# request timeout - in seconds
config.TIMEOUT = 5
```

## Using Proxies

```python
# Example {"http":"proxy_here","https":"proxy_here"} Accepts python dictionary.
config.PROXY = None
```