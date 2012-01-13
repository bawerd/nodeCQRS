# Introduction

The project goal is to provide a tiny sample how to approach (D)DDD, CQRS and EventSourcing 
in node.js. Don't take this as best practice or as starting point for a real implementation:


This sample implementation of CQRS / Eventsourcing is using:

- [redis](http://redis.io/) for Pub/Sub and Storage
- [nodeEventStore](https://github.com/KABA-CCEAC/nodeEventStore) for EventSourcing including it's redis storage implementation.

### get it up and running
        
1.  start server in _host_ and _domain_ folder

        node server.js
        
1.  direct your browser to 

        http://localhost:3000

# Read the annotated code

- [domain](public/docs/domain/server.html) - commandHandling, using nodeEventStore, Publishing.
- [host](public/docs/host/server.html) - webserver, socket.io, eventdenormalizing.
- [clientside](public/docs/client/bootstrap.html). - MVVM, incrementel updates via events