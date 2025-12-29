## What is AWS?

**AWS (Amazon Web Services)** is the world’s most widely adopted **cloud platform**, offering over **200 fully featured services** from data centers all around the world.
## The Shared Responsibility Model

This model explains **who is responsible for what** in terms of **security and compliance** when using AWS.

Think of it like renting an apartment:
- The building owner (AWS) is responsible for the structure and safety of the building.
- The tenant (you/your company) is responsible for what happens inside your apartment.

![[AWS_SecurityModel.png]]

## AWS Global Infraestrucute

The AWS Cloud spans 120 Availability Zones within 38 Geographic Regions, with announced plans for 10 more Availability Zones and 3 more AWS Regions in the Kingdom of Saudi Arabia, Chile, and the AWS European Sovereign Cloud.

### Regions 

AWS has the concept of a Region, which is a physical location around the world where we cluster data centers. We call each group of logical data centers an Availability Zone. Each AWS Region consists of a minimum of three, isolated, and physically separate AZs within a geographic area

### Availability Zones

An Availability Zone (AZ) is one or more discrete data centers with redundant power, networking, and connectivity in an AWS Region. AZs give customers the ability to operate production applications and databases that are more highly available, fault tolerant, and scalable than would be possible from a single data center. All AZs in an AWS Region are interconnected with high-bandwidth, low-latency networking, over fully redundant, dedicated metro fiber providing high-throughput, low-latency networking between AZs.

## Service Administration Levels

In AWS, services fall into three categories depending on how much administration **YOU** must perform versus how much AWS manages for you:

![[AWS_ServicesModel.png]]