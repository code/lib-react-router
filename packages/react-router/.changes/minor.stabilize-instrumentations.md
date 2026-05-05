Stabilize the instrumentation APIs. `unstable_instrumentations` is now `instrumentations` and `unstable_pattern` is now `pattern`

- The `unstable_ServerInstrumentation`, `unstable_ClientInstrumentation`, `unstable_InstrumentRequestHandlerFunction`, `unstable_InstrumentRouterFunction`, `unstable_InstrumentRouteFunction`, and `unstable_InstrumentationHandlerResult` types have had their `unstable_` prefixes removed
- ⚠️ This is a breaking change if you have already opted into the unstable version - you will need to update your code accordingly
