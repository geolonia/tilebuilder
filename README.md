# tilebuilder

`data/` に Shapeファイルを配置して以下を実行すると、`tiles` にベクトルタイルが作成されます。

```bash
$ npm install
$ npm run build
```

### タイルのカスタマイズ

`$ npm run build` を実行すると、`tiles` ディレクトリ以下に `kata.yml` が生成されます。任意でベクトルタイルの設定を変更してください。

```yaml
airport:
  source: ./data/airport.geojson
  properties:
    name: properties["name:ja"]
  minzoom: 9
  maxzoom: 14
town:
  source: ./data/town.geojson
  properties:
    title: properties.label
  minzoom: 9
  maxzoom: 14
```

## プレビュー

作成したベクトルタイルをプレビューすることができます。

```bash
$ npm start
```

## デプロイ

```bash
$ npm run deploy
```
