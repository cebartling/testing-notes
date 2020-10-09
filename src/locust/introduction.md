# Introduction

Locust is an easy to use, scriptable and scalable performance testing tool. You define the behavior of your users in regular Python code, instead of using a clunky UI or domain specific language. This makes Locust infinitely expandable and very developer friendly.

- [Locust website](https://locust.io)
- [Locust documentation](https://docs.locust.io/en/stable/index.html)

## Features

### Write user test scenarios in plain-old Python

If you want your users to loop, perform some conditional behaviour or do some calculations, you just use the regular programming constructs provided by Python. Locust runs every user inside its own greenlet (a lightweight process/coroutine). This enables you to write your tests like normal (blocking) Python code instead of having to use callbacks or some other mechanism. Because your scenarios are “just python” you can use your regular IDE, and version control your tests as regular code (as opposed to some other tools that use XML or binary formats)

### Distributed and scalable

Locust makes it easy to run load tests distributed over multiple machines. It is event-based (using gevent), which makes it possible for a single process to handle many thousands concurrent users. While there may be other tools that are capable of doing more requests per second on a given hardware, the low overhead of each Locust user makes it very suitable for testing highly concurrent workloads.

### Web-based UI

Locust has a user friendly web interface that shows the progress of your test in real-time. You can even change the load while the test is running. It can also be run without the UI, making it easy to use for CI/CD testing.

### Can test any system

Even though Locust primarily works with web sites/services, it can be used to test almost any system or protocol. Just write a client for what you want to test, or explore some created by the community.

### Hackable

Locust is small and very flexible and we intend to keep it that way. If you want to send reporting data to that database & graphing system you like, wrap calls to a REST API to handle the particulars of your system or run a totally custom load pattern, there is nothing stopping you!

