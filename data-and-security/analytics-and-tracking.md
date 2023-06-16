# Analytics & Tracking

While the product is in alpha, we use analytics services to help us understand performance of the app as a whole, adoption of certain features, and how the latter impacts retention.

**Amplitude** is the main service we use for tracking _events_ inside the app. It allows us to track metrics such as:

* How many users joined in the past month & how many dropped
* How many Objects, Blocks, Sets, and Custom Types were created (and average that per number of active users)
* How much time people spend in the app, on average
* Which devices are used to login to the app

We use these to understand our main product metrics and whether overall, we’re moving in the correct direction. While we can track frequency and adoption of events, _we cannot in any way track the content you create._ I’d like to emphasize that this last point is foundational to us.

In practice, this means that we know for instance that custom Types are very popular, but we cannot see what these custom types are (nor which Objects you’ve created with those types).

Besides Amplitude, our engineering teams use Sentry to track the prevalence of crashes.
