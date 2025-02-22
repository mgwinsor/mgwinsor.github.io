---
date: 2025-02-13T20:11:19+08:00
# description: ""
# image: ""
lastmod: 2025-02-13
showTableOfContents: false
# tags: ["",]
title: "Async vs. Concurrency: Explained"
type: "post"
draft: true
---

Recently, I have been exploring Go and ~~JavaScript~~ TypeScript. Coming from
the Python world, concurrent or asynchronous code was a completely foreign
concept. Sure, there are the
[asyncio](https://docs.python.org/3/library/asyncio.html) and
[multiprocessing](https://docs.python.org/3/library/multiprocessing.html)
packages in the standard library, but I never had a good reason to actually use
them. Working in the data space with Python typically means that I never need to
worry about any of these concepts. They are just magically handled by a library
(e.g. Pandas, Polars, etc.). Even when I explored building web APIs in Python,
pretty much any modern web backend library handles async or concurrency in some
form. It's just abstracted away. So what is asynchronous code? What is
concurrent code? Are they actually meaningfully different?

## Asynchronous Code

To state the obvious, asynchronous simply means that events or processes do not
occur synchronously (i.e. at the same time). This definition sounds quite
similar to concurrency, but they are quite different, and we'll soon see why.

Asynchronous code is extremely common in web development. It allows the client
(i.e. user) to send a request to a server without the whole webpage freezing up
while waiting for a response from the server. Needless to say, synchronous code
running on websites would be a pretty terrible user experience.

Like Python, JavaScript/TypeScript is single-threaded. Only one thing can happen at a time. 

### A Helpful Analogy

Let's imagine a real-world example of asynchronaity. As you go about your daily
life, there are services that you require from other people. These services can
be interacted with either syncrhonously (e.g. going to the store yourself), or
asynchronously (placing an order/request over the phone or online and receiving
the service/item when you are available). So every time that you place an order
on Grab Food or Uber Eats, for example, you just need to send the request and
you are free to do whatever else you need to do. The food can be dropped at
your door and you pick it up when you are available. So asynchronaity helps you
to leverage your time. You can still only do one thing, but you rely on the
services of others to help you do more.

TODO: involve terms like event loop, etc.

Concurrency, on the other hand, is a bit different. Instead of needing to rely
on other services, you can alternatively build up a team of people to work
together. You control what each person does. Obviously, this is more powerful,
but you also have more complexity since you now need to figure out how to
organize these people to work and communicate together effectively. If done
poorly, you might have just been better of interacting with another service.
But if it is something very custom that you need to control, this is an
excellent way to Go (no pun intended).

### Code Examples

With these concepts 

```typescript
const a = fetch()
```

```python
a: int = 5
```

## Concurrent Code

### Another Helpful Analogy

### A Real-World Example
