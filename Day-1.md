## AWS - Cloud Computing
- 1 subnet = 1 AZ ( Availability Zone)
### 1. models of cloud:
- Private cloud: used by a single org and not public (rackspace)
- Public cloud: owned by 3-party cloud service (aws, gg cloud)
- Hybrid Cloud: control private infra to public cloud (private + public)
### 2. Cloud computing types:
- **Infra**structure as a Service (IaaS): EC2, Azure, Rackspace
- **Platform** as a Service (PaaS): Elastic Beanstalk, Heroku, GCP (use to manage only apps and data)
- **Software** as a Service (SaaS): Rekognition, Gmail, Zoom
### 3. Pricing of the cloud: (3 types following the pay-as-you-go model)
- Compute: pay for compute time
- Storage: pay for data stored
- Data transfer OUT of the cloud (IN is free) **(?)**
### 4. AWS infrastructure:
- AWS Regions: us-east-1, eu-west-3,.. (is a cluster of data centers)

  -> Choose a region (4): properties of data (such as gov data is only stored in his country), proximity to customer (for reducing latency), available services and features within a Region and pricing is dependent on price page
- AWS availability zones: 1 region has 2 or more AZs called us-east-1a, us-east-1b,..
  
  Each AZ is 1 or n data centers
  
  Each AZ is separate, connected with ultra-low latency network together
- AWS points of presence (edge locations):  content is delivered lower latency
### 5. Shared responsibility model diagram:
- Customer is responsible to the security in the cloud
- AWS is responsible for the security of international cloud ([link](https://aws.amazon.com/compliance/shared-responsibility-model/))
### 6. AWS acceptable use policy:
- AWS not accept your unauthorized, harmful, security violation, network & data abuse

