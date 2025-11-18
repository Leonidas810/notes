## In simple terms:

EC2 = Virtual Servers in the cloud that you can configure, scale, secure, and pay only for what you use.

EC2 gives you full control of the compute environment - like choosing CPU, memory, storage, OS, and networking.
## What is [EC2](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/concepts.html) ? 

Amazon Elastic Compute Cloud (Amazon EC2) provides on-demand, scalable computing capacity in the Amazon Web Services (AWS) Cloud. Using Amazon EC2 reduces hardware costs so you can develop and deploy applications faster. You can use Amazon EC2 to launch as many or as few virtual servers as you need, configure security and networking, and manage storage. You can add capacity (scale up) to handle compute-heavy tasks, such as monthly or yearly processes, or spikes in website traffic. When usage decreases, you can reduce capacity (scale down) again.

An EC2 instance is a virtual server in the AWS Cloud. When you launch an EC2 instance, the instance type that you specify determines the hardware available to your instance. Each instance type offers a different balance of compute, memory, network, and storage resources. For more information, see the [Amazon EC2 Instance Types Guide](https://docs.aws.amazon.com/ec2/latest/instancetypes/instance-types.html).

![[EC2_Types.png]]

## Amazon EC2 instance types

When you launch an EC2 instance, the instance type that you specify determines the hardware of the host computer used for your instance.
Each instance type offer different compute, memory and storage capabilities, and is grouped in an instance family based on these capabilities, and is grouped in an instance family based on these capabilities

1. General purpose Amazon EC2
	- Make everyday workloads easier with a balanced instance
2. Compute optimized Amazon EC2
	- Get the right processing power for CPU-intensive workloads
3. Memory optimized Amazon EC2
	- Process massive data sets fast
4. Accelerated computing Amazon EC2
	- Boost function operations with faster hardware
5. Storage optimized Amazon EC2
	- Access data on local storage at high speeds
6. HPC optimized Amazon EC2
	- Speed up complex workloads using high-performance processors
### General purpose Amazon EC2
General purpose instances provide a balance of compute, memory and networking resources, and can be used for many workloads. These instances are good for applications such as web servers, code repositories, and small-to-medium databases.

### Compute optimized Amazon EC2

Compute optimized instances are ideal for compute bound applications that benefit from **high-performance processors**. Some examples of workloads for compute instances are batch processing, media transcoding, and dedicated game servers.

### Memory optimized Amazon EC2

Memory optimized instances are designed to deliver fast performance for workloads that process large data sets in memory. For example, these instances are good for in- memory databases, data analytics, and enterprise applications.

### Accelerated computing Amazon EC2

Accelerated computing instances use **hardware accelerators, or co-processors, to perform functions more efficiently**. For example, they can perform floating point number calculations, graphics processing, or data pattern matching.

### Storage optimized Amazon EC2

Storage optimized instances deliver millions of low-latency, random I/O operations per second to applications. They’re designed for workloads that require high, sequential read and write access to very large data sets on local storage. For example, they’re good for high-throughput databases, data processing, and data streaming.

### HPC optimized Amazon EC2

High-performance computing (HPC) instances offer the best price performance for running HPC workloads at scale. HPC instances are ideal for applications that benefit from high-performance processors such as complex simulations, deep learning, and visual effects rendering.