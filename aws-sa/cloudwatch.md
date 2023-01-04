# CloudWatch Architecture

## CloudWatch - Architecture Concepts

- `Ingestion`, `Storage` and `Management`of `Metrics`
- `Public` Service - public space endpoints
- .. `AWS Service Integration` - management plane
- .. `Agent` integration .. e.g. EC2 - richer metrics
- `On-Premises Integration` via Agent/API (custom metrics)
- .. `Application Integration` via API/Agent (custom metrics)
- View data via console UI, CLI, API, dashboards & anomaly detection
- `Alarms` ... react to metrics, can be used to notify or perform actions

## AWS CloudWatch - Architecture

![AWS CloudWatch Architecture](https://github.com/williammunozr/aws-sa-pro/blob/master/08-MonitoringLoggingCostManagement/00_LearningAids/CloudWatchArchitecture1.png)

## AWS CloudWatch - Data

- `Namespace` = `container` for `metrics` e.g. `AWS/EC2` & `AWS/Lambda`
- `Datapoint` = `Timestamp`, `Value`, (`optional`) `unit of measure`
- `Metric`.. `time ordered` set of `data points`
- .. `CPUUtilization`, `NetworkIn`, `DiskWriteBytes` - (EC2)
- Every metric has a `MetricName` (CPUUtilization) and a `Namespace` (AWS/EC2)
- Dimension .. name/value pair
- e.g. `CPUUtilization` Name=InstanceId, Value = i-11111111 (cat)
- e.g. `CPUUtilization` Name=InstanceId, Value = i-22222222 (cat)
- `AutoScalingGroupName`, `ImageId`, `InstanceId`, `InstanceType`
- `Resolution`.. Standard (60s granularity) .. High (1s)
- `Retention` .. sub 60s Retained for 3 hours
- 60s (1 minute) retained for 15 days
- 300s (5 minutes) retained for 63 days
- 3600s (1 hour) retained for 455 days
- As data ages, its `aggregated` and stored for `longer` with `less resolution`
- `Statistic` .. aggregation over a period (e.g. `Min`, `Max`, `Sum`, `Average`...)
- Percentile - e.g. p95 & p97.5

## CloudWatch - Data Architecture

![AWS CloudWatch Architecture](https://github.com/williammunozr/aws-sa-pro/blob/master/08-MonitoringLoggingCostManagement/00_LearningAids/CloudWatchArchitecture2.png)

## CloudWatch - Alarms

- `Alarm` - watches a metric over a time period
- ... `ALARM` or `OK`
- ... value of `metric` vs `threshold` .. over time
- ... one or more `actions`
- Alarm `Resolution`

## Resources

- [CloudWatch - Architecture Concepts](https://learn.cantrill.io/courses/895720/lectures/23304604)
