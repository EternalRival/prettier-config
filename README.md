# @eternalrival/prettier-config

Prettier [sharing configuration](https://prettier.io/docs/en/sharing-configurations)

## Using a Shareable Config

### Installation

```sh
npm install -D @eternalrival/prettier-config
```

### Usage

You can reference it in your `package.json`

```json
{
  "name": "my-cool-repo",
  "version": "1.0.0",
  "prettier": "@eternalrival/prettier-config"
}
```

or extend it in your `prettier.config.mjs`

```js
import erPrettierConfig from "@eternalrival/prettier-config";

/**
 * @type {import("prettier").Config}
 */
const config = {
  ...erPrettierConfig,
  /* your rules */
};

export default config;
```
