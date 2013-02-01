# Mock for the redis-py client library

Supports writing tests for code using the [redis-py][redis-py] library 
without requiring a [redis-server][redis] install.

This package will hopefully (soon) cover entire redis-py offering

## Install

    pip install redismock
    
## Usage

    from redismock import mockmanager
    redis_client = mockmanager.mock_redis_client()
    redis_client.set("key","value")
    redis_client.get("key")

## Attribution

This code is shamelessly derived from work by [John DeRosa][john] [locationlabs][locationlabs].

[redis-py]: https://github.com/andymccurdy/redis-py
[redis]:    http://redis.io
[john]:     http://seeknuance.com/2012/02/18/replacing-redis-with-a-python-mock/

