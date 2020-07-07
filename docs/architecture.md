# Software Architecture

* Infrastructure
    * Networking
        * Key Concepts:
            * ExpressRoute, VPN, Firewall
        * Questions:
            * Does the system reach to external services?
            * How do users interact with the system?
            * Is access to the system public or locked down?
                * If locked down, how so?
            * Any on-prem requirements?
    * Compute
        * Key Concepts:
            * VM, VMSS, Azure Functions, Batch
        * Questions:
            * Will the system run in containers?
            * Is the system CPU or memory intensive? (or both?)
            * How do you bundle the system?
            * How do you know when to scale?
            * What needs to happen for the system to scale? (e.g. more VM's)
    * Storage
        * Key Concepts:
            * Blob, NFS, SMB
        * Discovery Questions:
            * Does the system need to persist data outside a database?
            * What format is the data in?  (e.g. local files, blob)
            * What size is the data?
        * Technology: 
            * [Data Lake](docs/technology/storage/azure-data-lake.md)
            * Blob
            * NFS
    * IoT
        * Key Concepts:
            * IoT Hub, IoT Central
        * Questions:
            * How are the IoT devices deployed?
            * How are the IoT devices maintained and upgraded?
            * What central repository are the IoT devices reporting to?
            * Do you use Digital Twins?
* Third-party Integrations
    * Questions
        * What 3rd party systems does your system integreate with? (e.g. SMTP, Database)
        * How do you plan to manage these 3rd party systems?
        * What Microsoft/Azure SaaS offerings do you plan to use? (e.g. Cognitive Services, etc.) 
* Platform
    * OS
        * Key Concepts
            * Linux Distros, Windows Server
        * Questions:
            * What OS can the system run on?
            * How do plan to manage updates when there's a critical security update?
    * Runtime
        * Key Concepts
            * Container, Kubernetes
        * Questions:
            * What is your build system?
            * How often do you build new executable artifacts?
            * How often do you deploy new executable artifacts?
    * App Platform/Development Framework
        * Key Concepts
            * C#, Python, NodeJS, 12 Factor App
        * Questions:
            * What language/framework is the system written in?
            * Does the system follow the 12 Factor Apps model?
* Technical Roadmap
    * Is this a greenfield or brownfield app?
    * What optimizations do you foresee?
    * What are your highest technical priorities?
