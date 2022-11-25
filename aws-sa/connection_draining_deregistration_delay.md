# Connection Draining & Deregistration Delay

## Connection Draining

- What happens when instances are `unhealthy` ... or deregistered.
- Normally `all connections are closed` & `no new connections` ...
- `Connection draining` allows `in-flight` requests to `complete`.
- `CLASSIC LOAD BALANCER ONLY` - defined on the CLB.
- Timeout: Between `1` and `3,600` Seconds (default 300).
- InService: Instance deregistration currently in progress.
- Auto Scaling waits for all connections to complete or Timeout.

## Deregistration Delay

- Supported on `ALB`, `NLB` and `GWLBs` (subtle differences).
- Defined on the `Target group` - NOT the LB.
- Stops sending requests to deregistering targets.
- Existing connections can continue.
- ... until they `complete naturally`.
- ... or the `deregistration delay` is reached.
- Default `300` seconds (`0-3600` seconds).