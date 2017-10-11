# mongo-redis-node-8

This image can be used as a base image for your projects. It contains mongo, redis and node 8.

The default WORKDIR is `/usr/src/app`

## Example

```docker
FROM concreteplatform/mongo-redis-node-8

ENV NODE_ENV=test

# Set environment path for mongodb
ENV MONGO_URL=mongodb://localhost/concrete-one-test
ENV DB_MONGO=localhost/concrete-one-test
ENV REDIS_URL=redis://localhost:6379
CMD ["bin/run-tests-in-docker.sh"]
```