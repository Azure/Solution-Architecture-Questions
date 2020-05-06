# Technical Requirements

* Resiliency
    * HA
        * What is each service's SLA?  RPO?  RTO?
    * BC/DR
        * Which regions do you need to deploy to?  Are their Paired Regions?
* Security
    * What are your biggest threat vectors?
    * Do you need Firewall?  Egress/Ingress restrictions?
* Identity
    * B2C
    * B2B
* Data
* AI
* Observability
    * Metrics
        * What resolution/metrics do you need to understand the performance of your app?
    * Logs
        * How are logs collected?  aggregated?
    * Alerts
        * How do you know if the service experiences problems?
* Tenancy
    * Key Concepts:
        * Application based Multi-tenancy
        * Infrastructure based Multi-tenancy
        * Hybrid
    * Questions:
        * How do you onboard a new tenant?
        * Does this support a multi-tenancy control plane? Ingress?
* Scaling
    * Key Concepts:
        * RPS
        * Traffic Patterns
        * App vs Infra Scaling
    * Questions:
        * What's your traffic volume at normal load?  Peak?
        * What is your Y/Y, Q/Q growth?
* Governance
    * Enforcement Policy
    * Audit Policy
* Compliance
    * Key Concepts
        * SOC
        * HIPAA
        * ISO
        * PCI
    * Questions:
        * Do you have any compliance standards
        * What is your data retention policy?
