FROM python:3.12-bullseye

RUN pip install --no-cache-dir \
    pyserial \
    paho-mqtt==1.6.1 \
    construct

ADD pylon_to_mqtt.py /
ADD support/*.py support/

ENTRYPOINT ["python3", "pylon_to_mqtt.py"]
