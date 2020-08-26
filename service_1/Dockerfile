FROM python:3.6-stretch

RUN apt-get update && \
	apt-get install -y gcc make apt-transport-https ca-certificates build-essential

WORKDIR /app

COPY . /app

RUN pip3 --no-cache-dir install -r requirements.txt

EXPOSE 8080

ENTRYPOINT ["python3"]
CMD ["app.py"]
