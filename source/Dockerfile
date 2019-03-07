FROM alpine

# basic flask environment
RUN apk add --no-cache bash uwsgi uwsgi-python py2-pip \
	&& pip2 install --upgrade pip \
	&& pip2 install flask

COPY . /app
WORKDIR /app

RUN pip install -r requirements.txt

EXPOSE 5000
ENTRYPOINT ["python"]
CMD ["runserver.py"]
