# ChallengeCrf
## Challenge project put forward for testing.

The project proposes to make a rough study of market standards and mechanisms used in capital market solutions, such as mesageria and data specification libraries for the transport layer such as protobuf.

Architecture - Message/Event Driven and some elements of Clean Architecture.

Command-> Event

Query-> Reply

Using RabbiMQ Queues to choreograph the environment.

Protobuf for compression in the transport layer.

SignalR does not respond to the client/Angular.

Creational Patterns used:

Factory

Singleton

Behavioral Patterns

Command

Mediator 

## More

Ioc - Inversion of control

CQRS - with Choreography

dependency injection

Unit of Work

Event Sourcing (removed)

Some solid concepts were also used.


## Instructions for running

From within the ChallengeCrf project folder run:

```kind create cluster```

```kubectl apply -f k8s-configs/```

```kubectl get pods```

```kubectl get services```

```kubectl get deployments```

```kubectl get pvc```


If a pod is not working, for example 'angular-service'

```kubectl describe pod angular-service```

```kubectl logs angular-service```


Up Containers of:

rabbitmq-server - RabbitMQ

mongo - MongoDB

challengecrf.api - Request API for Release Control and daily consolidated

challengecrf.queue - Worker for Producer and consumer for the service 

angularcontainer - Angular Front End to register. http://localhost:4200/cashflow

## C4 architecture model

[![image](https://github.com/bvarandas/ChallengeCrf/assets/13907905/76c11216-d9b7-4d2a-bee2-ec5f4855334b)]

![image](https://github.com/bvarandas/ChallengeCrf/assets/13907905/43b306e1-df1d-443a-8199-dbeefc4915e8)

![image](https://github.com/bvarandas/ChallengeCrf/assets/13907905/6a10558d-eb43-4842-acba-58ea77442767)

