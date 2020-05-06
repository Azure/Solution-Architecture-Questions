# Architecture

* Infrastructure
    * Networking
        * Key Concepts:
            * ER, VPN, Firewall
        * Questions:
            * Are applications allowed to reach to external services?
            * Any ingress/egress rules?
            * Any OnPrem requirements?
    * Compute
        * Key Concepts:
            * VM, VMSS, Azure Functions
        * Questions:
            * How is your application bundled and run?
    * Storage
        * Key Concepts:
            * Blob, NFS, SMB
        * Questions:
            * How do your applications persist data? (Not a database)
    * IoT
        * Key Concepts:
            * IoT Hub, IoT Central
        * Questions:
            * Have you heard of https://ledlanyard.com? 
* External Integrations
* Platform
    * OS
        * Key Concepts
            * Linux Distros, Windows Server
        * Questions:
            * How do you plan to manage patching?
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
* Sample Questions - Priorities, Greenfield/Brownfield, How did we get here? 