# Parallel processing using work queue

In this example a kubernetes job runs multiple parallel worker processes in a given pod. 

Each worker consumes params from the work queue.

An instance of Redis is used as the work queue.

As stated in the example webpage:

> In this example, we use Redis to store our work items. In the previous example, we used RabbitMQ.
> This example uses Redis and a custom work-queue client library because AMQP does not provide
> a good way for clients to detect when a finite-length work queue is empty. In practice you would
> set up a store such as Redis once and reuse it for the work queues of many jobs, and other things.

## Reference

This is the original webpage where this example was copied from.

https://kubernetes.io/docs/tasks/job/fine-parallel-processing-work-queue/
