<h1 align="center">Welcome to conventional-commit-spec 👋</h1>
<p>
  <img alt="Version" src="https://img.shields.io/badge/version-1.0.0-blue.svg?cacheSeconds=2592000" />
</p>

> 约定式提交、自动生成 changelog

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
