# BASE-IMAGE_AI_SOLUTIONS

This repository implement the base image base for all AI Solutions projects, it is based in python:3.10-slim.

The base image in nexus is named nexus3.nex.intranet.unicreditgroup.eu:9080/dai/base-image-ais-python:3.10-slim.
This base image has only one high vulnerability due to pip. We should always use pip upgrade for the componentwise docker container creation to remove this vulnerability, when the fix is available.

