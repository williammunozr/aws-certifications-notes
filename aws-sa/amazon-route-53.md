# Amazon Route 53

## Routing Policies

- **Simple Routing Policy** - This is used for a single resource (for example, a web server created for the `www.example.com` website).
- **Failover Routing Policy** - This is used to configure active-passive failover.
- **Geolocation Routing Policy** - This routes traffic based on the user's location.
- **Geoproximity Routing Policy** - This is used for geolocation when users are shifting from one location to another.
- **Latency Routing Policy** - This optimizes the best latency for the resources deployed in multiple AWS Regions.
- **Multivalue Answer Routing Policy** - This is used to respond to DNS queries with up to eight healthy, randomly selected records.
- **Weighted Routing Policy** - This is used to route traffic to multiple resource properties as defined by you (for example, you want to say `80%` traffic to site A and `20%`to site B).

You can build advanced routing policies by `nesting` these primary routing policies into traffic policies.

## Notes

- `Route 53` is the only service in which AWS offers `100% SLA`, which means AWS makes its best effort to ensure it is `100% available`.

## References

- [Routing Policy](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/routing-policy.html)
