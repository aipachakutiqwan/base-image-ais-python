FROM gccaisolutionsucs/base-image-ais-python:3.10.4RUN apt-get update
ARG USERNAME=ai-solutions
RUN groupadd -r ${USERNAME} -g 103 && \
    useradd -u 102 -r -g ${USERNAME}  -m -d /home/${USERNAME}r  -s /sbin/nologin -c "${USERNAME} user" ${USERNAME}  && \
    chmod 755 /opt
USER ${USERNAME}
