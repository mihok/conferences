## Cost Optimization at Scale
##### Speaker: Shabaz Alam

Balance between Performance, Reliability, Security Cost, Optimization.

### **TCO**, Total Cost of Ownership

> "How much does it cost to keep the lights on"



> "Comparative total cost of ownership analysis (acquisition and operating costs) for running infrastructure environment end to end on premises vs on AWS"

- Server costs
- Storage costs
- Network costs
- IT Labour costs

- *Not Included: Facility, space, power, etc of each of the above (minus IT Labour)*

[Total Cost of Ownership Calculator](https://awstcocalculator.com)

##### Lowering TCO through cost Optimization
- Instance Right-sizing
- Improved Elasticity
- Measure, Monitor, Improve
- Optimized EC2
- Storage Optimization
- Serverless Architecture
- Managed Services

###  Cost Optimization is ...
Going from pay for what you **use** to pay for what you **need**.

##### Key Inputs
- Appropriate Pricing plans
- Periodic Review / Instance Resizing
- Shutdown Non-Prod Instances and EBS volumes
Gate Process / Architecture Review
- Governance (Indirect)
- Showbacks / Transparency (Indirect)
- Behavior Change / Incentive Alignment (Indirect)
- Limit Resource provisioning (Indirect)
- Implement automation (Indirect)

##### Four Pillars
###### Right-sizing
- Select cheapest instance available while meeting performance Requirements
- Looking at CPU RAM storage network utilization to identify potential instances that can be downsized
- Leverage Amazon CloudWatch metrics and setting up custom RAM metrics
- **Rule of thumb**: Right size, then reserver.

###### Reserved Instances
- RI Coverage: Step 1 (always on)
- RI Utilization: Step 2 (leverage RI flexibility to increase utilization, merge and split RIs as needed)
- **Rule of thumb**: Target 70-80% always -on coverage and 95% RI utilization rate.

###### Increase Elasticity
-  Turn off nonproduction Instances (Look for dev/test, non production instances that are always on and turn them off)
- Autoscale production (Scale up and down on demand, spikes)
- Using the right size, 29 m4.large vs 59 t2.medium ($2,505.60 vs $2,208.96)
- EC2 Spot Pricing, when excess capacity at Amazon exists, goes into spot market for auction at a significant discount
- **Rule of thumb**: Shoot for 20-30% of Amazon EC2 instances running on demand to be able to handle elasticity needs

###### Measure monitor, continuously Improve
-
