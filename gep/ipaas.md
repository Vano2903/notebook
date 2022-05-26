
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

## PDM

```mermaid
graph LR
	A[1: creating DB] --> B[2: connecting backend to DB]
	B --> C[3: development of main functions in the backend]
	C --> D[4: development of frontend]
	D --> E[5: setting up school servers]
	E --> F[6: testing]
	F --> G[7: hosting application]
	G --> H[8: releasing]
```

## GANTT

```mermaid
gantt
    title IPaaS
    dateFormat  DD-MM-YYYY
    section setting servers
    Hardware cleaning :done a1, 06-02-2022, 1d
    Starting server : 07-02-2022  , 1d
    Configuring machine :a2, 07-02-2022  , 1d
    section docker functions
    Coding db docker functions: a3, after a2, 7d
    Coding github functions: a4, after a3, 14d
    section backend functions
    Coding endpoints: a5, after a4, 3d
    Coding handlers: a6, after a4, 7d
    section fronend
    Coding frontend: a7, after a6, 1d
    section deploying
    Deploy on servers: a8, after a7, 1d
```
## OBS

```mermaid
graph TD
	PM --> System-Engineer
	PM --> Developers
	Developers --> Backend-Developers
	Developers --> Frontend-Developers
	PM --> Testers
```

## RACI
A = approve the work
R = person in charge
C = person that collaborates
I = informed of the work done
| activity | PM | system engineer | be dev | fe dev | tester |
|--|--|--|--|--|--|
| configuring servers | A | R | I | I |  |
| setting testing environment | A | I | R | I | C |
| creating db | A | C | R | I | I |
| coding backend | A |  | R | I |  |
| coding frontend | A |  | I | R | C |
| unit testing | A | I | R | C | C |
| testing beta | A/C |  | C | C | R |
| deploying release | A | R | C | I | I |
| make release public | A/R | C | C | C | C |
