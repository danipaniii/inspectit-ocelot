FROM busybox

ADD inspectit-ocelot-agent.jar /
RUN ln /inspectit-ocelot-agent.jar /javaagent.jar &&\
    chmod -R go+r /javaagent.jar

ADD entrypoint.sh  /
ENTRYPOINT ["sh", "/entrypoint.sh"]