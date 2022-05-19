# IPaaS: ITIS Paleocapa as a Service

IPaaS is a hosting service for the [ITIS Paleocapa](https://www.itispaleocapa.edu.it/) and it will let the students host their web-base application on the school servers.

## WBS
```mermaid
graph LR
  1.0[1.0 IPAAS] --> |1.1|1.1[planning]
  1.1 --> |1.1.1|1.1.1[choosing technologies]
  1.1 --> |1.1.2|1.1.2[checking compatibility of technologies]
  1.0 --> |1.2|1.2[configurations]
  1.2 --> |1.2.1|1.2.1[setting up servers and OS]
  1.2 --> |1.2.2|1.2.2[updating servers]
  1.2 --> |1.2.3|1.2.3[fixing problems]
  1.2 --> |1.2.4|1.2.4[configuring third party services]
  1.0 --> |1.3|1.3[testing development]
  1.3 --> |1.3.1|1.3.1[setting testing environment]
  1.3 --> |1.3.2|1.3.2[creating database and tables]
  1.3 --> |1.3.3|1.3.3[coding testing version of backend]
  1.3 --> |1.3.4|1.3.4[coding testing version of frontend]
  1.0 --> |1.4|1.4[production development]
  1.4 --> |1.4.1|1.4.1[coding endpoints]
  1.4 --> |1.4.2|1.4.2[connecting functions to endpoints]
  1.4 --> |1.4.3|1.4.3[linking backend to frontend]
  1.4 --> |1.4.4|1.4.4[setting service on the school servers]
  1.0 --> |1.5|1.5[testing alpha and beta]
  1.5 --> |1.5.1|1.5.1[unit testing and alpha version]
  1.5 --> |1.5.2|1.5.2[releasing beta]
  1.5 --> |1.5.3|1.5.3[testing beta in closed environment]
  1.0 --> |1.6|1.6[deploying release]
  1.6 --> |1.6.1|1.6.1[make release public]
```