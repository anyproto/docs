# Analytics & Tracking

{% hint style="info" %}
It will be possible to opt-out of analytics in the [future](https://github.com/orgs/anyproto/projects/1/views/1?pane=issue\&itemId=29227689).
{% endhint %}

While the product is still in pre-release, we use analytics services to help us understand performance of the app as a whole, adoption of certain features, and how the latter impacts retention.

Analytics consists of two parts: low-level analytics at the network level and app usage analytics at the client level. Both types are anonymous and do not analyze the content you are working with, as it is encrypted.

{% hint style="info" %}
If you switch to self-hosted or local-only network mode, Anytype Network does not collect low-level analytics. However, app usage analytics are still reported.
{% endhint %}

**Amplitude** is the main service we use for tracking _events_ inside the app. It allows us to track metrics such as:

* How many users joined in the past month & how many dropped
* How many Objects, Blocks, Sets, and Custom Types were created (and average that per number of active users)
* How much time people spend in the app, on average
* Which devices are used to log in to the app

We use these to understand our main product metrics and whether overall, we’re moving in the correct direction. While we can track frequency and adoption of events, _we cannot in any way track the content you create._

In practice, this means that we know for instance that custom Types are very popular, but we cannot see what these custom types are (nor which Objects you’ve created with those types).

Besides Amplitude, our engineering teams use Sentry to track the prevalence of crashes.

{% hint style="info" %}
The only way to disable analytics at the moment is to either block outgoing connections to analytics-related hosts, or to edit the relevant source code and rebuild the client for your own use.
{% endhint %}





