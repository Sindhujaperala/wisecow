FROM debian:bullseye-slim

WORKDIR /app

RUN apt-get update && apt-get install -y cowsay fortune && rm -rf /var/lib/apt/lists/*

COPY wisecow.sh ./server.sh

RUN chmod +x ./server.sh

EXPOSE 4499

CMD ["./server.sh"]
