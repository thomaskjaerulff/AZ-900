# SLA and Composite SLA in Azure

## SLA
**Service Level Agreement** (SLA) is a formal agreement between a service provider and a customer.

**SLA is a promise** of a service’s **availability** (uptime & connectivity). **Availability** is a measure of time that a service remains operational.

- Each Service has its own SLA
- Ranges from 99% to 99.999%
- Free services typically don’t have an SLA
- Broken SLA means service credit return (discount)

|SLA|Monthly Downtime|
|---|----------------|
|99%|7h 18m 17s|
|99.5%|3h 39m 8s|
|99.9%|43m 49s|
|99.95%|21m 54s|
|99.99%|4m 22s|
|99.999%|26s|

## Formulas
### Logical AND - adding dependency
Availability of S1 AND S2 = Availability(S1) * Availability(S2)

### Scenario - Azure website with SQL backend db
- Availability = Availability(web) app * Availability(sql)
- Availability = 99.95% * 99.95%
- Availability = 0.9995 * 0.9995
- Availability = 0.99900025
- Availability ~ 99.9%

### Logical OR - adding redundancy
Availability of S1 OR S2 = 100% - ( Unvailability(S1) * Unvailability(S2) )

### Scenario - Two redundant web apps behind a load balancer
- Availability(both-web) = 100% - ( Unvailability(web1) * Unvailability(web2) )
- Availability(both-web) = 100% - ( 0.05% * 0.05% )
- Availability(both-web) = 1 – ( 0.0005 * 0.0005 )
- Availability(both-web) = 1 – 0.00000025
- Availability(both-web) = 0.99999975
- Availability(both-web) ~ 99.9999%

## Key Items
- **Formal agreement** between **Microsoft** & the **customer**
- Calculated as a **percentage of service availability** (**uptime** & **connetivity**) (a promise)
- Breaking the SLA provides a discount from the final monthly bill (**Service Credit**)
- **Higher tier** services offer better **SLAs**
- **Free** services typically have **no SLA** (0% SLA)
- **Preview** services have **no SLA**
- **Composite SLA** is a combined SLA of all application components