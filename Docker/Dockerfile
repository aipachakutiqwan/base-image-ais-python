#FROM python:3.10.4-slim-buster
FROM nexus3.nex.intranet.unicreditgroup.eu:9080/dai/p2t-ocr:base_p2t_ocr_v_0.0.2
ARG USERNAME=ai-solutions
#RUN groupadd -r ${USERNAME} -g 103 && \
#    useradd -u 102 -r -g ${USERNAME}  -m -d /home/${USERNAME}  -s /sbin/nologin -c "${USERNAME} user" ${USERNAME}  && \
#    chmod 755 /opt
USER ${USERNAME}