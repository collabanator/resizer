# resizer
Need to resize images and other content? Resizer can do that for you.

## What can I do?
I was just born so more details to come. But the initial vision is that I am a stateless utility service. I should be able to help with the following.

### near term
* receive a command via Kafka or HTTP API with an image reference, resize it per the command, output a new image and respond with status 
* run in a OCI compliant container
* track my own performance
 
### further out
* support for knative (serverless) so I only run when I'm needed at the scale I'm needed
* provide my performance as metrics (prometheus?)
* be configured to securely access cloud blob/bucket storage
