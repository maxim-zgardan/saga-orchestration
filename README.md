SAGA Orchestration design pattern for distributed transaction means the tasks are invoked by another parent task. It plays the role of an
orchestrator.
It calls each tasks in sequence and based on their response decides whether to call the next task
or the compensating tasks.

To make orders:
POST http://localhost:8080/order/create
Content-Type: application/json

{"productId": 2,
"userId": 1
}

To retrieve orders:
GET http://localhost:8080/order/all
Content-Type: application/json
