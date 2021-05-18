# Azure Batch

## Concepts

Be familiar with the following [Azure Batch concepts](https://docs.microsoft.com/en-us/azure/batch/batch-service-workflow-features):

* Batch Account
* Application
* Pool
* Job
* Task

## Questions

* What are the [Batch SKU](https://docs.microsoft.com/en-us/azure/batch/batch-pool-vm-sizes)'s your tasks require?
* Will is the [pool allocation mode](https://docs.microsoft.com/en-us/azure/batch/accounts#batch-accounts)? (e.g. User Subscription or Batch Service)
* How often and how many jobs do you expect to run?
* How many tasks can run on a single node?
* How many tasks do you expect to run?
* When should a job start?
* When should a task start?
* When should a task complete?
* How long do you expect each task to run?
* What are the input/output of each task?
* What are the OS requirements? (e.g. Ubuntu 18.04, Windows Server 2019)
* Do you need to create a custom image for the OS?
* How is the application packaged?
* What language do you plan to use for the Batch SDK? (e.g. .NET Core, Python)
* Do you need autoscaling?  If so, what is the scale up and down trigger?
