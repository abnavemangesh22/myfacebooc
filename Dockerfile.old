FROM ubuntu
RUN mkdir /app
WORKDIR /app
COPY . .
RUN apt-get update &&  apt-get install -yq build-essential make libsqlite3-dev sqlite3
RUN make all
EXPOSE 16000
CMD ["bin/facebooc"]
