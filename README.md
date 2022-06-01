# BASE-IMAGE_AI_SOLUTIONS

This repo implement the base image base for all the projects


How was created the immage base?

1. pull python:3.10.4-buster from docker hub
2. remove openssl from this image since Prisma detected a vulnerability for this package
3. build a new image to be push to docker hub
    docker build -f Dockerfile.base -t gccaisolutionsucs/base-image-ais-python:3.10.4
4. 