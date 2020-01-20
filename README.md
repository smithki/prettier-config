# 💅 prettier-config

[![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat)](https://github.com/prettier/prettier)

> An opinionated [Prettier config](https://prettier.io/).

## 🔗 Getting Started

### Install via NPM or Yarn:

```sh
npm install @ikscodes/prettier-config --save-dev
```

```sh
yarn add -D @ikscodes/prettier-config
```

## 🛠️ Usage

If you don't need additional settings or overrides, you can set the `prettier` key in `package.json`:

```javascript
{
  "prettier": "@ikscodes/prettier-config"
}
```

Or, if you need more flexibility, you can use `require` in `.prettierrc.js`:

```javascript
module.exports = {
  ...require('@ikscodes/prettier-config'),
  // ...Override settings ad hoc
}
```

## ⚖️ License

[MIT](./LICENSE)
