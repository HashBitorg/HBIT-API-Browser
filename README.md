# HBIT-API-Node-Browser
============

API request wrapper for [HBIT crypto](https://hashbit.org/api.html) for browser.
It just has all the currently public API methods for HBIT along side with a dual API Promise/Callback based interface.

Plus it's created using Typescript, which should ensure the proper parameters for each API call.

## Install


In the browser (needs to have `nxt.apiServerCORS=true` in your NXT config file, otherwise you need to access it from same port and hostname):

```html
<script src="hbit-api.js"></script>
<script>
    var instance = new HBIT.API('http://127.0.0.1:11120');

    instance.getNextBlockGenerators().then(function(answer){
        console.log(answer);
    });
</script>
```
