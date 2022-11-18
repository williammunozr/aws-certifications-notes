# Session Stickiness

## Connection Stikiness

![Connection Stikiness](https://github.com/williammunozr/aws-sa-associate-saac03/blob/main/1500-HA_and_SCALING/00_LEARNINGAIDS/SessionStickiness.png)

### Stikiness Key Points

- Stikiness locks a session to 1 backend instance.
- Creates AWSALB .. which is held by the client.
- Sessions move on expiry or instance failure.
- Enable if an application doesn't use external sessions.
- Look for question keywords logout, lost carts, lost progress... These suggest lost session state.

## ALB Session Stickiness

![ALB Session Stikiness](https://github.com/williammunozr/aws-sa-pro/blob/master/07-ComputeScalingLoadBalancing/00_LearningAids/ALBArchitecture3.png)


## References

- [Session Stickiness](https://learn.cantrill.io/courses/895720/lectures/22009494)