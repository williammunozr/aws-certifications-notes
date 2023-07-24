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
