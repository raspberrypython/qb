# qb
qb (pronounced "*cube*") is a cross-platform toolkit for **system containers** inspired by the **application container** stack by Docker.

### Why not Docker?
```docker``` is great, we love it, but it's not suitable for everything. Docker is an **application container** technology, meaning it's intended to wrap a single process such as Apache, Nginx or MySQL. However, not everyone is in the position to adopt a micro-service infrastructure. Perhaps you have legacy systems to support, maybe you rely on other services a full system would provide such as systemd, cron or syslog. In these cases you either simply can't use Docker at all, or you have to hack it to work in a way in which it was never intended to be used, which can cause buggy behaviour.

```qb``` provides Docker-like functionality but is different in that it utilises **system containers**, meaning you don't need to choose a single process to wrap, the container boots all of the services you'd expect from a regular Linux distribution.

### Tools
#### qb client
The qb command-line client is a tool to manage all of the components listed below. It's designed to be intuitive, user-friendly and inherits a lot from the design decisions Docker have implemented in their hugely successful production-ready container infrastructure stack.

#### qb machine
A qb machine is a very minimal, light-weight Linux virtual Machine (VM) created to provide a consistent base environment on which as few or as many qb containers can be run as you wish, and that's it.
The primary use of qb machine is to allow users to run qb containers on their local machines regardless of operating system or configuration. It provides two core dependencies, the Linux kernel, and the LXD API which the qb client calls to manage containers.

#### qb container
TODO

#### qb registry
TODO

#### qb network
TODO

#### qb compose
TODO

### Installation
TODO

### Usage
TODO
```bash
qb --help
```

### Contribute
As always, we welcome **pull requests** with open arms. Hack away!
