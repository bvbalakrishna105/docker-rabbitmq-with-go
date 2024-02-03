# docker-rabbitmq-with-go

Pull the RabbitMQ Docker Image:

docker pull rabbitmq

Run RabbitMQ Container:

docker run -d --name my-rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq

Run docker ps to Get Container ID:

docker ps

Run Shell in RabbitMQ Container:

docker exec -it <container_id> /bin/bash

Run rabbitmqctl Commands:

rabbitmqctl list_queues

rabbitmqctl list_parameters

Check Docker Container Status:

docker ps

Check RabbitMQ Service Status Inside the Container:

docker exec -it <container_id> /bin/bash

rabbitmqctl status

First, make sure to install the "streadway/amqp" package:

go get github.com/streadway/amqp



