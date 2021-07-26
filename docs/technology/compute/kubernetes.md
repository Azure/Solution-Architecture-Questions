# Kubernetes

* Does the application already run in a containerized environment?
* Is this a new K8S cluster or a migration from an existing K8S cluster?
* Do you plan to use AKS or CAPI/CAPZ?
* What are the ingress network requirements?
* What are the egress network requirements?
* Does the application persist state inside the container?  If so, how?
* What are the scaling requirements?
* What are your build and deploy pipelines and how are they implemented?
* What languages are used? (e.g. C#, PHP, Python)
* How do you know if the application is healthy?
* What type of runtime resources does the container require?  (e.g. memory, CPU)
* What version of Kubernetes are you planning to use?

## Resources

* [The Twelve-Factor App](https://12factor.net/)
* [Container Security in Microsoft](https://azure.microsoft.com/mediahandler/files/resourcefiles/container-security-in-microsoft-azure/Open%20Container%20Security%20in%20Microsoft%20Azure.pdf)
* [Building Microservices by Sam Newman](http://shop.oreilly.com/product/0636920033158.do)
* [Production Ready Microservices by Susan Fowler](http://shop.oreilly.com/product/0636920053675.do)
* [Designing Distributed Systems](http://shop.oreilly.com/product/0636920072768.do)
* [GitOps](https://www.weave.works/blog/gitops-operations-by-pull-request)
* [Azure AKS Best Practices](https://www.cncf.io/webinars/optimize-your-kubernetes-clusters-on-azure-with-built-in-best-practices/)

## Tools
* [Polaris](https://www.fairwinds.com/polaris)
* [kube-scan](https://github.com/octarinesec/kube-scan)
* [Azure Advisor](https://azure.microsoft.com/en-us/updates/azure-advisor-integration-with-aks-now-generally-available/)
* [Open Policy Agent](https://www.openpolicyagent.org/docs/latest/kubernetes-introduction/)
* [Weave Scope](https://www.weave.works/oss/scope/)
* [Periscope](https://github.com/Azure/aks-periscope)
