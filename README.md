# 💅 prettier-config

[![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat)](https://github.com/prettier/prettier)

> An opinionated [Prettier config](https://prettier.io/).

## 🔗 Getting Started

### Install via NPM or Yarn:

Using `npm`:

```sh
npm install @ikscodes/prettier-config --save-dev
```

Using `yarn`:

```sh
yarn add -D @ikscodes/prettier-config
```

### Install required `peerDependencies`:


If using `npm@>7.x`, peer dependencies [will be installed automatically](https://github.blog/2021-02-02-npm-7-is-now-generally-available/), assuming no conflicts arise between peer dependency versions within your project.

If using **`npm@>5.x`**, use this shortcut (`yarn` will be automatically detected, if in use):

```sh
npx install-peerdeps --dev @ikscodes/prettier-config
```

Alternatively, Linux and macOS users can one of these commands:

```sh
# Using NPM:
(
  export PKG=@ikscodes/prettier-config;
  npm info "$PKG@latest" peerDependencies --json | command sed 's/[\{\},]//g ; s/: /@/g' | xargs npm install --save-dev "$PKG@latest"
)
```

```sh
# Using Yarn:
(
  export PKG=@ikscodes/prettier-config;
  npm info "$PKG@latest" peerDependencies --json | command sed 's/[\{\},]//g ; s/: /@/g' | xargs yarn add -D "$PKG@latest"
)
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

## 🗜️ Versioning

```
+————— Major version is synchronized with Prettier's major version.
| +——— Minor version has BREAKING CHANGES or features.
| | +— Patch version has non-breaking changes.
| | |
x.x.x
```

It's recommended that you pin the version of `@ikscodes/prettier-config` with a [semver tilde (`~`)](https://devhints.io/semver) so as to avoid unintended breaking changes when updating your NPM depedencies.

## ⚖️ License

[MIT](./LICENSE)
