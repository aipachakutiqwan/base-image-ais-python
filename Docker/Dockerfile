#FROM gccaisolutionsucs/leap-poller:base
#FROM nexus3.nex.intranet.unicreditgroup.eu:9080/dai/leap-poller:base
#FROM leap-poller:base
FROM nexus3.nex.intranet.unicreditgroup.eu:9080/dai/p2t-poller:base

ARG REPONAME=p2t-poller

WORKDIR /home/${REPONAME}

# Creation of logs
RUN mkdir /home/${REPONAME}/logs
RUN touch /home/${REPONAME}/logs/${REPONAME}.log && \
    chown ${REPONAME}:${REPONAME} /home/${REPONAME}/logs/${REPONAME}.log
RUN chmod -R 777 /home/${REPONAME}/logs

ADD src /home/${REPONAME}/src
ADD config /home/${REPONAME}/config

ENV PYTHONPATH "${PYTHONPATH}:/home/${REPONAME}"
CMD ["python", "./src/main_app.py"]
USER ${REPONAME}

