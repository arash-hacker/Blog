
<pre>
  <h1>system design</h1>h1


  •  Load balancer
  ◦  Active-passive
  ◦  Active-active
  ◦  Layer 4 load balancing
  ◦  Layer 7 load balancing
  ◦  Horizontal scaling
Database
  •  Relational database management system (RDBMS)
  ◦  in-memory 
  ◦  Vertical scaling
  ◦  Master-slave replication
  ◦  Master-master replication
  ◦  Federation
  ◦  Sharding
            ⁃  horizontal
            ⁃  vertical
  ◦  Denormalization
  ◦  SQL tuning
  
  •  NoSQL
  ◦  Key-value store
  ◦  Document store
  ◦  Wide column store
  ◦  Graph Databasev
  ◦  non-structure data
  ◦  write/read 

  •  Cache
  ◦  Cache-aside
  ◦  Write-through
  ◦  Read-through
  ◦  Write-behind (write-back)
  ◦  Refresh-ahead


  •  Communication
  ◦  TCP
  ◦  UDP
  ◦  RPC
  ◦  Graphql
  ◦  REST
  ◦  SOAP
  ◦  uwsgi
  ◦  gunicorn
  ◦ ---- Strong type, security, learning curve, bi-directinoal, versionning

  •  Asynchronism
  ◦  Message queues
  ◦  Task queues
  ◦  Back pressure


  •  Stablity pattern
  ◦  timeout
  ◦  rate limiting
  ◦  retries
  ◦  queueing
  ◦  failover
  ◦  bulkheads
  ◦  circuit breakers
  ◦  isolation
  ◦  redundency
  ◦  middleware
  ◦  impodency



Functional  Requirement (tech user-flow)
Non-functional 
  available-
  scale-
  latency-
  throughput-
  CAP-ACID-BASE
opensource - in-house
max throughput-atency 
how much developer need


Database per Service -
Saga 
API Composition 
CQRS 
Domain event -
Event sourcing -


Observablity / Monitoring
High level design 
low level design



-------- architect ---------
Clean architect,
robust,
maintainable, 
testibility, 
resistance, 
availiblity,       
reliability, 
resilience,
clean code, 
cupid, 
solid, 
grasp, 
code smells,       
anti-patters, 
code smells, 
security, 
speed, 
time , 
budget,
future running,
long process, 
------------------------------   
* distributed patterns
    Client-Server Pattern
    Peer-to-Peer (P2P) Pattern
    Master-Slave Pattern
    Publish-Subscribe Pattern
    MapReduce Pattern
    Microservices Pattern
    Layered Pattern (n-tier architecture)
    Service-Oriented Architecture (SOA)    
-----------------------------

Database per Service
Shared database
Saga
API Composition
CQRS (Command Query Responsibility Segregation)
Domain event
Event sourcing 
--------------------------

</pre>
