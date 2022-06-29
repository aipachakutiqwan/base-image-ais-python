#FROM python:3.10.4-slim-buster
FROM python:3.10-slim
RUN apt-get update
ARG USERNAME=ai-solutions
RUN groupadd -r ${USERNAME} -g 103 && \
    useradd -u 102 -r -g ${USERNAME}  -m -d /home/${USERNAME}  -s /sbin/nologin -c "${USERNAME} user" ${USERNAME}  && \
    chmod 755 /opt
USER ${USERNAME}