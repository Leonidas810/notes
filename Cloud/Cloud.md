## What is Cloud Computing?

Cloud computing is the **delivery of computing services** - such as **servers, storage, databases, networking, software, analytics, and intelligence - over the internet** (**"The cloud"**) instead of relying on local computer or physical servers.

Key Characteristics of Cloud Computing

1. On-demand self-service
	- Users can access resources whenever they need them, without human interaction from the provider.
		-> Example: Creating a virtual machine in seconds through a dashboard
2. Broad network access
	- Resources are avalaible over the internet and accessible from any device (PC, tablet, smathphone).
3. Resource pooling
	- The provider's resources are shared among many users using a multi-tenant model.
		->Think of it as an apartment building: many people share the same infrastructure
4. Rapid elasticity
	- Resources can scale up or down quickly based on demand
		-> Example: A website automatically scales during Black Friday 
5. Measured service (Pay-as-you-go)
	- You pay only for the resources you use (like electricity or water)

## Cloud Deployment Models

A **cloud deployment model** defines where the cloud infrastructure is located, who controls it, and **how it's managed**

There are three main types 

|                  | Public Cloud                                                                                                            | Private Cloud                                                                                                                                        | Hybrid Cloud                                                                                                                                                                                         |
| ---------------- | ----------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Definition       | A cloud environment owned and operated by a **third-party provider**, delivering services over the public internet      | A cloud infraestructure used exclusively by one organization. It can be located **on-premises** (in your own data center) or hosted by a third party | A combination of public and private cloud, allowing data and applications to move between them.                                                                                                      |
| Examples         | Amazon Web Services (AWS), Microsoft Azure, Google Cloud Plataform (GCP)                                                |                                                                                                                                                      |                                                                                                                                                                                                      |
| Characteristics: | Shared resources between multiple customers. / No need to buy or manage hardware. / Highly scalable and cost-efficient. | Complete control over data, security, and compliance / Customizable infrastructure / Higher cost, since hardware and maintenance are not shared      | Flexibility to run sensitive data in a private cloud and less-sensitive workloads in a public cloud. / Balances cost efficiency with security. / Enables backup, disaster recovery, and scalability. |
| Best for         | Startups, small businesses, or organizations that need flexibility and cost efficiency.                                 | Large enterprises, banks, or government institutions that require **strict data control** and **security**.                                          | Organizations needing both **control** and **agility**, such as hospitals or educational institutions.                                                                                               |
