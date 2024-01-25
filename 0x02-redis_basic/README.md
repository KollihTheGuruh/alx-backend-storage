# Redis Integration Tasks

This project involves several tasks focused on integrating Redis with Python, using Redis both locally and within a container. These tasks are part of the "alx-backend-storage" repository, located in the "0x02-redis_basic" directory.

## Prerequisites

- Ubuntu 18.04
- Python 3
- Redis server

### Install Redis on Ubuntu 18.04

To install Redis on Ubuntu 18.04, run the following commands:

```bash
sudo apt-get -y install redis-server
pip3 install redis
sed -i "s/bind .*/bind 127.0.0.1/g" /etc/redis/redis.conf
```

## Tasks Overview

### Task 0: Writing Strings to Redis

**File**: `exercise.py`

- Implement a `Cache` class with a `__init__` method that stores an instance of the Redis client as a private variable `_redis` and flushes the instance using `flushdb`.
- Create a `store` method to generate a random key, store input data in Redis using this key, and return the key.

### Task 1: Reading from Redis and Recovering Original Type

**File**: `exercise.py`

- Create a `get` method to retrieve data from Redis and convert it back to the desired format.
- Implement `get_str` and `get_int` methods for automatic conversion of the retrieved data into strings or integers.

### Task 2: Incrementing Values

**File**: `exercise.py`

- Implement a `count_calls` decorator to count how many times methods of the `Cache` class are called.
- Decorate `Cache.store` with `count_calls`.

### Task 3: Storing Lists

**File**: `exercise.py`

- Define a `call_history` decorator to store the history of inputs and outputs for a function in Redis.
- Decorate `Cache.store` with `call_history`.

### Task 4: Retrieving Lists

**File**: `exercise.py`

- Implement a `replay` function to display the history of calls of a particular function.

### Task 5: Implementing an Expiring Web Cache and Tracker

**File**: `web.py`

- Implement a `get_page` function to cache the HTML content of URLs with an expiration time of 10 seconds and track the number of times a URL was accessed.
