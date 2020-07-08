# Kubernetes

* Are the applications already in containers?
* Is this a new K8S cluster or a migration from an existing K8S cluster?
* Do you plan to use AKS or AKS-engine?
* Do you plan to use Ingress?
* Does the application persist state?  If so, how?
* What ports are exposed externally?
* What ports are exposed internally?
* Do you plan to implement manual or auto-scaling?
* What base container image do you use?
* How do you deploy your containers?
* What languages are used? (e.g. C#, PHP, Python)
* Are you using readiness and health probes?
* Do you have resource quotas set?
* Are you usising "latest" image tags? (HINT: You shouldn't be)
* Do you restrict the registries where iamges come from?
* What version of Kubernetes are you using?
* 

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
