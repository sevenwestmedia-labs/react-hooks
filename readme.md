# React hooks

A collection of hooks we have created

## [use-script]('./packages/use-script')

Loads a third party script and returns a value when it's loaded or fails to load.

There are a few hooks out there but they do not handle concurrency or rendering multiple components which require the same script at the same time.
