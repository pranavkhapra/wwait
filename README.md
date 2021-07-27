# wwait

Hold on a sec, or the time you pass it.

`wait()` Returns a promise that resolves after how many milliseconds you pass it.

Great for waiting any amount of time. If you do not pass it any value, it will immediately resolve. This is handy when you need to ensure the following code is put at the end of the JS event callstack.

## Usage

```js
import wait from 'wwait';

async function doWhatFunctionSays() {
  doSomething();
  await wait();
  doSomethingElse();
  await wait(300);
  console.log('300ms later');
}

```
