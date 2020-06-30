<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [puppeteer](./puppeteer.md) &gt; [JSHandle](./puppeteer.jshandle.md) &gt; [evaluateHandle](./puppeteer.jshandle.evaluatehandle.md)

## JSHandle.evaluateHandle() method

This method passes this handle as the first argument to `pageFunction`<!-- -->.

<b>Signature:</b>

```typescript
evaluateHandle(pageFunction: Function | string, ...args: unknown[]): Promise<JSHandle>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  pageFunction | Function \| string |  |
|  args | unknown\[\] |  |

<b>Returns:</b>

Promise&lt;[JSHandle](./puppeteer.jshandle.md)<!-- -->&gt;

## Remarks

The only difference between `jsHandle.evaluate` and `jsHandle.evaluateHandle` is that `jsHandle.evaluateHandle` returns an in-page object (JSHandle).

If the function passed to `jsHandle.evaluateHandle` returns a Promise, then `evaluateHandle.evaluateHandle` waits for the promise to resolve and returns its value.

See [Page.evaluateHandle()](./puppeteer.page.evaluatehandle.md) for more details.
