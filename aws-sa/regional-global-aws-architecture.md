# Regional & Global AWS Architecture

- Global Service Location & Discovery
- Content Delivery (CDN) and Optimization
- Global Health Checks & Failover
- Regional Entry Point
- Scaling & Resilience
- Application Services and Components

## Regional & Global AWS Architecture

## Global AWS Architecture

![Regional & Global Infrastructure 1](https://github.com/williammunozr/aws-sa-pro/blob/master/07-ComputeScalingLoadBalancing/00_LearningAids/RegionalandGlobalInfrastructure1.png)

## Regional AWS Architecture

![Regional & Global Infrastructure 2](https://github.com/williammunozr/aws-sa-pro/blob/master/07-ComputeScalingLoadBalancing/00_LearningAids/RegionalandGlobalInfrastructure2.png)

- Web Tier
    - Application Load Balancer (ALB).
    - API Gateway.
    - Act as entry point.
- Compute Tier
    - EC2.
    - Lambdas.
    - Containers (Like ECS).
- Storage Tier
    - EBS, EFS, S3.
    - S3 is used by CloudFront as origin.
- Caching Tier
    - Elastic Cache.
    - DynamoDB Accelerator (DAX) when using DynamoDB.
    - Reads to database can be decrease.
    - Apps will instead consult the cache first, and only the data that isn't present in the cache will be consulted from the DB, and the content in the cache will be apdated.
    - Cache is in-memory.
- DB Tier
    - RDS.
    - DynamoDB.
    - Redshift.
- App Services
    - Kinesis.
    - Step Functions.
    - SQS & SNS.
    - Decouple components using queues.
    
