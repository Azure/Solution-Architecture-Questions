# Software Architecture

* Infrastructure
    * Networking
        * Key Concepts:
            * ExpressRoute, VPN, Firewall
        * Questions:
            * What external services does the system connect to? (e.g. On-Prem DB, other cloud, etc.)
            * How do users interact and connect with the system? (e.g. User will VPN in and access web console)
            * Is access to the system public or locked down?
                * If locked down, how so? (e.g. VPN + AAD)
            * What are the on-prem requirements? (e.g. 1G u/d connection on-prem DC)

    * Compute
        * Key Concepts:
            * VM, VMSS, Azure Functions, Batch, Kubernetes
        * Questions:
            * Will the system run in containers and/or Kubernetes?
            * What are the application bottlenecks? (e.g. CPU, Memory, etc.)
            * What are the solution's scaling requirements? (e.g. Scale up specific microservice as part of "follow-the-sun" model)
            * What should trigger a scaling event? (e.g. CPU hits 70%)

    * Storage
        * Key Concepts:
            * Blob, NFS, SMB, Data Lake
        * Discovery Questions:
            * How does the system persist data? (e.g. user data is stored in MySQL, media files stored in blob)
            * What format is the data in?  (e.g. images, 1000's of media files)
            * What are the data volume requirements (e.g. 1GB of MySQL data, 1TB of blob storage)

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
        * What 3rd party systems does your system integreate with? (e.g. SMTP, MongoDB)
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
