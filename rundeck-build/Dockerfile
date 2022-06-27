FROM rundeck/rundeck:4.2.1

USER root

RUN export DEBIAN_FRONTEND=noninteractive && \
    apt-get update && \
    apt-get -qqy install --no-install-recommends git sshpass nmap python3 python3-pip python3-setuptools ansible && \
    apt-get clean && \
    python3 -m pip install bs4 requests
USER rundeck
