# vite-dev-server-crashes

If you edit `vite.config.js` and introduce a syntax error, the dev server crashes.

```
git clone git@github.com:Rich-Harris/vite-dev-server-crashes
cd vite-dev-server-crashes
npm i
npm run dev
```

Then, in a separate terminal tab:

```
npm run break
```

## Expected behaviour

The syntax error is reported, but the dev server stays alive and gracefully recovers once the error is fixed.

Ideally this would be the case for anything that errors on startup.

## Actual behaviour

💥
