FROM dai/python:3.10-slim
ARG USERNAME=python
RUN groupadd -r ${USERNAME} -g 103 && \
   useradd -u 102 -r -g ${USERNAME}  -m -d /home/${USERNAME}  -s /sbin/nologin -c "${USERNAME} user" ${USERNAME}  && \
   chmod 755 /opt

USER ${USERNAME}

RUN mkdir -p /home/${USERNAME}/agent