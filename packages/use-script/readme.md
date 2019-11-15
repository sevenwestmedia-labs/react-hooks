# useScript

Loads a third party script and returns a value when it's loaded or fails to load.

There are a few hooks out there but they do not handle concurrency or rendering multiple components which require the same script at the same time.

## Example

```ts
const MyComponent = () => {
    const [loading, error] = useScript({
        src: '//cdn.bootcss.com/jquery/2.2.1/jquery.min.js',
    })

    if (loading || error) {
        return null
    }

    return <OtherComponentWhichNeedsJQuery />
}
```
