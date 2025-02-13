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
occur synchronously (i.e. at the same time). This definitions sounds basically
like the same thing as concurrency, but they are quite different, and we'll
soon see why.

Asynchronous code is extremely common in web development. It allows the client
(i.e. user) to send a request to a server without the whole webpage freezing up
while waiting for a response from the server. Needless to say, synchronous code
running on websites would be a pretty terrible user experience.

Like Python, JavaScript/TypeScript is single-threaded. Only one thing can happen at a time. 

### A Helpful Analogy

### Real-World Examples

```typescript
const a = fetch()
```

```python
a: int = 5
```

## Concurrent Code

### Another Helpful Analogy

### A Real-World Example
