<h1 align="center">Welcome to conventional-commit-spec 👋</h1>
<p>
  <img alt="Version" src="https://img.shields.io/badge/version-1.0.1-blue.svg?cacheSeconds=2592000" />
</p>

> 约定式提交、格式校验、自动生成 changelog

## 安装

```sh
yarn
```

## 约定式提交

```sh
yarn add commitizen -D
```

```sh
yarn add cz-conventional-changelog -D
```

```json
#  package.json
{
  "scripts": {
    "commit": "git-cz"
  },
  "config": {
    "commitizen": {
      "path": "./node_modules/cz-conventional-changelog"
    }
  }
}
```

## 约定式提交格式校验

```sh
yarn add @commitlint/config-conventional @commitlint/cli -D

yarn add hooks lint-staged -D
```

```json
# package.json

{
  "config": {
    "commitizen": {
      "path": "./node_modules/cz-conventional-changelog"
    },
    "commitlint": {
      "extends": [
        "@commitlint/config-conventional"
      ]
    },
    "lint-staged": {
      "src/**/*.{js,ts,css,vue,tsx,jsx}": [
        "npm run lint",
        "git add"
      ]
    }
  }
}
```

## 自动生成 changelog

```sh
yarn add standard-version conventional-changelog -D
```
