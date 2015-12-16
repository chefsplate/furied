# furied
Publish private npm packages easily on [gemfury](http://fury.io).

## Global

```shell
npm i -g furied
```

Then on your project folder

```shell
furied <user> <key>
```

Or if you set the environment vars `GEMFURY_API_KEY` and `GEMFURY_USER`;

```shell
furied
```

done!

## Local
`npm i -D furied`

on your **package.json**

```json
{
  "scripts": {
    "private-publish": "furied <user> <key>"
  }
}
```

Then `npm run private-publish`. In a case that you want it right after `npm version <type>`:

```json
{
  "scripts": {
    "postversion": "furied <user> <key>"
  }
}
```

## Requirements
It's written in ECMA 2015 without transpilers. Node.js 4+

MIT License
(c) [Helder Santana](http://heldr.com)
