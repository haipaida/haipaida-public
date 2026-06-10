# How We Evaluate Network Changes

Not every network change is an improvement.

A route may become faster while becoming less stable.

A route may become more stable while increasing latency.

Because of this, we avoid judging changes based on a single test result.

When evaluating a change, we typically observe:

* Latency
* Stability
* Packet loss
* Consistency over time
* User experience

We prefer repeatable improvements over temporary gains.

Small improvements that remain stable are usually more valuable than large improvements that disappear after a few hours or days.

Our goal is not the best benchmark result.

Our goal is predictable performance.
