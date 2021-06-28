# Technical Requirements

* Resiliency
    * HA
        * What is the solution's SLA?
        * Are there any service dependencies that will impact this solution's availability?
        * What HA features are available in the current applications?  (ex. SQL HA)
    * BC/DR
        * What is the RTO/RPO? Is the solution business-critical?
        * Which regions do you need to deploy to?  Are they Paired Regions?
        * Will the DR solution need to meet the same production requirements (ex. same/reduced traffic, lower performance)
        * How do users access the service now, via IP, URL etc..
        * Do you have an existing DR or Incident Recovery Plan? 
        * How do you perform DR testing?

* Security
    * What are your biggest threat vectors?
    * Do you need Firewall?  Egress/Ingress restrictions?
    * Are you subject to any regulatory/organizational mandates or policies?

* Identity
    * Do you need to support identities from identity providers external to Azure Active Directory (eg., Google, Facebook, Active Directory Federation Services)? 
        * Do you need to share your apps and resources with external users? (B2B collaboration)
        * Do you need to build user journeys with a white-label identity management solution for consumer- and customer-facing apps (B2C collaboration)
        * Refer to the 'Compare External Identities solutions table for more decisions points (https://docs.microsoft.com/en-us/azure/active-directory/external-identities/compare-with-b2c)
    * What are you currently using to authenticate your users?
    * What are you currently using to authorize user/group/service access to your services?

* Data
    * Do you have retention policy? How is data backed up? 
    * Are their policies impacting how the data is shared? 
    * How much data does the solution generate? How much data do you intake daily? 
    * Is your data segregated by customer? How do they access the data? 
    * What kind of data is being stored? What is it used for? 

* AI
    * What level of AI is of interest? (Bots, Cognitive Service API, Data Scientist platforms, Machine Learning models)
    * What skill sets do you have on staff? (Data scientists, Developers)
    * What data sets do you have to leverage? (public/proprietary)
    * What feature/functionality are you supporting with the AI? 

* Observability
    * Questions: What existing solutions are you using?  Provided internally, by another provider? 
    * Metrics
        * What resolution/metrics do you need to understand the performance of your app/understand if you are meeting SLA?
        * What is needed at the network level, platform level, application level, user experience level? 
    * Logs
        * How are logs collected?  aggregated? 
    * Alerts
        * How do you know if the service experiences problems?
        * Who will be receiving the alerts?
    * Tenancy
        * Key Concepts:
            * Application based Multi-tenancy
            * Infrastructure based Multi-tenancy
            * Hybrid
    * Questions:
        * How do you onboard a new tenant?
        * Does this support a multi-tenancy control plane? Ingress?
        * What is the tenancy model of the solution? Is there a shared front end but seperate back-end/database per customer? 
        * How is the tenancy implemented in the database? Seperate tables, schema, databases on the same server, independent servers?
        * What is the tenancy model of supporting services like storage, CDN, VMs?

* Scaling
    * Key Concepts:
        * RPS
        * Traffic Patterns
        * App vs Infra Scaling
    * Questions:
        * What's your traffic volume at normal load?  Peak?
        * What is the bottleneck that causes you to scale? (e.g. Memory, CPU, bandwidth)
        * Are there any leading indicators to help you scale?
        * Do you have scalability/performance requirements? Ex. Number of users, transactions per second, Number of SQL statements running simultaneously
        * What is your Y/Y, Q/Q growth? Are there upcoming events that you anticipate growth/traffic spikes for? 
        * Is your application written with microservices or as a monolith? Can the components be deployed as seperate services? 
        * Are there closely coupled systems that must also scale or will be impacted when the solution scales up?

* Governance
    * What is currently in place for governance? Who controls environment access? 
    * Who dictates the enforcement policy and how is it enacted?
    * Who dictates the audit policy and how is it enacted?

* DevOps
   * What environments do you have? (e.g. Dev/Test/Prod)
   * How are you creating new software artifacts?
   * How do you deploy the new software artifacts across your environments?

* Compliance
   * Key Concepts
        * SOC, HIPAA, ISO, PCI
    * Questions:
        * Are you subject to security audits?
        * Do you have any compliance requirements?
        * How do you currently track compliance? Who is responsible for system compliance? 
