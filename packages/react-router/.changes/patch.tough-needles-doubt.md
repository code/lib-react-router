Improve route matching performance in Framework/Data Mode ([#14971](https://github.com/remix-run/react-router/pull/14971))

- Avoiding unnecessary calls to `matchRoutes` in data router scenarios
  - This includes adding back the optimization that was removed in `7.6.0` ([#13562](https://github.com/remix-run/react-router/pull/13562))
  - The issues that prompted the revert have been addressed by using the available router `matches` but always updating `match.route` to the latest route in the `manifest`
- Leverage pre-computed pre-computing flattened/cached route branches during client side route matching
- Performance benchmarks showed roughly a 15-30% improvement in server-side request handling performance
