#AMAZON #EC2

Different ways of paying for Amazon EC2
### On-Demand Pricing

On-Demand Instances let you pay for compute capacity by the hour or second (minimum of 60 seconds) with no long-term commitments. This frees you from the costs and complexities of planning, purchasing and maintaining hardaware and transforms what are commonly large fixed costs into much smaller variable costs.

### Saving plans Pricing

Saving plans are a flexible pricing model that offer low prices on Amazon EC2, AWS Lambda, and AWS Fargate usage, in exchange for a commitment to a consistent amount of usage (measured in $/hour) for a 1 or 3 year term. When you sign up for a Savings Plan, you will be charged the discounted Savings Plans price for your usage up to your usage up to your commitment. AWS offer two types of Savings Plans:

- **Compute Savings Plans**
	Compute Savings Plans provide the most flexibility and help to reduce your costs by up to 66%. These plans automatically apply to EC2 instance usage regardless of instance family, size, AZ, Region, OS or tenancy, and also apply to Fargate or Lambda usage. For example, with Compute Savings Plans, you can change from C4 to M5 instances, shift a workload from EU (Ireland) to EU (London), or move a workload from EC2 to Fargate or Lambda at any time and automatically continue to pay the Savings Plans price.
	
- **EC2 Instance Savings Plans**
	EC2 Instance Savings Plans provide the lowest prices, offering savings up to 72% in exchange for commitment to usage of individual instance families in a Region (e.g. M5 usage in N. Virginia). This automatically reduces your cost on the selected instance family in that region regardless of AZ, size, OS or tenancy. EC2 Instance Savings Plans give you the flexibility to change your usage between instances within a family in that region. For example, you can move from c5.xlarge running Windows to c5.2xlarge running Linux and automatically benefit from the Savings Plan prices.

### Spot Instances Pricing

With Spot Instances, you pay the Spot Price that's in effect for the time period your instance are running. Spot Instance price are set by Amazon EC2 and adjust gradually based on long-term  trends in supply and demand for Spot Instance capacity.

Spot Intances are available at a discount of up to 90% off compared to On-Demand pricing.