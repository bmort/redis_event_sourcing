[![Build Status](https://travis-ci.com/bmort/redis_event_sourcing.svg?branch=master)](https://travis-ci.com/bmort/redis_event_sourcing)

# Experimental SIP EC configuration database events library

This builds an API around ideas from the Event Sourcing pattern
and the idea that SBIs and PBs can be thought of as a DDD Aggregate.

## Quickstart

The unit tests for the library require that a Redis instance to
be available on localhost on the default Redis port.

This can be started with Docker using the following command:

```bash
docker run -d -p 6379:6379 --name=redis redis:4.0.6-alpine
```

Once Redis is available, unit tests and linters can be run with the
following command:

```bash
pytest -s -v --codestyle --docstyle --pylint .
```

In order to inspect the data stored in the database it can also
be useful to run the RedisCommander web UI. Thi can be done
with the following command:

```bash
TODO
```

Once started, this provides a web UI to the database at
<http://localhost:8081>
