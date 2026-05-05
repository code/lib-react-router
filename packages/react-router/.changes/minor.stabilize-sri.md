Remove `unstable_subResourceIntegrity` from the runtime `FutureConfig` type; the flag is now controlled by the top-level `subResourceIntegrity` option in `react-router.config.ts`

- ⚠️ This is a breaking change if you have already opted into the unstable version - you will need to update your code accordingly
