FROM ubuntu:18.04
ENTRYPOINT []
RUN apt-get update && apt-get install -y python3 python3-pip && python3 -m pip install --no-cache --upgrade pip 
RUN pip3 install --no-cache rasa-sdk==1.10.2
ADD . /app/actions
RUN chmod +x /app/actions/action_server.sh
CMD /app/actions/action_server.sh