# How We Decide When Not To Change A Route

Not every network problem requires a route change.

Sometimes the best decision is to leave a stable route unchanged.

## A Change Should Solve A Real Problem

Before changing a route, we first ask whether there is a clear problem to solve.

Examples include:

- Repeated packet loss
- Unstable latency
- Consistent peak-hour degradation
- Poor routing toward a specific destination
- A reproducible difference between available paths

If the current route is already stable and suitable for the use case, changing it may add risk without providing meaningful benefit.

## Small Differences May Not Matter

Two routes may produce slightly different latency numbers while providing nearly identical real-world performance.

For example, a route that averages 78 ms is not automatically worse than one that averages 74 ms.

If both remain stable, loss-free, and predictable, the difference may not justify a change.

## Every Change Introduces New Variables

Changing a route can affect more than latency.

It may also change:

- Path consistency
- Packet loss behaviour
- Peak-hour performance
- Return routing
- Reliability over time

A change that improves one measurement can make another part of the connection worse.

## Stability Is Evidence Too

When a route has remained stable across repeated use and testing, that history has value.

Replacing a known stable path with an unproven alternative should have a clear reason.

We do not change routes simply because another option looks better in one isolated test.

## Re-Test Before Making A Decision

If a possible improvement appears, we try to reproduce it under comparable conditions.

We may compare:

- Different testing times
- Repeated measurements
- Real application behaviour
- Latency variation
- Packet loss
- Route consistency

If the advantage does not remain consistent, there may be no strong reason to change.

## Sometimes The Correct Decision Is No Change

Optimization does not mean changing something constantly.

It means making changes when the evidence supports them and leaving stable systems alone when it does not.

A route that is already predictable, stable, and suitable for its purpose may be better left unchanged.
