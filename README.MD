## Enable Rabbitmqadmin Cli

Not every project can manage via web browser, cli is more suitable for most projects.

```
docker run -d --name=my-rabbit managable-rabbitmq:latest
```
This will give you a container where cli is available.

```
docker exec -it my-rabbit bash
// this will list current exchanges.
$rabbitmqadmin list exchange
