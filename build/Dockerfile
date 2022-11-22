FROM icr.io/appc-dev/ace-server@sha256:a41f7501fe4025d2705bcabf1ad2ff523bcaf9ec263b98054501de1fc0cf5f62

ENV LICENSE=accept

COPY initial-config/ /home/aceuser/initial-config/

USER root

RUN . /opt/ibm/ace-12/server/bin/mqsiprofile

RUN /opt/ibm/ace-12/server/bin/mqsicreateworkdir /home/aceuser/ace-server-test

USER aceuser
