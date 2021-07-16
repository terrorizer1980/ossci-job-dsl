FROM ubuntu:xenial-20210114

RUN apt-get update && apt-get install -y python-pip

ADD requirements.txt /requirements.txt

RUN pip install -r /requirements.txt

ADD gc.py /usr/bin/gc.py

ENTRYPOINT ["/usr/bin/gc.py"]
