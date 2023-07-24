# CloudFormation

## CloudFormation Physical and Logical Resources

- CloudFormation Template - YAML or JSON
- .. contains logical resources - the "WHAT"
- Templates are used to create `Stacks`
- .. 1 stack, 100 stacks, 20.. stacks in each region
- .. stacks create `physical resources` from logical
- If a stacks template is changed - `physical` resources are changed
- If a stack is `deleted`, normally, the `physical` resources are delete

## Physical and Logical Resources

![Physical and Logical Resources](../images/cf-physical-and-logical-resources.png)

![Physical and Logical Resources Lifecycle](../images/cf-physical-and-logical-resources-lifecycle.png)

## Template and Pseudo Parameters

- `Template Parameters` accept input - console/CLI/API
- .. when a stack is `created` or `updated`
- Can be referenced from within `Logical Resources`
- .. influence `physical resources` and/or configuration
- Can be configured with `Defaults`, `AllowedValues`, `Min` and `Max` length & `AllowedPatterns`, `NoEcho` & `Type`

## Template Parameters

![CF Template Parameters](../images/cf-template-parameters.png)

## Pseudo Parameters

![CF Pseudo Parameters](../images/cf-pseudo-parameters.png)

## CloudFormation Intrinsic Functions

- Ref & Fn::GetAtt
- Fn::Join & Fn::Split
- Fn::GetAZs & Fn::Select
- Conditions (Fn:: IF, And, Equals, Not or Or)
- Fn::Base64 & Fn::Sub
- Fn::Cidr

### Ref and Fn::GetAtt

![Ref and Fn::GetAtt](../images/ref-and-fn-getatt.png)

### Fn::GetAZs and Fn::Select

![Fn GetAZs and Fn Select](../images/fn-getazs-and-fn-select.png)

### Fn::Join and Fn::Split

![Fn Join and Fn Split](../images/fn-join-and-fn-split.png)

### Fn::Base64 and Fn:Sub

![Fn Base64 and Fn Sub](../images/fn-base64-and-fn-sub.png)

### Fn::Cidr

![Fn Cidr](../images/fn-cidr.png)

## CloudFormation Mappings

![CloudFormation Mappings](../images/cf-mappings.png)

![CloudFormation Mappings Example](../images/cf-mappings-example.png)

## CloudFormation Outputs

![CloudFormation Outputs](../images/cf-outputs.png)
