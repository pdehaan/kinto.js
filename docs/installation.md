# Installing Kinto.js

## NodeJS

If you're using [NodeJS](https://nodejs.org) and [npm](https://www.npmjs.com/) as a frontend package manager, you'll need [NodeJS v0.12.x](https://nodejs.org/download/) installed on your system. Then:

```js
$ npm install kinto --save-dev
```

> #### Notes
>
> *Read more about how to build Kinto.js in the [Hacking section](hacking.md).*

## Static assets

Dev and production ready assets are available in the [`dist` folder of the repository](https://github.com/Kinto/kinto.js/tree/master/dist). You can either download an archive of the code and use these files in your own project, or link to static assets served through [rawgit](http://rawgit.com/):

### Latest master

- Dev version, including source maps: [kinto.dev.js](https://rawgit.com/Kinto/kinto.js/master/dist/kinto.dev.js)
- Production version, minified, no source maps: [kinto.dev.js](https://rawgit.com/Kinto/kinto.js/master/dist/kinto.min.js)

### Latest tag

- Dev version, including source maps: [kinto.dev.js](https://cdn.rawgit.com/Kinto/kinto.js/1.0.0-rc.1/dist/kinto.dev.js)
- Production version, minified, no source maps: [kinto.dev.js](https://cdn.rawgit.com/Kinto/kinto.js/1.0.0-rc.1/dist/kinto.min.js)


### Subresource integrity

To make sure that you are using the right code when loading from a CDN, you can use subresource
integrity with the hash provided in ``kinto.min.sha384`` with your release.

For 1.0.0-rc.1, please use it like the following:

.. code-block:: html

    <script src="https://cdn.rawgit.com/Kinto/kinto.js/1.0.0-rc.1/dist/kinto.min.js"
            integrity="sha384-2EBP0zFAKrL1idZDEzowmRmkeEFAneGUwGUHKmGSWKtTtHRQPbyOJyCk0xCgT1pC"
            crossorigin="anonymous">
    </script>

Where ``2EBP0zFAKrL1idZDEzowmRmkeEFAneGUwGUHKmGSWKtTtHRQPbyOJyCk0xCgT1pC``
is the value in ``dist/kinto.min.sha384``.

If you need to calculate your subresource integrity hash please use
https://srihash.org/.
