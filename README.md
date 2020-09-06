### Motivation

Way before the ReScript compiler moved to OCaml 4.06.1, I liked the richness and interface provided by Jane Street's `ppx_let`, but I haven't had the chance to target native. It was time to give it a try in JavaScript-land.

### Installing

In your terminal, run:

```sh
yarn add --dev @leeor/rescript-ppx-let
```

Edit `bsconfig.json`:

```json
  "ppx-flags": [
    ["@leeor/rescript-ppx-let/ppx.exe", "-as-ppx"]
  ]
```

The specifics of using this PPX are very well documented in the original [README](https://github.com/janestreet/ppx_let).
