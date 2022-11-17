# Application and Network Load Balancer (ALB vs NLB)

## Load Balancer Consolidation

![Load Balancer Consolidation](https://github.com/williammunozr/aws-sa-pro/blob/master/07-ComputeScalingLoadBalancing/00_LearningAids/ALBArchitecture1.png)

## Application Load Balancer (ALB) Key Points

- `Layer 7` Load Balancer .. listens on `HTTP` and/or `HTTPS`.
- `No other Layer 7 protocols` (SMTP, SSH, Gaming ...).
- ... and `No TCP/UDP/TLS Listeners`.
- Can inspect L7 content type, cookies, custom headers, user location and app behaviour.
- `**` HTTP and HTTPS (SSL/TLS) always terminated on the ALB. - `No unbroken SSL` (security teams!).
- ... `a new connection` is made to the application.
- ALBs `MUST` have `SSL` certs if `HTTPS` is used.
- ALBs are `slower` than `NLB` .. more levels of the network stack to process.
- Health checks `evaluate application health` ... layer 7.

## Application Load Balancer (ALB) - Rules

- Rules `direct connections` which `arrive` at a `listener`.
- Processed in `priority order`.
- `Default rule` = `catchall`.
- `Rule Conditions`: host-header, http-header, http-request-method, path-pattern, query-string & source-ip.
- `Actions`: forward, redirect, fixed-response, authenticate-oidc & authenticate-cognito.

![ALB - Rules](https://github.com/williammunozr/aws-sa-pro/blob/master/07-ComputeScalingLoadBalancing/00_LearningAids/ALBArchitecture2.png)

## Network Load Balancer (NLB)

- `Layer 4 Load Balancer` ... TCP, TLS, UDP, TCP_UDP.
- `No visibility` or `understanding` of HTTP or HTTPS.
- `No headers`, `no cookies`, `no session stickiness`.
- Really Really Really Fast (`millions of Requests Per Second`, 25% of `ALB Latency`).
- ... SMTP, SSH, Game Servers, Financial Apps (not HTTP/S)
- Health checks `JUST` check ICMP / TCP Handshake .. `Not app aware`.
- NLB's can have `static IP's` - useful for whitelisting.
- `Forward TCP` to instances ... `unbroken encryption`.
- Used with private link to provide services to other VPCs.

## References

- [Application and Network Load Balancer](https://learn.cantrill.io/courses/895720/lectures/23012749)
