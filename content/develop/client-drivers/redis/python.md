
## Installation

Install the python driver using the following command.

```
sudo pip install redis
```

## Working Example

### Pre-requisites

This tutorial assumes that you have:

- installed YugaByte DB, created a universe and are able to interact with it using the CQL and Redis shell. If not, please follow these steps in the [quick start guide](/quick-start/test-cql/).


### Writing the python code

Create a file `yb-redis-helloworld.py` and add the following content to it.

```python
import redis

# Create the cluster connection.
r = redis.Redis(host='localhost', port=6379)

# Insert the user profile.
userid = 1
user_profile = {"name": "John", "age": "35", "language": "Python"}
r.hmset(userid, user_profile)
print "Inserted userid=1, profile=%s" % user_profile

# Query the user profile.
print r.hgetall(userid)
```

### Running the application

To run the application, type the following:

```sh
python yb-redis-helloworld.py
```

You should see the following output.

```sh
Inserted userid=1, profile={'age': '35', 'name': 'John', 'language': 'Python'}
{'age': '35', 'name': 'John', 'language': 'Python'}
```