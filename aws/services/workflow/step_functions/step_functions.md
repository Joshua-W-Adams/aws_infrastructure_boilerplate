# Step Functions

Orchestrate (coordinate) multiple AWS services with a visual workflow.

JSON document defines the workflow of the cloud functions.

## Error Handling

Error handling should be decoupled from the application code. Step functions provide two options to do this:

- Retry - retry step X amount of times
- Catch - after all retries, catch the error and send it to a specific step

ResultPath property can be used to pass information from one step to the next.

## Workflow Types

- Standard - Slower low throughput workflows
- Express - Fast high throughput workflows

## AWS Simple Workflow Service (SWF)

depreciated.