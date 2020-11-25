FROM node
SHELL ["/bin/bash", "-c"]
RUN apt-get update 
RUN apt-get install -y yarn mysql-server python3-pip python3-venv python3-wheel zopfli nano vim
ADD requirements.txt /
RUN python3 -m venv venv 
#ADD venv /
#RUN bash source /Users/acm/aol/yenositu/dev-image/venv/bin/activate && pip3 install -r /requirements.txt && yarn
RUN source /venv/bin/activate && pip3 install -r /requirements.txt && yarn
