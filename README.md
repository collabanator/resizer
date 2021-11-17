# resizer
Need to resize images and other content? Resizer can do that for you.

## What can I do?
I was just born so more details to come. But the initial vision is that I am a stateless utility service. I should be able to help with the following.

### near term
* receive a command via Kafka or HTTP API with an image (jpeg,png) reference, resize it per the command, output a new image and respond with status 
* run in a OCI compliant container
* track my own performance
 
### further out
* support for knative (serverless) so I only run when I'm needed at the scale I'm needed
* provide my performance as metrics (prometheus?)
* alert when things go wrong
* be configured to securely access cloud blob/bucket storage
* lots of image types support (gifs, HEIF, HEVC)
* leverage GPUs when available

## Why
A photo taken on a currrent iPhone is typically 12MP / 3024 x 4032 / ~4MB on device / ~18MB as png <- that's really big! Typically when sharing with someone that full resolution is overkill, we just want something that looks pretty good on our mobile device or laptop screen. Transfering and keeping all those big files around can get expensive in terms of performance as well as cloud storage costs.
