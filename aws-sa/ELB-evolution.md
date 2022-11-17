# Evolution of Elastic Load Balancers (ELB)

- 3 Types of Load Balancers (ELB) available within AWS.
- Split between `v1` (avoid / migrate) and v2 (prefer).
- Classic Load Balancer (CLB) - v1 - introduced in 2009.
- Not really layer 7, lacking features, 1 SSL per CLB.
- Application Load Balancer (ALB) - `v2` - HTTP/S/WebSocket
- Network Load Balancer (NLB) - v2 - TCP, TLS & UDP.
- V2 = faster, cheaper, support target groups and rules.

## References

- [ELB Evolution](https://learn.cantrill.io/courses/895720/lectures/24106630)
