# Software Architecture

* Infrastructure
    * Networking
        * Key Concepts:
            * ExpressRoute, VPN, Firewall
        * Questions:
            * Is the system allowed to reach to external services?
            * Will external services (or users) reach to the system?
            * Any ingress/egress rules?
            * Any on-premesis requirements?
    * Compute
        * Key Concepts:
            * VM, VMSS, Azure Functions, Batch
        * Questions:
            * Will the system run in containers?
            * Is the system CPU or memory intensive? (or both?)
            * How are you bundling the system?
            * How will your application scale?
            * How do you know when to scale?
            * What parts of the system are syncronous?  
            * What parts of the system are asyncronous?
    * Storage
        * Key Concepts:
            * Blob, NFS, SMB
        * Questions:
            * Does the system need to persist data outside a database?
            * What format is the data in?  (e.g. local files, blob)
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
        * If applicable, do you plan to use Azure 1st party services?
* Platform
    * OS
        * Key Concepts
            * Linux Distros, Windows Server
        * Questions:
            * How do want to manage updates when there's a critical security update?
    * Runtime
        * Key Concepts
            * Container, Kubernetes
        * Questions:
            * How do you plan to build your runtime image?
    * App Platform/Development Framework
        * Key Concepts
            * 12 Factor App
        * Questions:
            * What language/framework do you use?
            * Do you follow 12 Factor Apps model?
* Technical Roadmap
    * Is this a greenfield or brownfield app?
    * What optimizations do you foresee?
    * What is your highest technical priorities?
