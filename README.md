# Dockerfile

# Step1 specify the base image

FROM alpine

# Download and install dependencies

RUN apk add --update redis

# Setup the startup command

CMD ["redis-server"]
